<script setup>
import Mainn from "./components/Main.vue"
</script>
<template>
  <q-layout view="hhh lpR fff">

    <q-header elevated class="bg-black text-white" height-hint="98">
      <q-toolbar>
        <q-toolbar-title>
          <span class="headj">
            <q-avatar>
              <img src="./assets/uir.png">
            </q-avatar>
            <span class="judul">
              Teknik Informatika UIR SHOPPU
            </span>
          </span>
        </q-toolbar-title>
      </q-toolbar>
      <q-tabs align="left">
        <div class="bbbb">
          <div class="aaaa">
            <div class="leftbut">
              <q-btn outline style="color: goldenrod;" label="New" />
              <q-btn outline style="color: goldenrod;" label="Hot" />
              <q-btn outline style="color: goldenrod;" label="Limited" />
            </div>
          </div>
          <div class="cccc">
            <q-btn round color="primary" icon="shopping_cart" />
            <q-btn round color="secondary" icon="navigation" />
            <q-btn round color="purple" icon="my_location" />
            <q-btn color="red" icon="mail" label="Mail" />
          </div>
        </div>
      </q-tabs>


    </q-header>

    <q-page-container>
      <Mainn />
    </q-page-container>
    <div class="footer">
      <q-footer elevated class="bg-black-8 text-white blc">
        <q-toolbar>
          <q-toolbar-title>
            <div class="zzz">Copyright © 2023-2024 Muhammad Dani Nasution Inc. - All Rights Reserved.</div>
          </q-toolbar-title>
        </q-toolbar>
      </q-footer>
    </div>
  </q-layout>
</template>

<style scoped>
.blc{
  background-color: black;
}
.aaaa{
  display: flex;
  gap: 40px;

  align-items: center; 
}
.leftbut{
  margin-left: 30px;
  display: flex;
  gap: 30px;
}
.cccc {
  display: flex;
  padding-bottom: 20px;
  justify-content: space-between;
  gap: 40px;
  padding-right: 40px;
}
.bbbb{
  display: flex;justify-content: space-between;
 
  width: 100%;
}
.judul{
  font-family: "Freeman", sans-serif;
    font-weight: 400;
    font-style: normal;
}
.headj{
  display: flex;
  gap: 40px;
}
.zzz{
  position: relative;
  font-family: system-ui;
  width: 100%;
  text-align: center;
}

</style>