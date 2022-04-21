<template>
  <div class="app-header">
    <div class="logo"><a href="#">COFFEE HOUSE</a></div>
    <ul class="menu_ul">
      <li class="menu_li"><a href="#" class="menu_link"></a>HOME</li>
      <li class="menu_li"><a href="#" class="menu_link"></a>STORY</li>
      <li class="menu_li"><a href="#" class="menu_link"></a>BLOG</li>
      <li class="menu_li"><a href="#" class="menu_link"></a>SUBSCRIBE</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'AppHeader'

}
</script>

<style lang="scss" scoped>
.app-header {
  display: flex;
  justify-content: space-between;
  padding: 0px 80px;
  background: #FFFFFF;

  .logo {
    display: flex;
    width: 204px;
    height: 53px;
    align-self: center;

    a {
      text-decoration: none;
      color: #000000;
      font-weight: 500;
      font-size: 36px;
      line-height: 53px;
    }
  }

  .menu_ul {
    display: flex;
    flex-direction: row;
    height: 36px;
    font-weight: 300;
    font-size: 24px;
    line-height: 36px;
    list-style: none;
    color: #000000;

    .menu_li {
      margin-right: 46px;
      
    }
  }
}




</style>