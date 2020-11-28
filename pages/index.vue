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
         <div class="review-first">
            <h4 class="rev"><q class="comment-symbol"></q>recent reviews</h4>  
              <p class="rev-text">Lorem ipsum dolor sit amet, conssectetur adipising elit, sed incididunt ut labore et dolore magn.</p>
              <p class ="steve">- steve woz</p>
              <hr>
         </div>
               <q class="comment-symbol"></q>
               <div class="review-second">
                <p class="rev-text">Lorem ipsum dolor sit amet, conssectetur adipising elit, sed incididunt ut labore et dolore magn.</p>
                <p class ="steve">- david collum </p>
                <hr>
               </div>
    </div>
    <div class="col center">
       <img src="~assets/img/1.png" />
    </div>
     <div class="col"> 
       <div class="user-video">
          <p class="user-text">user videos </p>
            <img class="right-first" src="~assets/img/1_1.png" />
            <img class="right-second" src="~assets/img/1_2.png" />
       </div>
     </div>
   </div>
  
  <div class="slaider">
     <h3 class="label slaider">popular instractors</h3>
    <div class="slaider__container-slaider">
        <div class="col">
          <img class="first-foto" src="~assets/img/2_1.png" />
          <p class="name">simon adward</p>
          <p class="quantities">5,000 students</p>
       </div>
       <div class="col">
          <img class="second-foto" src="~assets/img/2.png" />
          <p class="name">elliana d'soza</p>
          <p class="quantities">4,350 students</p>
       </div>
       <div class="col">
          <img class="third-foto" src="~assets/img/3.png" />
          <p class="name">joseph bardon</p>
          <p class="quantities">3,248 students</p>
       </div>
     </div>
      <div class="nav-arrow">
        <button class="slick-prev slick-arrow" aria-label="Previous"> <svg xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 34 34" width="53%" height="53%">
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path d="M15.41 16.59L10.83 12l4.58-4.59L14 6l-6 6 6 6 1.41-1.41z" /></svg></button>
       <button class="slick-next slick-arrow" aria-label="next"><svg xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 34 34" width="53%" height="53%">
          <path d="M0 0h24v24H0V0z" fill="none" />
          <path d="M8.59 16.59L13.17 12 8.59 7.41 10 6l6 6-6 6-1.41-1.41z" /></svg></button>
    </div>
        <div class="circles"> </div>
 </div>

   <div class="wrapper">
        <h3 class="label">Recent Blogs by User</h3>
        <div class="blog-row">
          <div class="col">
            <img src="~assets/img/blog_user1.png" />
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
          <div class="col">
            <img src="~assets/img/blog_user2.png" />
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
export default {}
</script>

<style>

</style>
