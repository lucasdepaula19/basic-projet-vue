<template>
  <div class="Menu">
    <table align="center">
      <tr>
        <td>menu 1</td>
        <td>menu 2</td>
        <td>menu 3</td>
        <td>menu 4</td>
      </tr>
    </table>
</div>
</template>

<script>
export default {
  name: 'Menu',
  props: {
    // insira aqui as propriedades
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.Menu{
  border: 1px solid;
  border-color: black;
  margin: 5px;
  
}

td {
  padding-left: 1em;
  padding-right: 1em;
}
</style>
