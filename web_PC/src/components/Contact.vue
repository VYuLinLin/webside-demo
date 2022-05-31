<template>
  <div id="Contact">
    <h1 class="title">GET IN TOUCH</h1>
    <div>
      Send us your resume and portfolio! We look forward to meeting you.
    </div>
    <div class="form">
      <el-form
        ref="ruleFormRef"
        :model="ruleForm"
        status-icon
        :rules="rules"
        label-width="120px"
        class="demo-ruleForm"
      >
        <el-form-item prop="name">
          <el-input
            class="input-name"
            v-model="ruleForm.name"
            placeholder="Your Name"
            autocomplete="off"
          />
          <el-input
            class="input-email"
            v-model="ruleForm.email"
            placeholder="Your Email"
            autocomplete="off"
          />
        </el-form-item>
        <el-form-item prop="subject">
          <el-input
            v-model="ruleForm.subject"
            placeholder="Subject"
            autocomplete="off"
          />
        </el-form-item>
        <el-form-item prop="message">
          <el-input
            v-model.number="ruleForm.message"
            placeholder="Your Message"
            type="textarea"
            :autosize="{ minRows: 5, maxRows: 5 }"
          />
        </el-form-item>
        <el-form-item>
          <el-button
            class="submit"
            type="primary"
            @click="submitForm(ruleFormRef)"
            round
            >SEND MESSAGE</el-button
          >
        </el-form-item>
      </el-form>
      <ul>
        <li>
          <Icon10013 width="20" height="20" />
          <h4 class="title1">Location</h4>
          <div class="content">
            Millenia Tower, One Temasek Avenue#37-01/04/05/06, Singapore 039192
          </div>
        </li>
        <li>
          <Icon10014 width="20" height="20" />
          <h4 class="title1">Email</h4>
          <div class="content">hrsgnf@newfuture.com</div>
        </li>
        <li>
          <Icon10015 width="20" height="20" />
          <h4 class="title1">Phone</h4>
          <div class="content">+65 6251 7737</div>
        </li>
      </ul>
    </div>

    <div class="dt"></div>
  </div>
</template>

<script setup>
import Icon10013 from "@/assets/icons/svg/10013.svg?vueComponent";
import Icon10014 from "@/assets/icons/svg/10014.svg?vueComponent";
import Icon10015 from "@/assets/icons/svg/10015.svg?vueComponent";
import { reactive, ref } from "vue";

const validator = (rule, value, callback) => {
  if (!value) {
    return callback(new Error("Please input the value"));
  }
  callback();
};

const ruleForm = reactive({
  name: "",
  email: "",
  subject: "",
  message: "",
});

const rules = reactive({
  //   name: [{ validator: validator, trigger: "blur" }],
  //   email: [{ validator: validator, trigger: "blur" }],
  //   subject: [{ validator: validator, trigger: "blur" }],
  //   message: [{ validator: validator, trigger: "blur" }],
});

const submitForm = (formEl) => {
  if (!formEl) return;
  formEl.validate((valid) => {
    if (valid) {
      console.log("submit!");
    } else {
      console.log("error submit!");
      return false;
    }
  });
};
</script>

<style scoped>
#Contact {
  /* height: 620px; */
  padding-top: 40px;
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
.form {
  width: 940px;
  margin: 30px auto 50px;
  display: flex;
  justify-content: space-between;
}
.title1 {
  font-family: Helvetica-Bold;
  font-size: 14px;
  color: #2d2d2d;
  font-weight: 700;
}
.form ul li {
  width: 200px;
  text-align: left;
  margin-bottom: 10px;
}
.content {
  font-family: Helvetica-Light;
  font-size: 12px;
  color: #2d2d2d;
  font-weight: 200;
  word-break: break-all;
}
.dt {
  height: 340px;
  background-image: url(@/assets/img/dt.png);
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
<style>
.el-form {
  width: 710px;
}
.el-form-item__content {
  margin-left: 0 !important;
  display: flex;
  justify-content: space-between;
}
.el-input__wrapper,
.el-textarea__inner {
  height: 38px;
  background: rgba(216, 216, 216, 0.3);
  border-radius: 19px;
}
.el-input__inner {
  padding-left: 10px;
}
.el-textarea__inner {
  padding-left: 20px;
}
.input-name,
.input-email {
  width: 350px;
}
.submit {
  height: 38px;
  background-color: var(--theme-color) !important;
  border: none !important;
  border-radius: 19px;
}
</style>
