<script setup>
import Icon10002 from "@/assets/icons/svg/10002.svg?vueComponent";
import Icon10003 from "@/assets/icons/svg/10003.svg?vueComponent";
import Icon10001 from "@/assets/icons/svg/10001.svg?vueComponent";
import Icon10004 from "@/assets/icons/svg/10004.svg?vueComponent";
import Icon10005 from "@/assets/icons/svg/10005.svg?vueComponent";
import Iconjr from "@/assets/icons/svg/jr.svg?vueComponent";
</script>

<template>
  <div id="Solutions">
    <h1 class="title">SOLUTIONS</h1>
    <p>
      Drop us a line at hrsgnf@newfuture.com with your resume to discuss how we
      can craft your career together.
    </p>
    <ul>
      <li>
        <Icon10002 width="24" height="24" />
        <div class="description">
          <div>
            <h4>Front-end Development</h4>
          </div>
          <p>
            Beautiful graphic design. Stunning web pages. Because people ignore
            design that ignores people.
          </p>
        </div>
      </li>
      <li>
        <Icon10003 width="24" height="24" />
        <div class="description">
          <h4>Backend Development</h4>
          <p>
            A dedicated team of developers to thrive on complex, end‑to‑end
            backend challenges.
          </p>
        </div>
      </li>
      <li>
        <Icon10001 width="24" height="24" />
        <div class="description">
          <h4>Mobile App Development</h4>
          <p>
            We develop mobile solutions that will meet your business needs and
            goals. Our experience covers the development of native,
            cross-platform and hybrid mobile apps.
          </p>
        </div>
      </li>
      <li>
        <Icon10004 width="24" height="24" />
        <div class="description">
          <h4>QA and Testing</h4>
          <p>
            Software quality assurance is paramount. It represents the key to
            unlocking a better return on investment and to establishing a
            strong, positive relationship with your customer base. We offer a
            wide range of software testing services to help you achieve it.
          </p>
        </div>
      </li>
      <li>
        <Icon10005 width="24" height="24" />
        <div class="description">
          <h4>IT Consultancy</h4>
          <p>
            If you need help identifying the technology barriers that stand
            between you and a more profitable business, our software consultants
            can help.
          </p>
        </div>
      </li>
    </ul>
    <div class="advertising">
      <Iconjr width="60" height="60" />
      <h1 class="text1">Begin your new future now with us.</h1>
      <div class="text2">We strive to bring you the best.</div>
    </div>
  </div>
</template>

<style scoped>
#Solutions {
  /* height: 420px; */
  padding-top: 40px;
  font-family: Helvetica-Light;
  font-size: 14px;
  color: #2d2d2d;
  font-weight: 200;
  letter-spacing: 0;
}
.title {
  font-family: Helvetica-Bold;
  font-size: 30px;
  font-weight: 700;
  position: relative;
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
  font-size: 12px;
  display: flex;
  flex-wrap: wrap;
  width: 940px;
  margin: 10px auto 0;
  text-align: left;
}
li {
  display: flex;
  margin-top: 20px;
  width: 33.3%;
}
h4 {
  font-family: Helvetica-Bold;
  font-size: 14px;
  font-weight: 700;
  margin-bottom: 10px;
}
.description {
  width: 260px;
  margin-left: 10px;
  line-height: 14px;
}
.advertising {
  margin-top: 50px;
  height: 220px;
  background-image: url(../assets/img/advertising.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  padding-top: 35px;
}
.advertising::before {
  content: "";
  width: 100%;
  height: 100%;
  display: block;
  position: absolute;
  bottom: 0;
  left: 0%;
  background: var(--theme-color);
  opacity: 0.7;
}
.text1 {
  font-family: Helvetica-Bold;
  font-size: 30px;
  color: #ffffff;
  letter-spacing: 0;
  font-weight: 700;
}
.text2 {
  font-family: Helvetica-Light;
  font-size: 12px;
  color: #ffffff;
  font-weight: 200;
  margin-top: 16px;
}
</style>
