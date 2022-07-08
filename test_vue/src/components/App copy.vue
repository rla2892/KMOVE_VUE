<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
// import HelloWorld from './components/HelloWorld.vue'
console.log('test');
export default {
  data() {
    return {
      name: "This is test",
      user:{
        name: "Hello ~~~",
        age: 31
      },
      fruits: ["apple","banana","cherry"],
      button_html: '<button>v-html</button>',
      button_hack: `<button onclick="document.body.style='background-color:blue;'">css hack</button>`,
    }
  }
}
</script>

<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" /> -->
  <HelloWorld msg="test" />
  <div>sang jin</div>
  <div>{{name}}</div>
  <div>{{user.name}}</div>
  <div>{{fruits[2]}}</div>
  <div v-text="name"></div>
  <div v-html="button_html"></div>
  <div v-html="button_hack"></div>
</template>

<style scoped>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
div {
  margin: 1rem;
  border: 0.2rem solid black;
}
</style>
