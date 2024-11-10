<template>
  <div class="container">
    <h2 id="intro">Introduce us to your team</h2>
    <div class="in-flex">
      <div class="inflex-row">
        <img :src="require('@/assets/images/img6.png')" alt="Description" />
        <div class="inflex-info">
          <h4>Jordan Singer</h4>
          <h4 style="color: #555555">Founder & CEO</h4>
        </div>
      </div>
      <div class="inflex-row">
        <img :src="require('@/assets/images/img2.svg')" alt="Description" />
        <div class="inflex-info">
          <h4>Siddharth Sharma</h4>
          <h4 style="color: #555555">Founding Engineer</h4>
        </div>
      </div>
      <div class="inflex-row">
        <img :src="require('@/assets/images/img5.png')" alt="Description" />
        <div class="inflex-info">
          <h4>Andrew Pouliot</h4>
          <h4 style="color: #555555">ML Engineer</h4>
        </div>
      </div>
      <div class="inflex-row">
        <img :src="require('@/assets/images/img4.png')" alt="Description" />
        <div class="inflex-info">
          <h4>marco cornacchia</h4>
          <h4 style="color: #555555">Founding Designer</h4>
        </div>
      </div>
      <div class="inflex-row">
        <img :src="require('@/assets/images/img3.png')" alt="Description" />
        <div class="inflex-info">
          <h4>Vincent van der Meulen</h4>
          <h4 style="color: #555555">Design Engineer</h4>
        </div>
      </div>
    </div>
    <div class="img">
      <img
        id="imgOne"
        :src="require('@/assets/images/imageSticker-2d.png')"
        alt="Description"
      />
    </div>

    <div class="info-flex">
      <h3 style="font-weight: 500;">What is your team mission?</h3>
      <p style="font-weight: 400;">
        Diagram is a design tools company reimagining UI design in the era of
        generative AI. We’re a small team of builders, creatives, and
        prototypers looking to grow individually and together. <br />
        <br />
        Our vision is to create radically powerful tools to improve the lives of
        UI designers and allow new people to design their digital world.
        Combining intelligent systems and tasteful execution, we think we can
        make design more fun, inclusive, and creative.
      </p>
    </div>
    <div class="proj-layer">
      <h3 id="proj-flex">
        Share an interesting side project from a team member
      </h3>
      <img
        id="imgOne"
        :src="require('@/assets/images/imageSticker.png.png')"
        alt="Description"
      />
      <p id="proj-inflex">
        Jordan and Sidd built Airport , the best place to discover new
        TestFlight apps from developers.
      </p>
    </div>
  </div>
</template>





<style scoped>
#imgOne {
  width: 630px;
  height: 472.5px;
  gap: 0px;
  opacity: 0px;
}

.in-flex {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: space-between;
  padding: 24px 0;
  max-width: 540px;
  margin: auto;
}

.in-flex .inflex-row {
  display: flex;
  /* flex-direction: column; */
  align-items: center; /* Align items vertically in the center */
  gap: 1rem; /* Space between image and text */
  flex: 1 1 calc(50% - 0.5rem); /* Allows two items per row */
  max-width: calc(50% - 0.5rem);
  padding: 10px;
  box-sizing: border-box;
}

.inflex-row img {
  width: 60px; /* Adjust image size */
  height: 60px;
  border-radius: 50%; /* Circular image */
  object-fit: cover;
}

.inflex-row h4 {
  margin: 0;
  font-size: 15px;
  color: #111;
  line-height: 1.4;
  font-weight: 400;
}

.info-flex {
  padding: 20px;
  width: 550px;
  line-height: 25px;
  color: #111111;
  font-size: 14px;
}
#intro {
  width: Fill (540px) px;
  height: Hug (25.6px) px;
  padding: 0px 250px 0px 0px;
  color: #111111;
  font-size: 20px;
  font-weight: 500;
  line-height: 25.6px;
}
#proj-flex {
  margin-left: 40px;
  color: #111111;
  font-weight: 500;
  font-size: 16px;
}
#proj-inflex {
  width: 500px;
  margin-left: 40px;
  color: #111111;
  font-size: 14px;
  font-weight: 400;
}

@media only screen and (max-width: 600px){
    #intro{
        padding: 0px;
        width: 400px;
    }
    .in-flex{
        display: flex;
        flex-direction: column;
        width: 430px;
        margin: 0px;
    }
    .inflex-info{
        display: flex;
        flex-direction: column;
        width: 200px;
    }
    h4{
        width: 200px;
    }
    .info-flex{
        padding: 10px;
        width: 400px;
    }
    .proj-layer{
        margin-left:50px;
    }
    #imgOne{
        width: 550px;
        height: 450px;
    }
    img{
        background-image: cover;
    }
}

</style>