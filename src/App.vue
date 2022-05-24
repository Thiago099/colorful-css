<script setup lang="ts">
import './colors.css'
import './inputs.css'
import './table.css'
const colors = [
  'black',
  'red',
  'orange',
  'pink',
  'green',
  'cyan',
  'blue',
  'purple',
];
</script>

<template>
  <header>
  </header>
  <main>
    <div >
      <div :class="`input-container pastel-${color}`" v-for="color in colors" :key="color"    >
        <input type="text" class="pastel-input" />
        <input type="submit" class="pastel-button">
      </div>
    </div>
    <br>
    <table :class="`pastel-table pastel-${color}`" v-for="color in colors" :key="color">
      <tr>
        <th>Company</th>
        <th>Contact</th>
        <th>Country</th>
      </tr>
      <tr>
        <td>Alfreds Futterkiste</td>
        <td>Maria Anders</td>
        <td>Germany</td>
      </tr>
      <tr>
        <td>Centro comercial Moctezuma</td>
        <td>Francisco Chang</td>
        <td>Mexico</td>
      </tr>
      <tr>
        <td>Ernst Handel</td>
        <td>Roland Mendel</td>
        <td>Austria</td>
      </tr>
      <tr>
        <td>Island Trading</td>
        <td>Helen Bennett</td>
        <td>UK</td>
      </tr>
      <tr>
        <td>Laughing Bacchus Winecellars</td>
        <td>Yoshi Tannamuri</td>
        <td>Canada</td>
      </tr>
      <tr>
        <td>Magazzini Alimentari Riuniti</td>
        <td>Giovanni Rovelli</td>
        <td>Italy</td>
      </tr>
    </table>
  </main>
</template>

<style>
.input-container{
    margin:5px;
    width: 437px;
}
.pastel-table{
    margin:5px;
    display: inline-block;
}
</style>
