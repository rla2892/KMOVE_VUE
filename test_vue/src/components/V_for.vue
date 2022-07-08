<script>
import TextBind from './components/TextBind.vue';
export default {
    components : {
        // TextBind : TextBind // key, value 같아서 1개로 줄여도 됨
        TextBind
    },
    data() {
        return {
            fruits: ["apple", "banana", "orange"],
            cities: [
                {name: 'new york', population: 200},
                {name: 'pusan', population: 300},
                {name: 'london', population: 320},
            ],
            user: {
                name: 'dsfsf',
                age: 21,
                city: 'Seoul'
            }
        }
    }
}
</script>

<template>
    <ul >
        <li v-for="(fruit, index) in fruits" :key="index">
            {{fruit}}, {{index}}
        </li>
        <template v-for="(fruit, index) in fruits" :key="index">
            {{fruit}}, {{index}}
        </template>
    </ul>
    <ul>
        <template v-for="(value, key, index) in user" :key="index">
            <li>{{value}} / {{key}} / {{index}}</li>
        </template>
    </ul>
</template>


<style >

</style>
