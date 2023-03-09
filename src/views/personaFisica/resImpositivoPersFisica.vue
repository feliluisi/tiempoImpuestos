<template>
    <el-card>
        <el-form :inline="true" :model="formInline" class="demo-form-inline">
            <el-form-item class="yearinputpersfisc" label="Año">
                <el-date-picker v-model="formInline.user" type="year" placeholder="Año"></el-date-picker>
            </el-form-item>
            <el-form-item label="DDJJ">
                <el-input class="inputpersfisc" v-model="formInline.user" placeholder="DDJJ"></el-input>
            </el-form-item>
            <el-form-item label="Actv.">
                <el-input class="inputpersfisc" v-model="formInline.user" placeholder="Activ."></el-input>
                <el-button class="botonpersfisc">?</el-button>
            </el-form-item>
            <el-form-item label="DGI">
                <el-input class="inputpersfisc" v-model="formInline.user" placeholder="DGI"></el-input>
                <el-button class="botonpersfisc">?</el-button>
            </el-form-item>
        </el-form>
        <el-row class="tabladivisora">
            <el-col :span="12">
                <div>Ingresos computables</div>
                <div>Costo de ventas</div>
                <div>Gastos coputables</div>
                <div>Deducc. no erogan fondos</div>
                <div>Rtado. vta. bienes de uso</div>
                <div>Otros</div>
                <div>Diferencia</div>
            </el-col>
            <el-col :span="6">
                <div style="margin: 25px;"></div>
                <div>316,000.00</div>
                <div>1,980</div>
                <div>4,200</div>
                <div>0.00</div>
                <div>0.00</div>
                <div>0.00</div>
            </el-col>
            <el-col :span="4">
                <div>360,545.45</div>
                <div style="margin: 70px;"></div>
                <div>4,000</div>
                <div>0.00</div>
                <div>42,365.45</div>
            </el-col>
        </el-row>
        <div style="margin: 25px;"></div>
        <el-row>
            <el-col :span="12">
                <div>Ingresos exentos en el impuesto a las ganancias</div>
                <div>Compras y gastos atribuibles a ganancias exentas</div>
            </el-col>
            <el-col :span="4"></el-col>
            <el-col :span="4"></el-col>
            <el-col :span="4">
                <div>0.00</div>
                <div>0.00</div>
            </el-col>
        </el-row>
        <div style="margin: 25px;"></div>
        <el-row class="tabladivisora">
            <el-col :span="6">
                <div style="margin: 25px;"></div>
                <div>1998</div>
                <div>1999</div>
            </el-col>
            <el-col :span="6">
                <div>Activo</div>
                <div>789,645.00</div>
                <div>36,870.00</div>
            </el-col>
            <el-col :span="6">
                <div>Pasivo</div>
                <div>12,340.00</div>
                <div>6,560.00</div>
            </el-col>
            <el-col :span="6">
                <div>Capital</div>
                <div>777,314.00</div>
                <div>30,310.00</div>
            </el-col>
        </el-row>
        <div style="margin: 25px;"></div>
        <el-row :gutter="20">
            <el-col :span="3">
                <el-button type="default" size="default">Participación</el-button>
            </el-col>
            <el-col :span="4">
                <el-button type="default" size="default">Imprimir</el-button>
            </el-col>
            <el-col :span="13">
            </el-col>
            <el-col class="columnapersfisc" :span="4">
                <el-button type="default" size="default">Cerrar</el-button>
            </el-col>
        </el-row>
    </el-card>
</template>

<script>
export default {
    name: 'TiempoImpuestosResImpositivoPersFisica',

    data() {
        return {
            formInline: {
                user: '',
                region: ''
            }
        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>

<style scoped>
.inputpersfisc {
    width: 100px;
}

.yearinputpersfisc {
    width: 150px;
}

.el-card {
    width: 900px;
}

.botonpersfisc {
    color: gray;
    margin-left: 5px;
}

.tabladivisora {
    border: solid 1.5px #C0C0C0;
    background-color: #C0C0C0;
}

.botonpersonafisica {
    margin-bottom: 1%;
    display: flex;
    flex-direction: row;
    justify-content: left;
}

.columnapersfisc {}
</style>