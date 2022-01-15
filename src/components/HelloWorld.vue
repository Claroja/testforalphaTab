<template>
<div id="alphaTab" data-tex="true">
  \title "Hello alphaTab"
  .
  :4 0.6 1.6 3.6 0.5 2.5 3.5 0.4 2.4 |
    3.4 0.3 2.3 0.2 1.2 3.2 0.1 1.1 |
    3.1.1
</div>
<button @click="test">test</button>
</template>

<script lang='js'>
import { defineComponent, reactive, ref, toRefs } from 'vue'
import {AlphaTabApi} from "@coderline/alphatab"
export default defineComponent({
  name: 'HelloWorld',
  setup(){
    function test(){
      const element = document.getElementById('alphaTab');
      const api = new AlphaTabApi(element);
    }
    return{
      test
    }
  }

})
</script>
