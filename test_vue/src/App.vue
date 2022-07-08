<script>
export default {
    methods: {
        sayHello(){
            return "hello hello";
        }
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
    <h2>{{sayHello()}}</h2>
</template>


<style >

</style>
