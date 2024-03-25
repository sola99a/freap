<template>
  <div>
<button @click="get(32)">get</button>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  setup () {
    function get(e){
      console.log(e);
axios.post('https://sollio.freehostia.com/freap/',e).then((res)=>{
console.log(res.data);
}).catch((er)=>{
console.log(er);
})
    }

    return {get}
  }
}
</script>

<style lang="scss" scoped>

</style>
