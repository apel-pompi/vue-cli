<template>
    
    <div>
      <Header :myName="Student"/>
      <Futter/>
    </div>

</template>

<script>
import  Header  from "./components/Header_Futter/Header";
import  Futter  from "./components/Header_Futter/Futter";
export default {
  data(){
    return{
      Student:['Ashrafur Rahman','Apel','Khokon','Pompi']
    }
  },
  components:{
    Header,
    Futter,
  }
  
}
</script>

