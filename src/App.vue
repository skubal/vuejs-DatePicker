<template>
  <div id="app">
    DatePicker Sample
	<date-picker v-model="value1" lang="en" :not-before="new Date('08/10/2018')" :not-after="new Date('08/20/2018')"></date-picker>
	<br/><br/><br/>
	Month View:
	<date-picker v-model="value2" lang="en" type="month" format="YYYY-MM"></date-picker>
  </div>
</template>

<script>
import DatePicker from 'vue2-datepicker'

export default {
  name: 'App',
  components: {
	'date-picker': DatePicker
  },
  data: function() {
	 return  {
           value1: '',
		   value2: ''
         }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
