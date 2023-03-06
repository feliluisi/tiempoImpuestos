<template>
    <el-card>
        <div>
            <el-form-item>
                <el-col justify="center">
                    <div class="block">Mes y Año:
                        <el-date-picker v-model="value2" type="month" placeholder="Mes">
                        </el-date-picker>-
                        <el-date-picker v-model="value2" type="year" placeholder="Año">
                        </el-date-picker>
                    </div>
                </el-col>
            </el-form-item>
            <div class="divisorbutton">
                <el-button>Procesar</el-button>
                <el-button>Cancelar</el-button>
            </div>
        </div>
    </el-card>
</template>

<script>
export default {
    name: 'TiempoImpuestosLiquidacionDelIVAFecha',

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
.divisorbutton {
    margin-bottom: 1%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;

}
</style>