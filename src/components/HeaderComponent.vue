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
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
  border: 1px solid black;
  font-size: 14px;

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
      padding: 35px 0;

      &:hover{
        color: $primary-color;
      }

      &.active{
        border-bottom: 6px solid $primary-color;
      }

    }


  }

}

</style>