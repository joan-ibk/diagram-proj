<template>
  <div class="build-main">
    <div class="build-flex">
      <h3>What is the product you’re building?</h3>
      <p>
        Our first product, Automator , lets designers create their own
        automation tools, without writing code. Tens of thousands of designers
        and hundreds of teams are using Automator to speed up their design
        workflow. See this amazing site by @Marco Cornacchia about Automator in
        2022!
      </p>
      <p>
        We’re about to launch our second product, Magician , a collection of
        AI-powered tools that lets designers quickly prototype copy, glyphs, and
        images for their designs. It will soon solve previously intractable
        problems like automatically naming your layers, and add new capabilities
        you’ll help define, packaged as individual “spells” that can be
        prototyped and released quickly.
      </p>
      <p>
        Our next product, Genius , combines the latest AI models and engineering
        to deliver an auto-completing smart assistant experience right within
        tools like Figma. We’re really excited about our progress towards
        “drawing boxes better” and would love to work with you on it.
      </p>
      <p>
        We have a lot of exciting ideas for the future— our own UI-AI Glyphs
        model, Xdesign app, and more. Past experiments like Prototyper , UI
        Archive , and more show our unwavering commitment to build our ideas in
        public and push forward the field as a whole where we can.
      </p>
    </div>
   
    <div class="design-footer">
        <div class="design">
      <h3>What design tools do you use day to day?</h3>
      <ul>
        <li><a href="#">Figma</a></li>
        <li><a href="#">Automator</a></li>
        <li><a href="#">Magician</a></li>
      </ul>
    </div>
    <div class="footer">
      <h3>What does your stack look like?</h3>
      <h4>Web</h4>
      <p>We ❤️ Typescript</p>
      <ul>
        <li> <a href="#">React + Next.js</a> </li>
        <li> <a href="#">Tailwind</a> </li>
        <li> <a href="#">GraphQL</a> </li>
        <li> <a href="#">Node + Express + RPC</a> </li>
      </ul>
      <h4>Mobile</h4>
      <ul>
        <li>Swift + SwiftUI</li>
      </ul>
      <h4>Infrastructure</h4>
      <ul>
        <li> <a href="#">AWS</a> </li>
        <li> <a href="#">Vercel</a> </li>
        <li> <a href="#">Modal</a> </li>
      </ul>
      <h4>ML</h4>
      <ul>
        <li>pytorch</li>
        <li>weights&biases</li>
        <li>🤗 hub / datasets / diffusers</li>
      </ul>
    </div>
    </div>
    <div class="last-link">
        <a href="#">Share</a>
    </div>
  </div>
    
 
</template>


<style scoped>
.build-main{
    padding: 20px;
}
.build-flex{
    width:550px;
    line-height: 22px;
}
.design-footer{
    position: relative;
    /* left: -8.5%; */
}
.footer{
    margin-top: 50px;
}
a{
    text-decoration: none;
    line-height: 30px;
  font-size: 14px;
  color: #111111;
}
p{
    color: #111111;
  font-size: 14px;
  font-weight: 400;
}
h3{
    color: #111111;
  font-size: 17px;
  font-weight: 500;
}
li{
  list-style: none;
  line-height: 30px;
  font-size: 14px;
  color: #111111;
}
.last-link{
    display: flex;
    justify-content: center;
    align-items: center;
}


@media only screen and (max-width: 600px){

.build-main{
    margin-left: auto;
}
}
</style>