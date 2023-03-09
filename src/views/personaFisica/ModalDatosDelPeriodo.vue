<template>
  <el-card>
    <el-select v-model="value" class="selectcoloragugsto" placeholder="Socio--CUIT">
      <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value">
      </el-option>
    </el-select>
    <div style="margin: 20px;"></div>
    <el-form :label-position="labelPosition" label-width="350px" :model="formLabelAlign">
      <el-form-item class="modaldatosperiododivisor" label="Inmuebles">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.inmuebles" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Automotores, embarciones y aeronaves">
        <el-input-number class="inputnumberclass" controls-position="right" v-model="inputs.autoEmbarcaAero" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Cap. afec. a 3ª y 4ª cat. y otras p.s.">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.capAfecyotras" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Cta. cte. y caja de ahorro">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.ctaCteyCajaA" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Inversiones en entidades financieras">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.inversionesE" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Resto de bienes en el pais">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.restBienesPais" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Bienes en el exterior">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.bienesExte" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Deudas con personas fisicas">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.deudasPersFisica" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Otras deudas en el pais">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.otrasDeudasPais" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Deudas con personas fisicas del exter.">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.deudasPersFisicaExte" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Otras deudas en el exterior">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="inputs.deudasPersFisicaExte" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Patrimonio neto periodo fiscal anterior">
        <el-input-number  controls-position="right" class="inputnumberclass" v-model="inputs.patrimonioNetoFiscAnterio" :precision="2" :step="0.1"
          :min="0" />
      </el-form-item>
    </el-form>
  </el-card>
</template> 

<script>
export default {
  name: 'TiempoImpuestosModalDatosDelPeriodo',

  data() {
    return {
      inputs:{
        inmuebles:'0',
        autoEmbarcaAero:'0',
        capAfecyotras:'0',
        ctaCteyCajaA:'0',
        inversionesE:'0',
        restBienesPais:'0',
        bienesExte:'0',
        deudasPersFisica:'0',
        otrasDeudasPais:'0',
        deudasPersFisicaExte:'0',
        patrimonioNetoFiscAnterio:'0',
      },
      options: [{
        value: 'Socio1--12-34567899-8',
        label: 'Socio1--12-34567899-8'
      }, {
        value: 'Socio2--12-34567899-8',
        label: 'Socio2--12-34567899-8'
      }, {
        value: 'Socio3--12-34567899-8',
        label: 'Socio3--12-34567899-8'
      }, {
        value: 'Socio4--12-34567899-8',
        label: 'Socio4--12-34567899-8'
      }, {
        value: 'Socio5--12-34567899-8',
        label: 'Socio5--12-34567899-8'
      }],
      labelPosition: 'right',
      value: ''
    }
  }
}
</script>
<style scoped>
.modaldatosperiododivisor {
  margin-bottom: 1%;
  width: 600px;
}
.el-card{
  width: 600px;
}
.inputnumberclass{
  border:solid 1.5px  #C0C0C0;
  background-color: #C0C0C0;
}

.selectcoloragugsto{
  border:solid 1.5px  #C0C0C0;
  background-color: #C0C0C0;
}
</style>
