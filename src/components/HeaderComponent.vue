<template>

  <header>

    <div>
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <ul>
      <li><a href="#">characters</a></li>
      <li><a class="active" href="#">comics</a></li>
      <li><a href="#">movies</a></li>
      <li><a href="#">tv</a></li>
      <li><a href="#">games</a></li>
      <li><a href="#">collectibles</a></li>
      <li><a href="#">videos</a></li>
      <li><a href="#">fans</a></li>
      <li><a href="#">news</a></li>
      <li><a href="#">shop</a></li>
    </ul>
  </header>
  
</template>

<script>
export default {
  name: "HeaderComponent"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variable.scss";

header{
  width: 80%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  font-size: 14px;

  img{
    width: 80%;
  }

  ul{
    display: flex;
  }

  li{
    list-style: none;
    margin-right: 30px;

    a{
      text-transform: uppercase;
      color: black;
      text-decoration: none;
      padding: 36px 0;

      &:hover{
        color: $primary-color;
      }

      &.active{
        color: $primary-color;
        border-bottom: 6px solid $primary-color;
      }

    }


  }

}

</style>