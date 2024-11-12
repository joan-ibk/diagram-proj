<template>
  <div class="main">
    <div class="main-in">
      <h2 id="intro">Introduce us to your team</h2>
      <div class="in-flex">
        <div class="inflex-row" v-for="(member, index) in team" :key="index">
          <img
            :src="require(`@/assets/images/${member.img}`)"
            :alt="member.name"
          />
          <div class="inflex-info">
            <h4>{{ member.name }}</h4>
            <h4 class="position"  style="color: #555">{{ member.position }}</h4>
          </div>
        </div>
      </div>
    </div>
    <div class="proj-layer">
      <div class="img">
        <img
          id="imgOne"
          :src="require('@/assets/images/img8.png')"
          alt="Description"
        />
      </div>

      <div class="info-flex">
        <h3 style="font-weight: 500">What is your team mission?</h3>
        <p style="font-weight: 400">
          Diagram is a design tools company reimagining UI design in the era of
          generative AI. We’re a small team of builders, creatives, and
          prototypers looking to grow individually and together. <br />
          <br />
          Our vision is to create radically powerful tools to improve the lives
          of UI designers and allow new people to design their digital world.
          Combining intelligent systems and tasteful execution, we think we can
          make design more fun, inclusive, and creative.
        </p>
      </div>
    </div>
    <div class="proj-layer">
      <h3 id="proj-flex">
        Share an interesting side project from a team member
      </h3>
      <img
        id="imgOne"
        :src="require('@/assets/images/img9.png')"
        alt="Description"
      />
      <p id="proj-inflex">
        Jordan and Sidd built Airport , the best place to discover new
        TestFlight apps from developers.
      </p>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      team: [
        { name: "Jordan Singer", position: "Founder & CEO", img: "img6.png" },
        {
          name: "Siddharth Sharma",
          position: "Founding Engineer",
          img: "img2.svg",
        },
        { name: "Andrew Pouliot", position: "ML Engineer", img: "img5.png" },
        {
          name: "Marco Cornacchia",
          position: "Founding Designer",
          img: "img4.png",
        },
        {
          name: "Vincent van der Meulen",
          position: "Design Engineer",
          img: "img3.png",
        },
      ],
    };
  },
};
</script>


<style scoped>
.main{
    padding: 20px;
}
#imgOne {
  width: 100%;
  height: auto;
  max-width: 630px;
  display: block;
  margin: auto;
  object-fit: cover;
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
.inflex-row {
  display: flex;
  align-items: center;
  gap: 1rem;
  flex: 1 1 calc(50% - 0.5rem);
  max-width: calc(50% - 0.5rem);
  padding: 10px;
  box-sizing: border-box;
}

.inflex-row img {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  object-fit: cover;
}

.inflex-row h4 {
  margin: 0;
  font-size: 15px;
  color: #111;
  line-height: 1.4;
  font-weight: 400;
}
.position {
  color: #555555;
}

.info-flex {
  padding: 20px;
  width: 550px;
  line-height: 25px;
  color: #111111;
  font-size: 14px;
}
#intro {
  text-align: left;
  font-size: 1.2rem;
  color: #111111;
  font-weight: 500;
  /* margin-bottom: 20px; */
  padding: 24px 0;
  max-width: 540px;
  margin: auto;
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
/* .proj-layer {
  padding: 20px;
} */

@media only screen and (max-width: 600px) {
  #intro {
    padding: 0px;
   
  }
  .in-flex {
    display: flex;
    flex-direction: column;
    /* width: 430px; */
    
  }
  .inflex-info {
    display: flex;
    flex-direction: column;
    width: 200px;
  }
  h4 {
    width: 200px;
  }
  .info-flex {
    padding: auto;
    width: 400px;
    /* margin-left: auto; */
  }
  
  #imgOne {
    width: 550px;
    /* height: 450px; */
  }
  
  .main {
    margin-left: auto;
  }
}
</style>

