<template>
  <header class="bg white">
    <div class="container fx jc-between ai-center">
      <a href="#">
        <img id="logo-dc" src="../assets/img/dc-logo.png" alt="Logo DC Home">
      </a>
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index" :class="link.current?'active':''">
            <a :href="link.url">
              {{link.text}}
            </a>
          </li>
        </ul>
      </nav>
    </div>
    <div class="jumbotron">
      <img src="../assets/img/jumbotron.jpg" alt="Awesome comics!">
    </div>
  </header>
</template>

<script>
export default {
  name: 'TopHeader',
    props: {
      links: Array,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

header.bg {
  // padding: 6px 0 0;
}

#logo-dc {
  width: 100px;
  padding: 5px;
}

nav {
  text-align: end;
  position: relative;
  top: 4px;

  ul {
    list-style-type: none;

    li {
      display: inline-block;
      padding: 45px 10px;
      &.active {
        border-bottom: 4px solid #0282f9;

        a {
          color: #0282f9;
        }

      }

      a {
        text-decoration: none;
        color: black;
        font-size: smaller;
        font-weight: bold;


        &:hover {
          color: #0282f9;
        }
      }
    }
  }
}

.jumbotron {
  // background-image: url(../assets/img/jumbotron.jpg);
  img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    object-position: top center;
    position: relative;
    top: 4px;
  }
}

</style>
