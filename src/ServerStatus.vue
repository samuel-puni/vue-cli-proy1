<template>
    <div>
        <p>Estado del servicio:  {{ status}}</p>
        <hr>
        <button @click="changeStatus">Cambia Estado</button>
    </div>
</template>

<script>
    export default {
        data: function() {
            return { status: 'Critical' }
        },
        methods: { 
            changeStatus() {
                this.status = 'Normal';
            }
        },
    }
</script>