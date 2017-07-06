<template>
  <div>
   <button @click="currentComponent = 'app-blue'">Blue</button>
   <button @click="currentComponent = 'app-green'">Green</button>
   <button @click="currentComponent = 'app-red'">Red</button>
   <hr>
   <keep-alive>
     <component :is="currentComponent"></component>
   </keep-alive>
    
  </div>
</template>

<script>

import Blue from './components/Blue.vue';
import Green from './components/Green.vue';
import Red from './components/Red.vue';

export default {
  data () {
    return {
      currentComponent: 'app-blue'
    }
  },
  components: {
    'app-blue': Blue,
    'app-green': Green,
    'app-red': Red
  }
}
</script>

<style>
div{
  width: 400px;
  margin: auto;
}
</style>
