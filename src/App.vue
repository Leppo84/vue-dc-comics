<template>
  <div id="app">
    <TopHeader>
    </TopHeader>
    <SecContents>
    </SecContents>
    <SecPurchases>
    </SecPurchases>   
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
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  border: 0;
  box-sizing: border-box;
  text-align: center;
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
  padding: 5px 0;
}

.container {
  width: 90%;
  display: flex;
}

.row {
  width: 100%;
}

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
