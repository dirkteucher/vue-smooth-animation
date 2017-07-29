<template>
  <div class="vueContainer" v-on:click="changeBackgroundColour()">
    <div class="firstLineContainer">
      <div class="firstLine">

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>



        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

      </div>
    </div>

    <div class="secondLineContainer">
      <div class="secondLine">

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>



        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

        <div class="singleObject">
          <h4>{{ msg }}</h4>
        </div>

      </div>
    </div>

  </div>

</template>

<script>
export default {
  name: 'Hello',
  data () {
    return {
      msg: '1'
    }
  },
  methods: {
    changeBackgroundColour(){

      function getRandomColor () {
        var hex = Math.floor(Math.random() * 0xFFFFFF);
        return "#" + ("000000" + hex.toString(16)).substr(-6);
      }

      $(".singleObject h4").css("background-color", getRandomColor())
    }
  },
  mounted: function(){
    console.log("----------A short explanation of what this code is doing.----------");
    console.log("1) I watched the react presentation on fibre and wanted to try out vueJS to see how fast it was. It turns out that Vue is pretty fast.");
    console.log("2) The view is found inside Hello.vue ... go take a look.");
    console.log("3) This hello.view file contains a template, scss, data, and computational methods which are like a controller");
    console.log("4) This example has 40+ elements on a setInterval of 16ms and the whole container is being animated. "+
    +"It's silky smooth not that I can recall ever having to animate 80+ elements each containing reactive 2 way data binded properties but who knows, maybe one day I will need to.");
    console.log("-");
    console.log("5) And it only took 45 minutes to build the entire project with vue-cli + webpack.");
    console.log("6) Adding routing takes a few minutes as does adding vuex for more complicated data managment system and you get hot-reloading out the box.")
    console.log("7) I really like VueJS!");

      setInterval(() => {
         this.msg++; // |this| properly refers to the person object
       }, 16);

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
/*Remember to install the  following to ensure scss works*/
/*  npm install sass-loader node-sass webpack --save-dev  */
.vueContainer {
  height: 590px;
  overflow: hidden;
}

.firstLine {
  width: 100%;
}

.firstLine .singleObject {
  position: relative;
  margin-right: 1%;
  padding-left: 1%;
}

$i: 100;
@while $i > 0 {
  .singleObject:nth-child(#{$i}) {
    left: 4.1% * $i;
    top: -20px * $i;

  }
  $i: $i - 1;
}

h4 {
  background-color: green;
  width:4%;
  height:20px;
  border-radius:45px;
  color: #fff;
  padding:2px;
}


.vueContainer {
  width: 100%;
  animation: vuexSecond 4s ease-in-out 0s infinite;
}

.secondLine {
  width: 100%;

}

@keyframes vuexSecond{
0% {
  width: 100%;
}

50% {
  width: 50%;
  background-color: white;
}

100% {
  width: 100%;
}
}

.secondLineContainer {
  position: relative;
  top: -1040px;
  left: 98%;
}
.secondLine .singleObject {
  position: relative;
  margin-right: 1%;
  padding-left: 1%;
}
$secondLine: 100;
@while $secondLine > 0 {
.secondLine .singleObject:nth-child(#{$secondLine}) {
  left: -4.1% * $secondLine;
  top: -20px * $secondLine;

}
  $secondLine: $secondLine - 1;
}
</style>
