<template>
    <el-card class="elcardFiscalAnterior">
        <div>
            Estos datos solo deben completarse la primera vez que se liquide el Impuestos
            a las ganancias con este sistema. En los años siguientes, estos datos se tomarán
            de la declaracion jurada anterior.
        </div>
        <el-col justify="center">
            <span class="block">Año fiscal:
                <el-date-picker class="yearpickerclass" v-model="inputs.año" type="year" placeholder="Año">
                </el-date-picker>
            </span>
        </el-col>
        <el-form :label-position="labelPosition" label-width="350px" :model="formLabelAlign">
            <el-form-item class="modaldatosperiododivisor" label="Bienes de cambio">
                <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.bienes" :precision="2"
                    :step="0.1" :min="0" />
            </el-form-item>
            <el-form-item class="modaldatosperiododivisor" label="Total del activo">
                <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.activo" :precision="2"
                    :step="0.1" :min="0" />
            </el-form-item>
            <el-form-item class="modaldatosperiododivisor" label="Total del pasivo">
                <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.pasivo" :precision="2"
                    :step="0.1" :min="0" />
            </el-form-item>
        </el-form>
        <div>
            <el-button type="default" size="default">Declaracion de bienes y deudas...</el-button>
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
            inputs: {
                bienes: '0',
                activo: '0',
                pasivo: '0',
                año: '0',
            },

            labelPosition: 'right',
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

.modaldatosperiododivisor {
    margin-bottom: 1%;
    width: 600px;
    margin-top: 1%;
}

.inputnumberclass {
    border: solid 1.5px #C0C0C0;
    background-color: #C0C0C0;
}

.yearpickerclass {
    border: #C0C0C0;
    background-color: #C0C0C0;
}</style>