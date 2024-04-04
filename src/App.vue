<template>
    
    <div>
      <Header :myName="name"/>
      <Futter/>
    </div>

</template>

<script>
import  Header  from "./components/Header_Futter/Header";
import  Futter  from "./components/Header_Futter/Futter";
export default {
  data(){
    return{
      name:'Ashrafur Rahman'
    }
  },
  components:{
    Header,
    Futter,
  }
  
}
</script>

