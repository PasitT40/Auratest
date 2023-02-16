<template>
  <v-row no-gutters>
    <Content :isShow="isShow" />
    <HoverMenuRight />
    <MenuMobile />
  </v-row>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      isShow: { status: false },
    };
  },
};
</script>
<style>
.mobile-menu {
  display: none;
}
.pc {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.item {
  height: 150px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.sectionHover {
  background-color: black;
  height: 100vh;
  width: 200px;
  position: absolute;
  right: 0;
  transition: width 0.5s;
  opacity: 0.75;
}
.sectionHover:hover {
  width: 400px;
}
.hide {
  display: none;
}
.colHover:hover .hide {
  display: block;
}
.textHover {
  color: gray !important;
}
.sectionText:hover .textHover {
  color: white !important;
}

@media screen and (max-device-width: 480px) {
  .mobile {
    display: none;
  }
  .mobile-menu {
    display: block;
  }
  .pc {
    display: flex;
    justify-content: center;
    align-items: center;
    height: auto;
  }
}
</style>
