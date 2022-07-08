<script>
import TextBind from './components/TextBind.vue';
export default {
    components : {
        // TextBind : TextBind // key, value 같아서 1개로 줄여도 됨
        TextBind
    },
    data() {
        return {
            // bind_url: "http://www.google.com",
            bind_url: "http://www.daum.net",
            bind_a: {
                bind_url: "http://www.google.com",
                domain_name: "google"
            },
            img :{
                size_x: 100,
                size_y: 100,
                url: `https://placeimg.com/100/100/animals`
            }
        }
    }
}
</script>

<template>
    <!-- <TextBind /> -->
    <h2 id="title">Hello World</h2>
    <a v-bind:href="bind_a.bind_url">{{bind_a.domain_name}}</a>
    <img v-bind:src="img.url" alt="">
</template>

<style scoped>
#title {
    color:blueviolet;
    text-align: center;

}

</style>
