<template>
    <div class="footer">
           <ul>
                <div class="home">
                   <li><router-link to="/">HOME</router-link></li>
                  <li> <router-link to="/provide">WE PROVIDE</router-link></li>
                  <li> <router-link to="/contact">CONTACT US</router-link></li>
                </div>
                
            </ul>
    </div>
</template>
<script lang="ts">
import { computed, defineComponent, ref} from 'vue'
export default defineComponent({
     name: 'App',
  components: {},
  setup(){
   
    return {};
  }, 
})
</script>
<style scoped lang = "scss">
/*Smart phone nhỏ*/
@media screen and (min-width: 240px){
    
}
/*Iphone(480 x 640)*/
@media screen and (min-width: 320px){
  .footer {
  overflow: hidden;
  background-color: #121212;
  padding: 0px 0px;
  display: inline-block;
  text-align: center;
  width: 100%;
  a {
    color: white;
    text-align: center;
    text-decoration: none;
    font-size: 5px;
    line-height: 5px;
    border-radius: 4px;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }
  a:hover {
    color: orangered;
    transition: 700ms;
  }
  ul {
  list-style-type: none;
  margin: 0;
  text-align: center;
  overflow: hidden;
   li {
    float: left;
    padding: 0px;
    margin: 5px;
        a {
        font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        color: white;
        padding: 8px;
        text-decoration: none;
        font-size: 13px;
        line-height: 5px;
        margin: 0;
        display: inline-block;
        text-align: center;
        }
      }
  } 
  
 
}
.home{
      padding-left: 5%;
      padding-top: 1%;
    }
}
/*Tablet nhỏ(480 x 640)*/
@media screen and (min-width: 480px){
    
}
/*Ipad dọc(768 x 1024)*/
@media screen and (min-width: 768px){
    
}
/*Ipad ngang(1024 x 768)*/
@media screen and (min-width: 1024px){
  .footer {
  overflow: hidden;
  background-color: #121212;
  padding: 5px 10px;
  display: inline-block;
  text-align: center;
  width: 100%;
  a {
    color: white;
    text-align: center;
    text-decoration: none;
    font-size: 18px;
    line-height: 5px;
    border-radius: 4px;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    
  }
  a:hover {
    color: orangered;
    transition: 700ms;
  }
  ul {
  list-style-type: none;
  margin: 0;
  text-align: center;
  // border: 1px solid white;
  overflow: hidden;
  padding-left: 20%;
   li {
    float: left;
    padding: 5px;
    margin: 5px;
        a {
        font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        color: white;
        padding: 5px;
        text-decoration: none;
        font-size: 18px;
        line-height: 5px;
        // border: 1px solid white;
        margin: 0;
        text-align: center;
        }
      }
  } 
  
 
}
.home{
      // text-align: center;
      padding-left: 25%;
      padding-top: 1%;
    }
}

</style>
