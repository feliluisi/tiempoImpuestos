<template>
  <el-card>
    <el-select v-model="value" placeholder="Socio--CUIT">
      <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value">
      </el-option>
    </el-select>
    <el-form class="elcardFiscalAnterior">
      <el-form-item class="modaldatosperiododivisor" label="Inmuebles">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1"/>
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Automotores, embarciones y aeronaves">
        <el-input-number class="inputnumberclass" controls-position="right" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Cap. afec. a 3ª y 4ª cat. y otras p.s.">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Cta. cte. y caja de ahorro">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Inversiones en entidades financieras">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Resto de bienes en el pais">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Bienes en el exterior">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Deudas con personas fisicas">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Otras deudas en el pais">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Deudas con personas fisicas del exter.">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Otras deudas en el exterior">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
      <el-form-item class="modaldatosperiododivisor" label="Patrimonio neto periodo fiscal anterior">
        <el-input-number controls-position="right" class="inputnumberclass" v-model="bienes" :precision="2" :step="0.1" :min="1" />
      </el-form-item>
    </el-form>
  </el-card>
</template> 

<script>
export default {
  name: 'TiempoImpuestosModalDatosDelPeriodo',

  data() {
    return {
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
      value: ''
    }
  }
}
</script>
<style scoped>
.elcardFiscalAnterior {
  margin-bottom: 1%;
  justify-content: right;
  margin-top: 1%;

}
.inputnumberclass{ 
  width: 15rem;
  justify-content: right;

}

.el-card {
  width: 600px;
  justify-content: right;
}

.modaldatosperiododivisor {
  margin-bottom: 1%;
  justify-content: right;
 

}

</style>
