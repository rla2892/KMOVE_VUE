<script>
import TextBind from './components/TextBind.vue';
export default {
    components : {
        // TextBind : TextBind // key, value 같아서 1개로 줄여도 됨
        TextBind
    },
    data() {
        return {
            isActive: false,
            user: {
                name: "ejerjjr",
                age: 30
            }
        }
    }
}
</script>

<template>
    <h2 v-if="isActive">hello World</h2>
    <h2 v-if="!isActive">good bye World</h2>
    <h2 v-if="isActive">123</h2>
    <h2 v-else>456</h2>

    <h2 v-if="user.age > 20">Adult {{user.name}}</h2>
    <h2 v-else-if="user.age > 10">Teenager {{user.name}}</h2>
    <h2 v-else>Child {{user.name}}</h2>

    <input type="text" v-model="user.age">
    <h3>{{user.age}}</h3>
</template>


<style >

</style>
