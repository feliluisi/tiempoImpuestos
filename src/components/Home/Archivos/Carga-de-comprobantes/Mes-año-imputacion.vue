<template>
    <el-card>
        <el-header>
            <h4> Ingrese mes/año de imputación que se utilizará para los comprobantes que se ingresarán al sistema.</h4>
        </el-header>

        <h4>Mes/Año de la imputación: <input placeholder="11-2022"/></h4>
        <el-col ><div><el-button>Seguir</el-button></div></el-col>
    </el-card>        
</template>

<script>    

export default {
    name: 'TiempoImpuestosMesAOImputacion',
    data() {
        return {
            
        };
    },

    mounted() {
        
    },

    methods: {
        
    },
};
</script>

<style scoped>

</style>