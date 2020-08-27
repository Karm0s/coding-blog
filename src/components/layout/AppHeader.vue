<template>

  <div>
    <div class="header flex flex-wrap items-center justify-between px-5 md:px-10">
      <div class="brand">
        <img src="../../assets/BushidoCodeLogo.png" class="h-12">
      </div>

      <div class="header-actions">
        <mq-layout mq="sm">
          <button @click.prevent="headerMenuButtonClick">
            <img src="../../assets/burger-menu-icon.svg" width="30px" alt="">
          </button>
        </mq-layout>

        <mq-layout mq="md+">
          <button class="btn header-btn">
            <a href="">About</a>
          </button>
          <button class="btn header-btn">
            <a href="">Contact</a>
          </button>
        </mq-layout>
      </div>
    </div>

    <div class="header-menu flex flex-col mb-5" :class="menuState">
      <a class="py-3 text-white" href="">About</a>
      <a class="py-3 text-white" href="">Contact</a>
    </div>
  </div>

</template>

<script>
export default {
  name: 'AppHeader',

  data() {
    return {
      menuVisible: false,
    };
  },
  computed: {
    menuState() {
      return (this.menuVisible)? '' : 'hidden';
    }
  },
  methods: {
    headerMenuButtonClick() {
      this.menuVisible = !this.menuVisible;
    }
  }
};
</script>

<style scoped>
.header{
  height: 70px;
}
.header-btn{
  height: 70px;
  width: 80px;
  color: var(--white);
}
</style>
