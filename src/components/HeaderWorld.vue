<template>
  <div class="header">
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

<style scoped>
/* General Styles */
.header {
  padding: 20px;
 
}

img {
  width: 92px;
  height: 92px;
  object-fit: cover;
}

h1 {
  font-weight: 400;
  line-height: 26px;
  color: #111111;
  font-size: 1.6rem;
}

p,
button {
  color: #555555;
}

.con-flex {
  display: flex;
  gap:1.2rem; /* Reduced gap to bring items closer */
  align-items: center;
  max-width: 100%;
  padding: 0; /* Ensure no extra padding */
  margin: 0; /* Ensure no extra margin */
}

.con-inflex {
  display: flex;
  flex-direction: column;
  line-height: 2; /* Adjust line-height to reduce spacing between text lines */
}

h1 {
  font-weight: 400;
  font-size: 1.6rem;
  margin: 0; /* Remove default margin */
  line-height: 1.2; /* Adjust to reduce spacing */
}

p {
  margin: 0; /* Remove any default margin */
}

#shaped {
  margin-top: 4px; /* Add minimal space between button and text */
  border-radius: 15px;
  height: 30px;
  width: 120px;
  outline: none;
  border: none;
  background-color: #f0f0f0;
  font-size: 0.9rem;
}

.con-info {
  display: flex;
  flex-wrap: wrap;
  /* justify-content: center; */
  gap: 0.5rem;
  margin-top: 1.5rem;
  width: 500px;
}

.con-info button {
  padding: 8px 12px;
  border-radius: 15px;
  background: #ffffff;
  border: 2px solid #eeeeee;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 0.9rem;
}

/* Responsive Adjustments */
@media only screen and (max-width: 600px) {
  .header {
  margin-left:auto;
  }

  .con-flex {
   
    gap: 1rem;
    margin-top: 10px;
  }

  h1 {
    font-size: 1.4rem;
    text-align: center;
  }

  #shaped {
    width: 100px;
    font-size: 0.85rem;
  }


  .con-flex {
    padding: 0 10px;
  }

  img {
    width: 80px;
    height: 80px;
  }

  

  .con-info button {
    font-size: 0.8rem;
    padding: 6px 10px;
  }
}
</style>
