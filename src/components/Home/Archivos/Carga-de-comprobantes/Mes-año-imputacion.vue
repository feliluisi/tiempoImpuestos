<template>
    <div>
        <el-header>
            <h2> Ingrese mes/año de imputación que se utilizará para los comprobantes que se ingresarán al sistema.</h2>
        </el-header>
    </div>
    <div>
        <h2>Mes/Año de la imputación: <input placeholder="11-2022" v-model="input"/></h2>
        <el-col :span="6"><div class="grid-content bg-purple"><el-button>Seguir</el-button></div></el-col>
        
    </div>
    

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

<style lang="scss" scoped>

</style>