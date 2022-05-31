<template>
  <div id="Gallery">
    <h1 class="title">CAREERS</h1>
    <div>Take a look at our office space.</div>
    <ul>
      <li><img src="@/assets/img/t1@2x.png" /></li>
      <li><img src="@/assets/img/t2@2x.png" /></li>
      <li><img src="@/assets/img/t3@2x.png" /></li>
      <li><img src="@/assets/img/t4@2x.png" /></li>
      <li><img src="@/assets/img/t5@2x.png" /></li>
      <li><img src="@/assets/img/t6@2x.png" /></li>
    </ul>
  </div>
</template>

<style scoped>
#Gallery {
  height: 620px;
  background: rgba(216, 216, 216, 0.2);
  padding: 40px 0 50px;
  color: #2d2d2d;
  font-family: Helvetica-Light;
  font-size: 12px;
  font-weight: 200;
}
.title {
  font-family: Helvetica-Bold;
  font-size: 30px;
  letter-spacing: 0;
  font-weight: 700;
  margin-bottom: 10px;
}
.title::after {
  content: "";
  display: inline-block;
  width: 80px;
  height: 2px;
  background: var(--color-text);
  position: absolute;
  left: 50%;
  bottom: 0px;
  transform: translateX(-50%);
}
ul {
  width: 940px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
li {
  width: 300px;
  height: 200px;
  border-radius: 4px;
  margin-top: 24px;
}
li img {
  width: inherit;
}
</style>
