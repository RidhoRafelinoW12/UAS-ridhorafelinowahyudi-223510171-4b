<template>
  <div class="q-pa-md" style="background-image: url('@/assets/pp2.jpg');">
    <q-page>
      <q-list bordered padding>
        <q-item clickable v-ripple @click="goToTask(1)">Sa pu Tugas 1 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(2)">Sa pu Tugas 2 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(3)">Sa pu Tugas 3 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(4)">Sa pu Tugas 4 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(5)">Sa pu Tugas 5 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(6)">Sa pu Tugas 6 Ridho</q-item>
        <q-item clickable v-ripple @click="goToTask(7)">Sa pu Tugas 7 Ridho</q-item>
      </q-list>
    </q-page>
  </div>
</template>

<script>
export default {
  methods: {
    goToTask(taskNumber) {
      const taskLinks = {
        1: "https://ridho-project-cv.vercel.app/", 
        2: "https://223510171-ridhorafelinow-tugas2-prak-pbk.vercel.app/", 
        3: "https://223510171-ridhorafelinow-tugas3-prak.vercel.app/", 
        4: "https://tugas4-ridho-rafelino-wahyudi-223510171-4b.vercel.app/", 
        5: "https://avocadostore09-ridho-rafelino-wahyudi-223510171-4b.vercel.app/", 
        6: "https://tugas6-ridho-rafelino-wahyudi-223510171-4b.vercel.app/", 
        7: "https://tugas7-ridho-rafelino-wahyudi-223510171-4b.vercel.app/" 
      };
      window.location.href = taskLinks[taskNumber];
    }
  }
}
</script>

<style scoped>
.q-pa-md {
  padding: 16px;
  background-size: cover;
  background-position: center;
  background-image: url('@/assets/pp3.jpeg');
}

.q-list {
  max-width: 400px;
  margin: 0 auto;
}

.q-item {
  padding: 8px 10px;
  border-radius: 5px;
  background-color: #FFC0CB; /* Light background color */
  margin-bottom: 8px;
  cursor: pointer;
}

</style>
