<template>
  <div id="app">
     <div class="navibar ">
        <Navibar /> 
     </div> 
    
    <main>
     <Home class="home"/>
     <About class="about"/>
     <Work class="work"/>
     <Contact class="contact"/>
     <Foot class="footer"/>

    </main>
    <div v-if="seen" id="gotop">
      <svg class="icon" v-on:click="gotop">
             <use xlink:href="#icon-huojian"></use>
      </svg>
        
    </div>
    
  </div>
</template>

<script>
import Navibar from './components/Navibar'
import Home from './components/Home'
import Work from './components/Work'
import About from './components/About'
import Contact from './components/Contact'
import Foot from './components/Foot'



export default {
  name: 'app',
  data(){
    return {
      scroll: '',
      seen : false
    }
  },
  components: {
    Navibar,
    Home,
    Work,
    About,
    Contact,
    Foot
  },
  methods:{
    gotop :function(){
      document.documentElement.scrollTop = 0
    },
    menu() {
    this.scroll = document.documentElement.scrollTop;
      if(this.scroll>600){
        this.seen=true;
      }else{
        this.seen=false;
      }
    }
    },
    mounted() {
      window.addEventListener('scroll', this.menu)
    },

  }

</script>

<style lang = "scss" scoped>

 @media screen and (max-width: 600px) {
    
  }


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 1920px;
   .navibar{
      width: 100%;
      position: fixed;
      background:rgb(60,174,162);
      height:70px;
    }     
    main{
        width: 100%;
        .home{
          background:rgb(60,174,162);
          height:580px;
        }
        .about{
          width:1280px;
          margin:100px auto;
       }
        .work{
        width:100%;
        background:rgb(247,247,247);
       }
        .contact{
         width:100%;
         background:rgb(60,174,162);
      }
        .foot{
        padding:30px 0;
        background:rgb(256,256,247);
      }

    }
    #gotop{
       & >.icon {
         width: 3.5em; height: 3.5em;
         vertical-align: -0.15em;
         overflow: hidden;
         position: fixed;
         bottom:60px;
         right: 50px; 
         cursor: pointer;
         fill : #ddd;
        }

        i:hover{
        opacity: 0.8;
        }
    }
}


</style>
