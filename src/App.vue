<template>
<div>
  <input v-model="forms.name" placeholder="Name">
  <input v-model="forms.surename" placeholder="Surename">
  <input v-model="forms.address" placeholder="Address">
  <input v-model="forms.phone" placeholder="Phone">
  <input v-model="forms.email" placeholder="Email">
  <input v-model="forms.born" placeholder="Born">
  Driving License
  <input type="radio" id="yes" value="Yes" v-model="forms.drivingLicense">
  <label for="yes">Yes</label>
  <input type="radio" id="no" value="No" v-model="forms.drivingLicense">
  <label for="no">No</label>


  <p> <br>
      Name:{{ forms.name }}<br>
      Surename:{{ forms.surename }}<br>
      Address:{{ forms.address }}<br>
      Phone:{{ forms.phone }}<br>
      Email:{{ forms.email }}<br>
      Born:{{ forms.born }}<br> 
      Driving License: {{ forms.drivingLicense }}
  </p>
</div>

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      forms: [
         {
            'name' : '',
            'surename' : '',
            'address' : '',
            'phone' : '',
            'email' : '',
            'born' : '',
            'drivingLicense' : true,
          }
      ]
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
