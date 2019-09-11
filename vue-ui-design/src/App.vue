<template>
  <div id="app">
    <zippy>
   <p slot="zippy-heading">This is the heading</p>
     <p slot="zippy-content">This is the demo only You can use this component in any component, just use the zippy tag and you are blahhhhhhhhhhhh............</p>
    </zippy>
  </div>
</template>

<script>
import zippy from './components/zippy';
export default {
  name: 'app',
  components: {
    zippy
  },
 
}
</script>

<style scoped>

</style>


