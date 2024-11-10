<template>
  <div class="container">
    <div class="con-flex">
      <div class="con-image">
        <img :src="require('@/assets/images/img1.svg')" alt="Description" />
      </div>
      <div class="con-inflex">
        <h1>Diagram</h1>
        <p>Generative Creativity</p>
        <button id="shaped">diagram.com</button>
      </div>
    </div>

    <div class="con-info">
      <button><i class="fas fa-user-group"></i>5 members</button>
      <button><i class="fa-solid fa-laptop"></i>Remote</button>
      <button><i class="fa-solid fa-map-pin"></i>San Francisco, US</button>
      <button><i class="fa-solid fa-map-pin"></i>New York City, US</button>
    </div>
  </div>
</template>



<style scoped >
h1 {
  font-weight: 400;
  line-height: 26px;
  text-align: left;
  color: #111111;
  font-size: 25px;
}
p,
button {
  color: #555555;
}

.container {
  margin: 40px;
}
.con-flex {
  display: flex;
  gap: 1.5rem;
  align-items: center;
  width: Fill (540px) px;
  height: Hug (92px) px;
  padding: 0px 253.73px 0px 0px;
}
.con-inflex {
  line-height: 10px;
}
#shaped {
  border-radius: 15px;
  height: 25px;
  width: 100px;
  outline: none;
  border: none;
}
.con-info {
  margin-top: 30px;
  width: 540px;
  height: 72px;
  gap: 0px;
  opacity: 0px;
}
.con-info button {
  padding: 8px;
  border-radius: 15px;
  margin: 10px;
  background: #ffffff;
  /* outline: none; */
  border: 2px solid #eeeeee;
}

@media only screen and (max-width: 600px) {
  .con-flex {
    padding: 5px;
    width: 400px;
   
  }
  .con-info {
    /* display: flex; */
    width:500px;
    margin-left: 30px;
    padding-left: 30px;
  }
 
}
</style>