<template>
  <main>
    <div class="jumbotron">
    </div>
    <div class="main">
      <div class="wrapper-70">
        <div class="current_series">Current series</div>
        <div class="card_container" v-for="(comic, index_comic) in lista_comix" :key="index_comic">
          <div class="card">
            <img :src="comic.thumb" alt="img">
            <span>{{comic.series}}</span>
          </div>
        </div>
      </div>
      <a href="\"><div class="load-more">Load more</div></a>
    </div>
    <div class="advertisement">
      <div class="wrapper-70">

        <a href="">
          <div class="product">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital comics">
            <p>DC Comics</p>
          </div>
        </a>
        <a href="">
          <div class="product">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <p>DC Merchandise</p>
          </div>
        </a>
        <a href="">
           <div class="product">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <p>subscriptions</p>
          </div>
        </a>
        <a href="">
          <div class="product">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <p>Comic shop locator</p>
          </div>
        </a>
        <a href="">
          <div class="product">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <p>Dc power Visa</p>
          </div>
        </a>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'DcMain',
  props:{
    lista_comix: Array
    
  }
  }
</script>

<style scoped lang="scss">
  main{
    color:#fff;
  }
  .jumbotron{
    height:400px;
    width: 100%;
    background-image:url("../assets/img/jumbotron.jpg") ;
  }
  .main{
    text-transform: uppercase;
    width: 100%;
    padding-bottom:30px;
    background-color:#1C1C1C;
    .wrapper-70{
      display: flex;
      width: 70%;
      margin:0 auto;
      position: relative;
      flex-wrap: wrap;
      justify-content: space-around ;
      .current_series{
        display: inline-block;
        height: 50px;
        width:220px;
        line-height:50px;
        background-color: #0282F9;
        position: absolute;
        top:0;
        left:20px;
        transform: translate(0, -50%);
      }
      .card_container{
        width: 15%;
        margin-top: 60px;
        .card{
          .img{
            height: 800px;
          }
        }
      }
    }
    .load-more{
      display: inline-block;
      width:250px;
      height: 40px;
      line-height: 40px;
      margin:0 auto;
      background-color:#0282F9;
    }
    a{
      color:white;
      text-decoration: none;
    }
    
  }
  .advertisement{
      display:inline-block;
      width:100%;
      height:200px;
      background-color:#0282F9 ;
      .wrapper-70{
      display: flex;
      width: 70%;
      margin:0 auto;
      flex-wrap: wrap;
      justify-content: space-around;
      align-items: center;
      height: 100%;
      a{
        color:white;
        text-decoration: none;
        .product{
        display: flex;
        vertical-align: middle;
        img{
          height: 50px;
        }
        p{
          display: inline-block;
          text-transform: uppercase;
          line-height: 50px;
          margin-left: 10px;
        }
      }
      }
      }
    }
  
</style>