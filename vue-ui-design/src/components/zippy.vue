<template>
  <div class="zippy-container">
    <button class="accordion"  v-on:click="display= !display">
        <slot name="zippy-heading"></slot>
    </button>
    <div class="panel" v-show="display">
        <slot name="zippy-content"></slot>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'zippy',
  data(){
      return{
          display: false
      }
  },
    methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.accordion {
  background-color: #eee;
  color: #444;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  transition: 0.4s;
}

.active, .accordion:hover {
  background-color: #ccc; 
}

.panel {
  padding: 0 18px;
  background-color: whitesmoke;
  overflow: hidden;
}
</style>
