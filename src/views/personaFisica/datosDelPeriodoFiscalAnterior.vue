<template>
    <el-card class="elcardFiscalAnterior">
        <div>
            Estos datos solo deben completarse la primera vez que se liquide el Impuestos
            a las ganancias con este sistema. En los años siguientes, estos datos se tomarán
            de la declaracion jurada anterior.
        </div>
        <el-col justify="center">
            <div class="block">Año fiscal:
                <el-date-picker v-model="value4" type="year" placeholder="Año">
                </el-date-picker>
            </div>
        </el-col>
        <el-row :gutter="20">
            <el-col justify="center">Capital Afectado a la actividad
                <div>Bienes de cambio
                    <el-input-number controls-position="right" v-model="bienes" :precision="2" :step="0.1" :min="1" />
                </div>
                <div>Total del activo
                    <el-input-number controls-position="right" v-model="activo" :precision="2" :step="0.1" :min="1" />
                </div>
                <div>Total del pasivo
                    <el-input-number controls-position="right" v-model="pasivo" :precision="2" :step="0.1" :min="1" />
                </div>
            </el-col>
        </el-row>
        <div>
            <el-button type="default" size="default" >Declaracion de bienes y deudas...</el-button>
        </div>
        <div class="divisorbutton">
            <el-button>Procesar</el-button>
            <el-button>Cancelar</el-button>
        </div>
    </el-card>
</template>

<script>
export default {
    name: 'TiempoImpuestosDatosDelPeriodoFiscalAnterior',

    data() {
        return {
            value4: '',
            bienes: '',
            activo: '',
            pasivo: '',

        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>

<style scoped>
.elcardFiscalAnterior {
    max-width: 800px;
}
.divisor2 {
    margin-bottom: 1%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}
.divisorbutton {
    margin-bottom: 1%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;

}
</style>