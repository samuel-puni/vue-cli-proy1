<template>
    <p>Service Staus:  {{ status}}</p>
    <hr>
    <button @click="changeStatus">Change Status</button>
</template>

<script>
    export default {
        data: function() {
            return {
                status: 'Critical'
            }
        },
        methods: { 
            changeStatus() {
                this.status = 'Normal'
            }
        },
    }
</script>