<template>
  <div class="Header">
    <table>
      <tr>
        <td><img alt="Vue logo" src="../assets/logo.png" /></td>
        <td>topico 1</td>
        <td>Tópico 2</td>
        <td>Tópico 3</td>
        <td>Tópico 4</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Header {
  border: 1px solid;
  border-color: black;
  margin: 5px;
}

img {
  height: 30px;
}
</style>
