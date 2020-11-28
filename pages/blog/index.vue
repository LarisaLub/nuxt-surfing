<template>
    <section>
        <h1>Blog</h1>
        <p> Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        <img src=""/>
        <ul>
            <li v-for="post of 5" :key="post">
                <a href="#" @click.prevent="openPost(post)"> Post {{post}} </a>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
    methods: {
        openPost(post) {
            this.$router.push('/blog/'+post)
        }
    },
    layout: 'empty'
}
</script>

<style scoped>

h1{
    color: rgb(51, 51, 224);
    font-size: 54px;
    padding-top: 50px ;
    padding-bottom: 30px;
    padding-left: 120px;
}

p{
    color: rgb(27, 27, 114);
     padding-right: 50px;
     font-size: 24px;
}

li{
    padding-top: 20px;
    padding-left: 145px;
    list-style: none;
    font-family: helvetica, arial, sans-serif;
    font-size: 15px;
    color: rgb(3, 7, 44);
    font-size: 25px;
}

</style>