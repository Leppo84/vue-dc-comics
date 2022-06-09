<template>
  <div id="app" class="fx wrap">
    <TopHeader :links="menu"/>
    <!-- <main class="fx"> -->
      <SecContents>
      </SecContents>
      <SecPurchases>
      </SecPurchases>   
    <!-- </main> -->
    <TopFooter>
    </TopFooter>
    <BottomFooter>
    </BottomFooter>
  </div>
</template>

<script>
import TopHeader from './components/TopHeader.vue'
import SecPurchases from './components/SecPurchases.vue'
import SecContents from './components/SecContents.vue'
import TopFooter from './components/TopFooter.vue'
import BottomFooter from './components/BottomFooter.vue'



export default {
  name: 'App',
  components: {
    TopHeader,
    SecPurchases,
    SecContents,
    TopFooter,
    BottomFooter
  },
  data() {
    return {
      menu: [
        {
          text: "CHARACTERS",
          url:"#",
          current: false,
        },
        {
          text: "COMICS",
          url:"#",
          current: true,
        },
        {
          text: "MOVIES",
          url:"#",
          current: false,
        },
        {
          text: "TV",
          url:"#",
          current: false,
        },
        {
          text: "GAMES",
          url:"#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url:"#",
          current: false,
        },
        {
          text: "VIDEOS",
          url:"#",
          current: false,
        },
        {
          text: "FANS",
          url:"#",
          current: false,
        },
        {
          text: "NEWS",
          url:"#",
          current: false,
        },
        {
          text: "SHOP",
          url:"#",
          current: false,
        },

      ]
    }
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  border: 0;
  box-sizing: border-box;
  // text-align: center;
}

#app {
  font-family: 'Roboto Condensed', sans-serif;
}

// palette

.white {
  background-color: white;
}

.txt-white {
  color: white;
}

.black {
  background-color: black;
}

.txt-black {
  color: black;
}

.dc-blue {
  background-color: #0282f9;
}

.dc-txt-blue {
  color: #0282f9;
}

.dc-darkgrey {
  background-color: #303030;
}

.dc-txt-darkgrey {
  color: #303030;
}

.dc-mediumgrey {
  background-color: #797979;
}

.dc-txt-mediumgrey {
  color: #797979;
}

// structure rules

.bg {
  width: 100%;
  // padding: 5px 0;
}

.container {
  width: 80%;
  margin: 0 auto;
}

.fx {
  display: flex;
}

.wrap {
  flex-wrap: wrap;
}

.col50 {
  width: 50%;
}

.col-sixth {
  width: calc(100% / 6);
}

// .row {
//   width: 100%;
// }

.ai-center {
  align-items: center;
}

.jc-center {
  justify-content: center;
}

.jc-between {
  justify-content: space-between;
}

.ji-center {
  justify-items: center;
}

</style>
