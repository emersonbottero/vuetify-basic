<template>
  <p @click="sayHello">hello times: {{ helloTimes }}</p>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
@Component({})
export default class Hello extends Vue {
  helloTimes = 0
  sayHello() {
      this.helloTimes++  
  }

  mounted() {
    console.log('hello from hello');
  }
}
</script>
