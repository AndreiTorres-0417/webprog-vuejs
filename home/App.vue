<template>
  <h2>Example v-bind Directive</h2>
  <p>The v-bind directive connects the style attribute of the DIV element to the 'colorVal' data property.</p>
  <div v-bind:style="{ backgroundColor: colorVal }">DIV element</div>
  <p>Use the input type="color" box below to change the color.</p>
  <p><input type="color" v-model="colorVal"> <pre>colorVal: '{{ colorVal }}'</pre></p>
</template>

<script>
export default {
  data() {
    return {
      colorVal: 'lightgreen'
    };
  }
};
</script>

<style scoped>
div {
  border: solid black 1px;
  width: 150px;
  height: 150px;
  padding: 10px;
  margin: 10px;
}
pre {
  display: inline;
}
</style>   
