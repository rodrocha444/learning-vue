<script setup lang="ts">
  import './styles/global.css'
  import TopAd from './components/TopAd.vue'

</script>

<template>
  <div id="container">
    <TopAd text-of-ad="Up to $7,500 tax credit available for Model Y and Model 3. Learn More"/>
    <section id="firstSection">
      <img id="imgBackground" src="https://w.wallhaven.cc/full/eo/wallhaven-eodvmr.png"/>
      <header>
        <div id="logoTesla">Tesla</div>
        <nav id="productsNav">
          <span>Model S</span>
          <span>Model S</span>
          <span>Model S</span>
          <span>Model S</span>
          <span>Model S</span>
        </nav>
        <nav id="menuNav">
          <span>Shop</span>
          <span>Account</span>
          <span>Menu</span>
        </nav>
      </header>
      <main>
        <div>
          <div>Experience Tesla</div>
          <div>Schedule a Demo Drive Today</div>
        </div>
        <button>Demo Drive</button>
      </main>
    </section>
    
  </div>
</template>

<style scoped>
#container{
  display: flex;
  flex-direction: column;
  height: 100vh;
  overflow: hidden;
}

#firstSection{
  display: flex;
  flex-direction: column;
  position: relative;
  flex:1;
}

#imgBackground{
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  filter: blur(5px);
  
}

header{
  padding: 1.5rem;
  display: flex;
  width: 100%;
  font-size: 0.95rem;
  color: white;
}

#logoTesla, #productsNav, #menuNav{
  flex: 1;
  display: flex;
}

#logoTesla{
  justify-content: flex-start;
}

#productsNav{
  gap: 3rem;
  justify-content: center;
}

#menuNav{
  gap: 3rem;
  justify-content: flex-end;
}

#firstSection main{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 4.5rem;
  flex:1;
}

#firstSection main > div{
  color: white;
  text-align: center;
}

#firstSection main > div :first-child{
  font-size: 3rem;
  font-weight: 400;
  word-spacing: 10px;
}

#firstSection main > button{
  background: transparent;
  border: 4px solid white;
  padding: 0.5rem 6rem;
  color: white;
}
</style>