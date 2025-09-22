<script>
    export default { 
        data() {
            return {
                // Add code here
                isRed: false,
                id: "demo1"
            }
        },
        methods: { 
   			// Add code here
		}
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" class="m-2" :class="isRed ? 'redBox':'blueBox'">
            div ID : {{id}} 
        </div>
        
        <button type="button" :class="isRed ? 'btn-danger': 'btn-secondary'" @click="isRed = !isRed">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
