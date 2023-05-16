<script setup lang="ts">
</script>

<template>
  <main>
    <div>

      <div style="display: flex;">
        <p class="name" style="">guilherme@moog:~$</p>
        <input style="caret-color:chartreuse;"  type="text" name="" id="" @keypress="">
        
      </div>

    </div>
  </main>
</template>


<script>
  import { onMounted } from 'vue';
  export default {
    components: {
     
    },
    data() {
      return {
        
      };
    },
    watch: {
      banco(newValue) {
      }
    },
    setup() {
      onMounted(() => {

      })
    }
  }
</script>

<style>

  .name {
    color:chartreuse; 
    font-family:Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    margin-right: 0.5rem;
  }

</style>