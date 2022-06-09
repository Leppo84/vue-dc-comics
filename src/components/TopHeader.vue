<template>
  <header class="bg white">
    <div class="container fx jc-between ai-center">
      <a href="#">
        <img src="../assets/img/dc-logo.png" alt="Logo DC Home">
      </a>
      <nav>
        <ul>
          <li>
            <a class="txt-black" href="#">Placeholder</a>
          </li>
          <li>
            <a class="txt-black" href="#">Placeholder</a>
          </li>
          <li>
            <a class="txt-black" href="#">Placeholder</a>
          </li>
          <li>
            <a class="txt-black" href="#">Placeholder</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'TopHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

nav {
  text-align: end;

  ul {
    list-style-type: none;

    li {
      display: inline-block;
      padding: 20px 40px;

      a {
        text-decoration: none;


        &:hover {
          color: #0282f9;
        }
      }
    }
  }
}
</style>
