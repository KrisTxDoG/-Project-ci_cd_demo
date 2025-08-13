<template>
  <div style="font-family: Arial, Helvetica, sans-serif; padding: 2rem;">
    <h1>KristTest X TTT 成功? CI/CD Demo — Frontend</h1>
    <p>This is a minimal Vue 3 app for the CI/CD demo.</p>
    <p>Backend API message: <strong id="msg">-</strong></p>
    <button @click="callApi">Call Backend</button>
  </div>
</template>

<script>
export default {
  methods: {
    async callApi() {
      try {
        const res = await fetch('http://localhost:3000/');
        const json = await res.json();
        document.getElementById('msg').innerText = json.message;
      } catch (e) {
        document.getElementById('msg').innerText = 'Error: ' + e.message;
      }
    }
  }
}
</script>
