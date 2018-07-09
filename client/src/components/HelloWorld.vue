<template>

  <div class="hello">
  <div id="blackBar">

  </div>
  <div id = "header">
   <ul>
    <li>What We Do</li>
    <li>Subjects offered</li>
    <li>Book your free assessment</li>
    <li>Book Your Session</li>
    <li>Contact us</li>
   </ul>
  </div>

  <div id = "slider">
    <figure>
      <img src = "../../images/geom.jpg">
      <img src = "../../images/geom.jpg">
      <img src = "../../images/geom.jpg">
    </figure>
  </div>
  <div id = "info">
    <article>
      <img src = "../../images/K-6.png">
    </article>
    <aside>
    Hello
    </aside>
  </div>
  <div id = "info2">
    Shiny!
  </div>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      welcome: 'Hello its me, I will be your tutor!!!!!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#blackBar{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:20px;
  background-color:black;
}
html{
    height:2000px;
}
#header{
  position:fixed;
  left:0;
  top:20px;
  width:100%;
  height: 45px;
  background-color:lightgrey;
}
@keyframes slider {
  0% {
    left: 0;
  }
  20% {
    left: 0;
  }
  25% {
    left:-100%;
  }
  45% {
    left: -100%;
  }
  50% {
    left: -200%;
  }
  70% {
    left: -200%;
  }
  75% {
    left: -300%;
  }
  95% {
    left: -400%;
  }
  100% {
    left: -400%;
  }
}

#slider {
  overflow: hidden;
  left: 0;

  display:block;
  width: 100%;
}

#slider figure img {
  width: 20%;
  float:left;
}

#slider figure {
  position: relative;
  width: 500%;
  margin: 0;
  left: 0;
  text-align: left;
  font-size: 0;
  animation: 20s slider;
}

#info {
  text-align:left;
  display:block;
  width: 100%;
}

#info2 {
  text-align:left;
  display:block;
  width: 100%;
}

article {
  float: left;
  margin: 0 auto;
  width: 50%;
  height: auto;
}

aside {
  float:right;
  margin: 0 auto;
  width: 50%;
  height: auto;
}
</style>
