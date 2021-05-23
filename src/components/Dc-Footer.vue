<template>
  <footer>
    <div class="footer">
      <div class="wrapper-70">
        <div class="container-40">
          <div class="container-20">
            <h4>Dc Comics</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>Tv</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
            <h4>Shops</h4>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <div class="container-20">
            <h4>DC</h4>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy Policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certficates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <div class="container-20">
            <h4>Sites</h4>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>Dc Universe</li>
              <li>Dc Power Visa</li>
            </ul>
          </div>
          <div class="container-20">            
          </div>
        </div>
        <div class="container-60"></div>
      </div>
    </div>
    <div class="socials">

    </div>
  </footer>
</template>

<script>
export default {
  name: 'DcFooter'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .footer{
   width: 100%; 
   background-image: url("../assets/img/footer-bg.jpg");
   background-size:cover;
   .wrapper-70{
      display: flex;
      width: 70%;
      height:100%;
      margin:0 auto;
      .container-40{
        padding:40px 0;
        width:40%;
        height: 100%;
        display:flex;
        justify-content: space-between;
        .container-20{
          width:20%;
          text-align: left;
          h4{
            margin:20px 0;
            color:white;
            text-transform: uppercase;
            font-weight: bold;
            font-size:18px;
          }
          ul{
            list-style: none;
            li{
              color:white;
              text-decoration: none;
              font-size:14px;
              color:#707B83;
            }
          }

        }
      }
      .container-60{
          background-image: url("../assets/img/dc-logo-bg.png");
          background-repeat: no-repeat;
          background-size:unset;
          background-position: center;
          width:60%;
        }
    }
  }
  .socials{
    width:100%;
    height:90px;
    background-color:#303030;
  }
</style>