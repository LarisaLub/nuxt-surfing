<template>
    <section>
        <h4> №: {{post.id}}</h4> 
        <hr>
        <h1>{{post.title}} </h1>
        
        <h3>{{post.body}}</h3>
        

       <li> 
            <a href="/blog">Blog</a>

        </li>
    </section>
</template>

<script>
export default {
    validate({params}) {
        return /^\d+$/.test(params.id)
    },
    async asyncData({$axios, params}) {
        const post = await $axios.$get('http://jsonplaceholder.typicode.com/posts' + params.id)
        return {post}
    },
    layout: 'empty'
}
</script>

















  <!-- <h1> Post{{$route.params.id}} </h1> -->
         <!-- <img class="foto" src="~assets/img/2_1.png" /> -->



<style scoped>

h1{
    color: rgb(51, 51, 224);
    font-size: 24px;
    padding-top: 15px ;
    padding-bottom: 15px;
    padding-left: 520px;
}
.foto {
   padding-left: 387px;  
}

</style>