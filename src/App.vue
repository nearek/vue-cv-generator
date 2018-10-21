<template>
<div class="wrapper">
  
 <div class="left">
  <div class="cv-tmpl-1">
   <div class="cv-values">
   <div class="full-name todo-item-left">
   <div class="todo-item-label">{{ forms.name }}</div>
   <input type="text" v-model="forms.name" placeholder="Name" class="name todo-item-edit">
    
   </div>
   <input v-model="forms.surename" placeholder="Surename" class="surename"> 

   </div>
</div>
  </div>


    <div class="right">
    test
    </div>
</div>

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      forms: [
         {
            'name' : [
              {
                'value': 'name',
                'visible': true,
                'editing': false,
              }
            ],
            'surename' : [
              {
                'value': 'surename',
                'visible': true,
                'editing': false,
              }
            ],
            'address' : [
              {
                'value': 'address',
                'visible': true,
                'editing': false,
              }
            ],
            'phone' : [
              {
                'value': 'phone',
                'visible': true,
                'editing': false,
              }
            ],
            'email' : [
              {
                'value': 'email',
                'visible': true,
                'editing': false,
              }
            ],
            'born' : [
              {
                'value': 'born',
                'visible': true,
                'editing': false,
              }
            ],
              'name' : [
              {
                'value': 'name',
                'visible': true,
                'editing': false,
              }
            ],
          }
      ]
    }
  }
}
</script>

<style>
.wrapper{
  height:100%;
  width:100%;
  display: inline-flex;
}
.left{
  width:80%;
  height: 100%;
  background: #fff;
  display: flex;
  justify-content: center;
}

.right{
   width:20%;
  height:29.7cm;
  background: #E0E0E0;
}

.cv-tmpl-1{
  height:29.7cm;
  width: 21cm;
  border: 1px solid #E0E0E0;
}

.cv-values{
  padding: 5% 9%;
}

.cv-values .full-name{
 
}
</style>
