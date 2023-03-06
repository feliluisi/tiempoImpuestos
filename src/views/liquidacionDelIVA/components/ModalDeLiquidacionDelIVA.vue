<template>
    <el-card>
        <el-card>
            <el-row>
                <div>
                    <el-button>NUEVA LIQUIDACIÓN DEL IVA</el-button>
                </div>
            </el-row>

            <br>
            <el-row>
                <div>
                    <el-button>LIQUIDACIÓN DEL IVA ANTERIOR</el-button>
                </div>
            </el-row>

        </el-card>
        <br>
        <el-button>Cancelar</el-button>
    </el-card>
</template>

<script>
export default {
    name: 'TiempoImpuestosModalDeLiquidacionDelIVA',

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
.el-button {
    min-width: 250px;
}
</style>