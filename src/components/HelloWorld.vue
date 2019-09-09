<template>
  <div class="hello">
    <table id="LinhaTempo"> 
      <tr>
        <th style="width:40%">Pacientes</th>
        <th style="width:15%">Recepcionado</th>
        <th style="width:15%">Em andamento</th>
        <th style="width:15%">Sala de Recuperação</th>
        <th style="width:15%">Alta</th>
      </tr>
      <tr>
        <td>H068494 - Rebeca Almeida</td>
        <td><button class="button buttonOn"></button></td>
        <td><button class="button buttonOff"></button></td>
        <td><button class="button buttonOff"></button></td>
        <td><button class="button buttonOff"></button></td>
      </tr>
      <tr>
        <td>H037983 - Ana Maria Albuquerque</td>
        <td><button class="button buttonOn"></button></td>
        <td><button class="button buttonOn"></button></td>
        <td><button class="button buttonOff"></button></td>
        <td><button class="button buttonOff"></button></td>
      </tr>
      <tr>
        <td>H023484 - Antonio dos Santos</td>
        <td><button class="button buttonOn c1"></button></td>
        <td><button class="button buttonOn c2"></button></td>
        <td><button class="button buttonOff c3"></button></td>
        <td><button class="button buttonOff c4"></button></td>
      </tr>
  </table>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

#LinhaTempo {
  border: 1px solid black;
  border-collapse: collapse;
}

#LinhaTempo td, #LinhaTempo th {
  border-bottom: 1px solid #ddd;
  padding: 8px;
  font-size: 20px;
}

#LinhaTempo tr:nth-child(even){background-color: #f2f2f2;}

#LinhaTempo tr:hover {background-color: #ddd;}

#LinhaTempo th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: center;
  background-color: #4CAF50;
  color: white;
  font-weight: bold;
}

.button {
  background-color: #4CAF50;
  border: none;
  padding: 10px;
  display: inline-block;
  margin: 4px 2px;
  cursor: pointer;
}

.buttonOn {
  border-radius: 50px;
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
}

.buttonOff {
  border-radius: 50px;
  background-color:rgb(240, 238, 238);
  border: 1px solid #e7e7e7;
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
}

.c1 {
  background-color:yellow;
}

.c2 {
  background-color:blue;
}

.c3 {
  background-color:black;
}

.c4 {
  background-color:red;
}

</style>
