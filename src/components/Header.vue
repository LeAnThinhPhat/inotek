<template>
    <div class="header">
            <ul>
              <li><img src="../assets/logo-innotech.png" alt="logo"></li>
                <div class="home">
                  <li><router-link to="/">HOME</router-link></li>
                  <li> <router-link to="/provide">WE PROVIDE</router-link></li>
                  <li> <router-link to="/contact">CONTACT US</router-link></li>
                </div>
                  <div class="container nav-container">
            <input class="checkbox" type="checkbox" name="" id="" />
            <div class="hamburger-lines">
              <span class="line line1"></span>
              <span class="line line2"></span>
              <span class="line line3"></span>
            </div>  
          <div class="menu-items">
            <li><a href="#">Home</a></li>
            <li><a href="#">about</a></li>
            <li><a href="#">blogs</a></li>
            <li><a href="#">portfolio</a></li>
            <li><a href="#">contact</a></li>
          </div>
        </div> 
                <!-- <div class="language">
                  <li> <router-link to="/">EN</router-link></li>
                  <li> <router-link to="/">VN</router-link></li>     
                </div>    -->
            </ul>
    </div>
</template>
<script lang="ts">
import { computed, defineComponent, ref} from 'vue'
export default defineComponent({
     name: 'App',
  components: {},
  setup(){
    return { };
  }, 
})
</script>
<style scoped lang="scss">
/*Smart phone nhỏ*/
@media screen and (min-width: 240px){
    
}
/*Iphone(480 x 640)*/
@media screen and (min-width: 320px){
    .header {
  overflow: hidden;
  background-color: #121212;
  padding: 0px 0px;
  display: inline-block;
  text-align: center;
  width: 100%;
  .home li a {
    display: none;
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
  overflow: hidden;
  padding-left: 0;
   li {
    float: right;
    padding: 0px;
    margin: 10px;
    
    
        // a {
        // font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        // color: white;
        // padding: 0px;
        // text-decoration: none;
        // font-size: 18px;
        // line-height: 5px;
        // margin: 0;
        // text-align: center;
        // }
       }
   } 

  
 img {
      width: 60%;
      float: right;
    }
}
.home{
      // text-align: center;
      padding-left: 25%;
      padding-top: 1%;
    }
    .nav-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 62px;
}

.menu-items {
  display: flex;
}

.nav-container li {
  list-style: none;
}

.nav-container a {
  text-decoration: none;
  color: #0e2431;
  font-weight: 500;
  font-size: 1.2rem;
  padding: 0.7rem;
}

.nav-container a:hover{
    font-weight: bolder;
}

.nav-container {
  display: block;
  position: relative;
  height: 60px;
}

.nav-container .checkbox {
  position: absolute;
  display: block;
  height: 32px;
  width: 32px;
  top: 20px;
  left: 20px;
  z-index: 5;
  opacity: 0;
  cursor: pointer;
}

.nav-container .hamburger-lines {
  display: block;
  height: 26px;
  width: 32px;
  position: absolute;
  top: 17px;
  left: 20px;
  z-index: 2;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.nav-container .hamburger-lines .line {
  display: block;
  height: 4px;
  width: 100%;
  border-radius: 10px;
  background: white;
}

.nav-container .hamburger-lines .line1 {
  transform-origin: 0% 0%;
  transition: transform 0.4s ease-in-out;
}

.nav-container .hamburger-lines .line2 {
  transition: transform 0.2s ease-in-out;
}

.nav-container .hamburger-lines .line3 {
  transform-origin: 0% 100%;
  transition: transform 0.4s ease-in-out;
}

.menu-items {
  padding-top: 120px;
  box-shadow: inset 0 0 2000px rgba(255, 255, 255, .5);
  height: 100vh;
  width: 100%;
  transform: translate(-150%);
  display: flex;
  flex-direction: column;
  margin-left: -40px;
  padding-left: 50px;
  transition: transform 0.5s ease-in-out;
  text-align: center;
}

.menu-items li {
  margin-bottom: 1.2rem;
  font-size: 1.5rem;
  font-weight: 500;
}
.nav-container input[type="checkbox"]:checked ~ .menu-items {
  transform: translateX(0);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line1 {
  transform: rotate(45deg);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line2 {
  transform: scaleY(0);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line3 {
  transform: rotate(-45deg);
}

.nav-container input[type="checkbox"]:checked ~ .logo{
  display: none;
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
  .header {
  overflow: hidden;
  background-color: #121212;
  padding: 5px 10px;
  display: inline-block;
  text-align: center;
  width: 100%;
  .home li a {
    display: inline-block;
    color: white;
    text-align: center;
    text-decoration: none;
    font-size: 18px;
    line-height: 5px;
    border-radius: 4px;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    
  }
  .home li a:hover {
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
    
    img {
      cursor: pointer;
      width: 90%;
      // border: 1px solid white;
    }
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
  .nav-container {
  display: none;
  justify-content: space-between;
  align-items: center;
  height: 62px;
}

.navbar .menu-items {
  display: none;
}

.navbar .nav-container li {
  list-style: none;
}

.navbar .nav-container a {
  text-decoration: none;
  color: #0e2431;
  font-weight: 500;
  font-size: 1.2rem;
  padding: 0.7rem;
}

.navbar .nav-container a:hover{
    font-weight: bolder;
}

.nav-container {
  display: none;
  position: relative;
  height: 60px;
}

.nav-container .checkbox {
  position: absolute;
  display: block;
  height: 32px;
  width: 32px;
  top: 20px;
  left: 20px;
  z-index: 5;
  opacity: 0;
  cursor: pointer;
}

.nav-container .hamburger-lines {
  display: block;
  height: 26px;
  width: 32px;
  position: absolute;
  top: 17px;
  left: 20px;
  z-index: 2;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.nav-container .hamburger-lines .line {
  display: block;
  height: 4px;
  width: 100%;
  border-radius: 10px;
  background: #0e2431;
}

.nav-container .hamburger-lines .line1 {
  transform-origin: 0% 0%;
  transition: transform 0.4s ease-in-out;
}

.nav-container .hamburger-lines .line2 {
  transition: transform 0.2s ease-in-out;
}

.nav-container .hamburger-lines .line3 {
  transform-origin: 0% 100%;
  transition: transform 0.4s ease-in-out;
}

.navbar .menu-items {
  padding-top: 120px;
  box-shadow: inset 0 0 2000px rgba(255, 255, 255, .5);
  height: 100vh;
  width: 100%;
  transform: translate(-150%);
  display: flex;
  flex-direction: column;
  margin-left: -40px;
  padding-left: 50px;
  transition: transform 0.5s ease-in-out;
  text-align: center;
}

.navbar .menu-items li {
  margin-bottom: 1.2rem;
  font-size: 1.5rem;
  font-weight: 500;
}
.nav-container input[type="checkbox"]:checked ~ .menu-items {
  transform: translateX(0);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line1 {
  transform: rotate(45deg);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line2 {
  transform: scaleY(0);
}

.nav-container input[type="checkbox"]:checked ~ .hamburger-lines .line3 {
  transform: rotate(-45deg);
}

.nav-container input[type="checkbox"]:checked ~ .logo{
  display: none;
}
}
</style>
