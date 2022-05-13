<template>

  <header>

    <div>
      <img style="cursor:pointer" src="../assets/img/dc-logo.png" alt="">
    </div>

    <ul>
      <li v-for="(item, index) in menu" :key="`menu-${index}`">
       <a :class="{'active':item.isActive}" href="item.href">{{item.name}}</a>
      </li>
    </ul>
  </header>
  
</template>

<script>
export default {
  name: "HeaderComponent",
  data(){
    return{
      menu:[
        {
          name: "characters",
          href: "#",
          isActive: false
        },
        {
          name: "comics",
          href: "#",
          isActive: true
        },
        {
          name: "movies",
          href: "#",
          isActive: false
        },
        {
          name: "tv",
          href: "#",
          isActive: false
        },
        {
          name: "games",
          href: "#",
          isActive: false
        },
        {
          name: "collectibles",
          href: "#",
          isActive: false
        },
        {
          name: "videos",
          href: "#",
          isActive: false
        },
        {
          name: "fans",
          href: "#",
          isActive: false
        },
        {
          name: "news",
          href: "#",
          isActive: false
        },
        {
          name: "shop",
          href: "#",
          isActive: false
        }


      ] 
    }
  }
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