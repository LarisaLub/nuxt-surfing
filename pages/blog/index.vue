<template>
    <section>
         <h1>{{pageTitle}}</h1>
        <!-- <h4>Posts:</h4>  -->
        <ul>
            <li v-for="post of posts" :key="post.id">
                <a href="#" @click.prevent="openPost(post)"> {{`${post.id}. ${post.title}`}} </a>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
    async fetch({store}) {
        
  if (store.getters['posts/posts'].length === 0) {
      await store.dispatch('posts/fetch')
  }
    },
   
    data: () =>({
        pageTitle: 'Blog'
    }),
    computed: {
        posts() {
            return this.$store.getters['posts/posts']
        }
    },
  
    methods: {
        openPost(post) {
            this.$router.push('/blog/' + post.id)
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