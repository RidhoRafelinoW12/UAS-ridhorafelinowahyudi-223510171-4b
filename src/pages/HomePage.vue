<template>
    <q-layout view="hHh lpR fFf">
      <q-header elevated class="bg-primary text-white" height-hint="98">
        <q-toolbar>
          <q-toolbar-title>
            <q-avatar>
              <img src="@/assets/pp1.jpg" alt="Profile Picture">
            </q-avatar>
            Ujian Akhir Semester Matkul PraktikumPBK
          </q-toolbar-title>
        </q-toolbar>
  
        <q-tabs align="left">
          <q-route-tab to="/tasks" label="Lubuak Tugas Ridho Rafel" />
        </q-tabs>
      </q-header>
  
      <q-page-container>
        <WeatherPage />
        <router-view />
      </q-page-container>
    </q-layout>
  </template>
  
  <script>
  import WeatherPage from '../pages/WeatherPage.vue'
  
  export default {
    components: {
      WeatherPage
    }
  }
  </script>
  <style lang="scss">
  .bg-primary {
    background-color: #FFC0CB !important; /* warna pink */
  }
  
  .text-white {
    color: #fff !important; /* warna putih */
  }
  
  .q-toolbar {
    padding: 0.5rem;
  }
  
  .q-toolbar-title {
    font-size: 1.5rem;
    font-weight: bold;
  }
  
  .q-route-tab {
    font-size: 1.2rem;
    font-weight: bold;
  }
  
  .q-page-container {
    padding: 1rem;
  }
  
  .weather-page {
    padding: 2rem;
    border: 1px solid #ccc;
    border-radius: 0.5rem;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
</style>