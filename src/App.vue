<script setup lang="ts">
</script>

<template>
  <header>
  </header>
  <main>
    <div class="input-group pastel-input-red">
      <input type="text" class="pastel-input" />
      <input type="submit" class="pastel-button">
      <input type="submit" class="pastel-button">
    </div>
      <!-- <input type="text" class="pastel-input pastel-input-green" />
      <input type="text" class="pastel-input pastel-input-blue" />
      <input type="text" class="pastel-input pastel-input-orange" />
      <input type="text" class="pastel-input pastel-input-pink" />
      <input type="text" class="pastel-input pastel-input-gray" />
      <input type="text" class="pastel-input pastel-input-cyan" /> -->
  </main>
</template>

<style>
#app{
  /* center */
  display: flex;
  align-items: center;
  justify-content: center;
  height: 90vh;
}



.pastel-input-default{
  --background:rgb(255, 255, 255);
  --border:#c2c2c2;
}
.pastel-input-red{
  --background:rgb(255, 200, 200);
  --border:rgb(255, 100, 100);
}
.pastel-input-green{
  --background:rgb(200, 255, 200);
  --border:rgb(100, 255, 100);
}
.pastel-input-blue{
  --background:rgb(200, 200, 255);
  --border:rgb(100, 100, 255);
}
.pastel-input-orange{
  --background:rgb(255, 229, 200);
  --border:rgb(255, 175, 100);
}
.pastel-input-pink{
  --background:rgb(255, 200, 255);
  --border:rgb(255, 100, 255);
}
.pastel-input-gray{
  --background:rgb(200, 200, 200);
  --border:rgb(100, 100, 100);
}
.pastel-input-cyan{
  --background:rgb(200, 255, 255);
  --border:rgb(100, 255, 255);
}

.pastel-button, .pastel-input{
  padding: 5px;
  padding-left: 0px;
  padding-right: 0px;
  border-radius: 3px;
  background-color:var(--background) ;
  border:2pt solid var(--border);
  font-size: 13pt;
  text-align : center;
  outline-style: none;
  
}
.pastel-button{
  cursor: pointer;
  padding-left: 10px;
  padding-right: 10px;
}
.pastel-button:hover{
  background-color:var(--border);
  color:var(--background);
}


.input-group *:first-child{
  border-right :none;
  border-radius: 3px 0 0 3px;
}

.input-group *:last-child{
  border-left :none;
  border-radius: 0 3px 3px 0;
}
.input-group *:not(:last-child,:first-child){
  border-left: none;
  border-right: none;
  border-radius: 0 0 0 0;
}
</style>
