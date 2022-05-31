<script setup>
import Icon10007 from "@/assets/icons/svg/10007.svg?vueComponent";
import Icon10008 from "@/assets/icons/svg/10008.svg?vueComponent";
import Icon10009 from "@/assets/icons/svg/10009.svg?vueComponent";
import Icon10010 from "@/assets/icons/svg/10010.svg?vueComponent";
import Icon10011 from "@/assets/icons/svg/10011.svg?vueComponent";
import Icon10012 from "@/assets/icons/svg/10012.svg?vueComponent";
</script>

<template>
  <div id="Careers">
    <h1 class="title">CAREERS</h1>
    <div>
      Drop us a line at hrsgnf@newfuture.com with your resume to discuss how we
      can craft your career together.
    </div>
    <ul>
      <li>
        <Icon10007 width="48" height="48" />
        <h4 class="title1">Front-end Developer</h4>
        <div class="description">
          <p>
            Front-end developers don’t just create static sites – they also know
            how to code up interactive pages and web apps.
          </p>

          <p>
            Tasks: Front-end development could be right for you if you like the
            idea of prototyping and building interactive sites, debugging across
            browsers, and managing user data.
          </p>

          <p>
            Skills: Git + GitHub, JavaScript, jQuery, Grunt/Gulp, SASS, HTML,
            CSS, frameworks like Bootstrap, Node.js, AngularJS, and Ember.js
          </p>
        </div>
      </li>
      <li>
        <Icon10008 width="48" height="48" />
        <h4 class="title1">Backend Developer</h4>
        <div class="description">
          <p>
            Have you ever wondered how websites are turned into apps? That’s the
            secret super power of mobile developers!
          </p>

          <p>
            Tasks: You’ll work as a mobile developer to optimize code for
            mobile, take designs from prototype to code, and test and analyze
            code for mobile.
          </p>

          <p>
            Skills: Git + GitHub, iOs, Android, other languages like Ruby,
            Objective-C, or Java
          </p>
        </div>
      </li>
      <li>
        <Icon10009 width="48" height="48" />
        <h4 class="title1">UX Designer</h4>
        <div class="description">
          <p>
            User experience designers are a lot like information architects,
            only they spend more time coding, mocking up designs, and working
            with developers.
          </p>

          <p>
            Tasks: If you get into UX design, your job will include developing
            prototypes, mocking up designs, designing specs, researching and
            analyzing user experience and behavior to iterate and traction test.
          </p>

          <p>
            Skills: HTML, CSS, JavaScript, wireframing tools, version control
            tools, data analysis, Git + GitHub
          </p>
        </div>
      </li>
      <li>
        <Icon10010 width="48" height="48" />
        <h4 class="title1">Software Developer</h4>
        <div class="description">
          <p>
            Software developers design apps and programs. Microsoft Word?
            Software devs were behind it.
          </p>

          <p>
            Tasks: Are you ready to write code; design, prototype, and analyze
            software; and work with designers, product managers, and
            programmers? Then there’s probably a future software developer in
            you waiting to get out!
          </p>

          <p>
            Skills: Git + GitHub, skills like HTML, CSS, SASS, JavaScript, Java,
            MySQL, Ruby, Python, Responsive Web Design, jQuery, frameworks, PHP,
            Apache, etc
          </p>
        </div>
      </li>
      <li>
        <Icon10011 width="48" height="48" />
        <h4 class="title1">Data Architects</h4>
        <div class="description">
          <p>
            Being a data architect is like being the architect for the virtual
            house that an organization’s data will live in.
          </p>

          <p>
            Tasks: As a data architect, you’ll spend your days designing and
            building systems for collecting, processing, and storing data.
          </p>

          <p>
            Skills: understanding of databases and data storage, systematic
            thinking
          </p>
        </div>
      </li>
      <li>
        <Icon10012 width="48" height="48" />
        <h4 class="title1">UI Designer</h4>
        <div class="description">
          <p>
            User interface designers work closely with user experience
            designers, but rather than focusing on analysis, user interface
            designers are all about the look and feel of a site.
          </p>

          <p>
            Tasks: Your work as a UI designer will be to design site interfaces
            and graphics, do customer analysis, perform design research, and
            create branding and interactive and animated designs.
          </p>

          <p>
            Skills: Photoshop, wireframing, prototyping tools, HTML, CSS,
            JavaScript, Git + GitHu
          </p>
        </div>
      </li>
    </ul>
  </div>
</template>

<style scoped>
#Careers {
  color: #2d2d2d;
  font-family: Helvetica-Light;
  font-size: 12px;
  font-weight: 200;
  padding: 40px 0 50px;
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
  background: #fdfdfd;
  border: 1px solid rgba(221, 221, 221, 1);
  border-radius: 4px;
  margin-top: 24px;
  padding: 20px;
}
.title1 {
  font-family: Helvetica-Bold;
  font-size: 14px;
  font-weight: 700;
  margin: 8px 0;
}
.description {
  text-align: left;
  line-height: 14px;
}
.description p {
  margin-top: 12px;
}
</style>
