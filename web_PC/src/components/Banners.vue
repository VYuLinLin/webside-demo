<template>
  <el-carousel height="580px" id="Home">
    <el-carousel-item v-for="item in 3" :key="item">
      <div class="banner banner_bj">
        <h4 class="title1">Bundled With Tons of</h4>
        <h1 class="title2">Cutting-Edge Solutions</h1>
        <h6 class="title3">
          State your needs and we will turn your ideas into reality
        </h6>
        <div class="btn">FIND OUT MORE</div>
      </div>
    </el-carousel-item>
  </el-carousel>
</template>

<script>
import { defineComponent } from 'vue'
import { ElCarousel, ElCarouselItem } from "element-plus";
export default defineComponent({
  components: {
    ElCarousel,
    ElCarouselItem,
  },
});
</script>

<style>
.banner {
  padding-top: 180px;
}
.banner_bj {
  height: 100%;
  background-image: url(../assets/img/banner@2x.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}
.title1 {
  font-family: Helvetica-Bold;
  font-weight: 700;
  font-size: 24px;
  letter-spacing: 0;
}
.title2 {
  font-family: Helvetica-Bold;
  font-weight: 700;
  font-size: 70px;
  letter-spacing: 0;
}
.title3 {
  font-family: Helvetica-Light;
  font-size: 12px;
  letter-spacing: 0;
  font-weight: 200;
  margin-top: 10px;
}
.btn {
  width: 130px;
  height: 38px;
  line-height: 38px;
  background: var(--theme-color);
  font-family: Helvetica-Bold;
  font-size: 12px;
  font-weight: 700;
  border-radius: 19px;
  display: inline-block;
  margin-top: 50px;
  cursor: pointer;
}
.el-carousel__button {
  width: 50px;
  height: 4px;
  border-radius: 2px;
}
.el-carousel__arrow i {
  font-size: 24px;
}
</style>
