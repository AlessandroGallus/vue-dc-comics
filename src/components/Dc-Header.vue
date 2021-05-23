<template>
  <header>
    <a href="/">
      <img src="../assets/img/dc-logo.png" alt="Logo">
    </a>
    <ul>
      <li v-for="(link, index) in menu_header" :key="index">
        <a :class="{'active': link.current}" :href="link.url">{{link.text}}</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'DcHeader',
  props:{
    menu_header: Array
    
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header{
    display: flex;
    text-align: center;
    margin-bottom: 1rem;
    justify-content: space-around;
    align-items: center;
  }
  ul{
    margin: 2rem 0;
    li{
      display: inline-block;
    }
    a{
      text-decoration: none;
      margin:1rem;
      padding:2rem 0;
      color:#51565B;
      &:hover,
      &.active{
        color:#4AABFC;;
        border-bottom: 4px solid #4AABFC;
      }
    }
  }
</style>


