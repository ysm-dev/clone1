<template>
  <div class="container">
    <navigate-card />
    <main-card />
    <div class="loadmore">
      <div class="button">
        <span>
          load more
        </span>
        <img src="ic_arrow_bottom.svg"
             alt="">
      </div>
    </div>
    <footer-card />
  </div>
</template>

<script>
import { NavigateCard, MainCard, FooterCard } from '@/components'

export default {
  components: {
    NavigateCard,
    MainCard,
    FooterCard,
  },
}
</script>

<style lang="scss" scoped>
.container {
  overflow: hidden auto;
  height: 100%;
  .loadmore {
    display: flex;
    justify-content: center;
    text-align: center;
    .button {
      display: flex;
      margin: 5px 0px 35px 0px;
      padding-right: 5px;
      padding-left: 15px;
      border-radius: 5px;
      span {
        color: #b3b3b3;
        text-transform: uppercase;
        letter-spacing: 1.5px;
        font-weight: 900;
        font-size: 12px;
        line-height: 50px;
      }
      img {
      }
      &:hover {
        background-color: rgba(0, 0, 0, 0.05);
        cursor: pointer;
      }
    }
  }
}
</style>
