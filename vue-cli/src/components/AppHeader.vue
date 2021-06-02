<template>
  <header>
      {{ probsdata}}
      <button v-on:click="sendEvent">send</button>
  </header>
</template>

<script>
export default {
    props: ['probsdata'],
    methods:{
        sendEvent: function(){
            this.$emit('renew');
        }
    }
}
</script>

<style>

</style>