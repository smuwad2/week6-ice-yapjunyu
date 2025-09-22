<script>
    export default { 
       // add code here
        data() {
            return {
                selectVal: "username"
            };
        },
    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="selectVal">
        <option value="username">Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div v-if="selectVal == 'username'">
        <label>Username</label>
        <input placeholder="Enter your username">
    </div>
    <div v-else>
        <label>Email</label>
        <input placeholder="Enter your email">
    </div>
</template>

