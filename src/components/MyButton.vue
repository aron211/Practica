<template>
  <div class="btn">
    
    <button id="btn" @click="incrementCont">{{name}} {{contador}}</button>
  </div>
</template>

<script>
export default {
  name: 'MyButton', 
  props: {
   name: String,
   contador: Number
  }
}
</script>
