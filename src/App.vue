<script setup lang="ts">
import './css/colors.css'
import './css/inputs.css'
import './css/table.css'
import './css/card.css'
import './css/nav.css'
import './css/content.css'
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
      <div class="row">
        <div :class="`col-3 pastel-${color}`" v-for="color in colors" :key="color" >
          <label for="a" class="input-label">Label:</label>
          <div class="input-container">
            <input type="text" class="pastel-input" />
            <input type="submit" class="pastel-button">
          </div>
        </div>
      <table :class="`col-3 pastel-table pastel-${color}`" v-for="color in colors" :key="color">
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
    <div :class="`col-3 card pastel-${color}`" v-for="color in colors" :key="color">
      <div class="card-header">Title</div>
      <div class="card-body">Content</div>
    </div>
    <div :class="`col-3 nav pastel-${color}`" v-for="color in colors" :key="color">
      <div class="nav-item nav-selected">Home</div>
      <div class="nav-item">About</div>
      <div class="nav-item">Contact</div>
    </div>
    </div>
  </main>
</template>

<style>




</style>
