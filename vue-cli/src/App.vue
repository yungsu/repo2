<template>
  <div>
   <!-- <app-header v-bind="프롭스속성이름"="상위컴포넌트"></app-header> -->
   <app-header v-bind:probsdata="str"
              v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
// new Vue({
//   data:{
//     str:'hi'
//   }
// })

export default {
  data: function(){
    return{
      str: 'Header'
    }
  },
  components: {
    'app-header':AppHeader
  },
  methods: {
    renewStr: function(){
      this.str = 'hi';
    }
  }
}
</script>

<style>

</style>