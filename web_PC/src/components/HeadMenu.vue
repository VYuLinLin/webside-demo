<template>
  <header>
    <div class="content">
      <div class="logo">logo</div>
      <div class="menu">
        <a
          v-for="val in menuList"
          :key="val"
          :class="active === val && 'active'"
          :href="`#${val}`"
          @click="activeHandler(val)"
          >{{ val }}
        </a>
      </div>
    </div>
  </header>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      menuList: ["Home", "About", "Solutions", "Careers", "Gallery", "Contact"],
      active: "Home",
    };
  },
  methods: {
    activeHandler(a) {
      this.active = a;
    },
  },
});
</script>

<style scoped>
header {
  height: 50px;
  line-height: 50px;
  border-bottom: 1px solid var(--theme-color);
}
.content {
  width: 940px;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
}
.logo {
  font-family: Helvetica-Bold;
  font-size: 24px;
  color: var(--color-text);
  letter-spacing: 0;
  font-weight: 700;
}
.menu {
  font-family: Helvetica-Light;
  font-size: 12px;
  color: #2d2d2d;
  font-weight: 200;
}
.menu a {
  display: inline-block;
  width: 54px;
  margin-left: 17px;
  text-align: center;
}
.menu .active {
  font-family: Helvetica-Bold;
  color: var(--color-text);
  font-weight: 700;
  position: relative;
}
.menu .active::after {
  content: "";
  display: inline-block;
  width: 30px;
  height: 2px;
  background: var(--color-text);
  position: absolute;
  left: 10px;
  bottom: 12px;
}
</style>
