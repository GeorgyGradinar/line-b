<template>
  <div class="main">
    <img src="/img/newLogoLB.png" alt="">

    <div class="content">
      <p class="address">0xe517b8367bcdf9b556402a81e6e67efed87ac03f</p>
      <p class="text">Buy now or fomo</p>


      <div class="buttons">
        <a href="https://syncswap.xyz/swap?outputCurrency=0xe517b8367bcdf9b556402a81e6e67efed87ac03f" target="_blank">Buy</a>
        <a href="https://www.dextools.io/app/en/linea/pair-explorer/0x5ed8e8f554e00f3992abecbc392104c6c23cf504?t=1713187103674"
           target="_blank">Chart</a>
      </div>
    </div>
  </div>
</template>

<script setup>

useHead({
  htmlAttrs: {
    lang: 'ru'
  },
  title: 'LINE-B',
})

</script>

<style scoped lang="scss">
.main {
  position: relative;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: flex-start;

  img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    object-fit: cover;
  }

  .content {
    display: flex;
    flex-direction: column;
    margin-left: 60px;
    margin-top: 240px;
    z-index: 2;

    .address {
      color: white;
      margin-bottom: 30px;
      font-size: 20px;
    }

    .text {
      color: white;
      font-size: 35px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      gap: 20px;

      a {
        color: white;
        text-decoration: none;
        font-size: 25px;
        border: 1px solid white;
        padding: 10px 20px;
        transition: all 0.2s;

        &:first-of-type {
          background-color: #f7931a;
          color: black;
          border: 1px solid #f7931a;
          font-weight: 700;

          &:hover {
            transform: scale(1.1);
          }
        }

        &:hover {
          background-color: #f7931a;
          color: black;
          border: 1px solid #f7931a;
        }
      }
    }
  }

}
</style>
