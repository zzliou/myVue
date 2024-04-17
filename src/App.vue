<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="container">
    <div class="header">
      <div class="red" onclick="alert('這是紅色');"></div>
    </div>
    <div class="footer">
      <div class="wrapper">
        <div class="purple" onclick="alert('這是紫色');"></div>
        <div class="middleWrapper">
          <div class="blue"onclick="alert('這是藍色');"></div>
          <div class="bottomWrapper">
            <div class="black" onclick="alert('這是黑色');"></div>
            <div class="white" onclick="alert('這是白色');"></div>
          </div>
        </div>
        <div class="green" onclick="alert('這是綠色');"></div>
      </div>
    </div>
  </div>

</template>

<style lang='scss'>

.container {
  width: 100%;
  height: auto;
  .header {
    display: flex;
    .red {
      background-color: #EA0000;
      width: 900px;
      height: 200px;
      
      @include change {
        background-color: yellow;
      }
    }
  }
  .footer {
    width: 100%;
    height: auto;
    .wrapper {
      display: flex;
      .purple {
        width: 300px;
        height: 500px;
        background-color: 	#930093;
      }
      .middleWrapper {
        width: 300px;
        height: 500px;
        .blue {
          height: 250px;
          background-color:#000093;
        }
        .bottomWrapper {
          display: flex;
          height: 250px;
          .black {
            background-color: #000000;
            width: 50%;
          }
          .white {
            background-color: 	#FFFFFF;
            width: 50%;
          }
        }
      }
      .green {
        width: 300px;
        height: 500px;
        background-color: #009100;
      }
    }
  }
}
</style>
