<template>
  <div class="home"> 
    <h2 class="inscript"> 
      long  beach  surfing  institute
    </h2>
    <p class="descript">
      Lorem ipsum dolor sit amet, consectetur adipicing elit, sed do eiusmod tempor 
       incididunt ut labore et dolare magna alique. Ut enim ad minim veniam.
    </p>
    <div class="box">
      <div class="col">
        <div class="reviews">
          <h4 class="rev">recent reviews</h4>  
          <div class="review">
              <p class="rev-text">
                <q class="comment-symbol"></q>
                Lorem ipsum dolor sit amet, conssectetur adipising elit, sed incididunt ut labore et dolore magn.
              </p>
              <p class ="steve">- steve woz</p>
              <hr>
          </div>
          <div class="review">
            <p class="rev-text">
              <q class="comment-symbol"></q>
              Lorem ipsum dolor sit amet, conssectetur adipising elit, sed incididunt ut labore et dolore magn.
            </p>
            <p class ="steve">- david collum </p>
            <hr class="mini-line">
          </div>
        </div>
    </div>
    <div class="col center">
       <img class="photo-center" src="~assets/img/1.png" />
    </div>
     <div class="col"> 
       <div class="user-video">
          <p class="user-text">user videos </p>
            <img class="right" src="~assets/img/1_1.png" />
            <img class="right second-photo" src="~assets/img/1_2.png" />
       </div>
     </div>
    </div>
  
  <div class="slaider">
     <h3 class="label slaider">popular instractors</h3>
    <div class="slaider__container-slaider">
        <carousel :autoplay="false" :dots="true" 
        :responsive="{0:{items:1,nav:false},480:{items:1,nav:true}, 768: {items:2}, 1024: {items: 3}}" >
        <div class="wrapper-slide">
          <img class="first-foto" src="~assets/img/2_1.png" />
          <p class="name">simon adward</p>
          <p class="quantities">5,000 students</p>
       </div>
       <div class="wrapper-slide">
          <img class="second-foto" src="~assets/img/2.png" />
          <p class="name">elliana d'soza</p>
          <p class="quantities">4,350 students</p>
       </div>
       <div class="wrapper-slide">
          <img class="third-foto" src="~assets/img/3.png" />
          <p class="name">joseph bardon</p>
          <p class="quantities">3,248 students</p>
       </div>
         <div class="wrapper-slide">
          <img class="first-foto" src="~assets/img/2_1.png" />
          <p class="name">simon adward</p>
          <p class="quantities">5,000 students</p>
       </div>
       <div class="wrapper-slide">
          <img class="second-foto" src="~assets/img/2.png" />
          <p class="name">elliana d'soza</p>
          <p class="quantities">4,350 students</p>
       </div>
       <div class="wrapper-slide">
          <img class="third-foto" src="~assets/img/3.png" />
          <p class="name">joseph bardon</p>
          <p class="quantities">3,248 students</p>
       </div>
         <div class="wrapper-slide">
          <img class="first-foto" src="~assets/img/2_1.png" />
          <p class="name">simon adward</p>
          <p class="quantities">5,000 students</p>
       </div>
      <div class="wrapper-slide">
          <img class="second-foto" src="~assets/img/2.png" />
          <p class="name">elliana d'soza</p>
          <p class="quantities">4,350 students</p>
       </div>
       <div class="wrapper-slide">
          <img class="third-foto" src="~assets/img/3.png" />
          <p class="name">joseph bardon</p>
          <p class="quantities">3,248 students</p>
       </div>
        </carousel >
    </div>
    </div>
     <div class="wrapper">
      <h3 class="label">Recent Blogs by User</h3>
        <div class="blog-row">
          <div class="col">
            <img class="photo-blog" src="~assets/img/blog_user1.png" />
          </div>
          <div class="col right-discription">
            <h3 class="title">Lipsum cound be headline</h3>
            <p class="discription">Lorem ipsum dolor sit amet, consectetur adipicing elit, sed do eiusmod tempor 
            incididunt ut labore et dolare magna alique. Ut enim ad minim veniam.</p>
            <button class="snap">Read More</button>
          </div>
        </div>
        <div class="blog-row revers">
          <div class="col">
            <h3 class="title">Lipsum cound be headline</h3>
            <p class="discription">Lorem ipsum dolor sit amet, consectetur adipicing elit, sed do eiusmod tempor 
            incididunt ut labore et dolare magna alique. Ut enim ad minim veniam.</p>
            <button class="snap">Read More</button>
          </div>
          <div class="col left">
            <img class= "photo-blog" src="~assets/img/blog_user2.png" />
          </div>
        </div>
      </div>
      <section class="enroll">
        <h3 class="label interes">Aren't you intrested Yet!!</h3>
        <div class="enroll-button" >
        <button class="snap entr">enroll now</button>
        </div>
      </section>
  </div>
</template>


<script>
</script>

<style>

</style>
