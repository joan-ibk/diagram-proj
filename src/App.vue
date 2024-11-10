<template>
  <SideBar />
  <HeaderWorld />
  <IntroDeets />
  <BuildDeets />
  
</template>

<script>
import HeaderWorld from "./components/HeaderWorld.vue";
import IntroDeets from "./components/IntroDeets.vue";
import BuildDeets from "./components/BuildDeets.vue";
import SideBar from "./components/SideBar.vue";

export default {
  name: "App",
  components: {
    SideBar,
    HeaderWorld,
    IntroDeets,
    BuildDeets,
   
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&display=swap");

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 50px;
  font-family: "Inter", sans-serif;
}
* {
  margin: 0;
  padding: 0;
  list-style: none;
  box-sizing: border-box;
}
img {
  width: 92px;
  height: 92px;
  gap: 0px;
  opacity: 0px;
}
@media only screen and (max-width: 600px) {
  .container {
    display: flex;
    width: 100%;
    flex-direction: column; /* Switch to column layout on small screens */
    margin: 50px;
  }
  .con-flex {
 
  padding: 0px;
}
}
</style>
