<template>
    
    <div class="container">
      <button @click="componentToRender='Home'">Home</button>
      <button @click="componentToRender='About'">About</button>
      <button @click="componentToRender='ListHelperVue'">ListHelper</button>
      <button @click="componentToRender='Contact'">Contact</button>
      <keep-alive>
         <component :is="componentToRender"></component>
      </keep-alive>
     
      
    </div>

</template>

<script>
import Home from './components/Home.vue'
import About from './components/About.vue'
import Contact from './components/Contract.vue'
import ListHelperVue from './components/ListHelper.vue'
export default {

  data(){
    return {
      componentToRender: 'Contact'
    }
  },
  components:{
    Home,About,Contact,ListHelperVue
  },
  created(){
    setTimeout(()=>{
      this.loader = 'other'
    },3000)
  }
  
}
</script>

