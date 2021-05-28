<template>
  <h1>Welcome To My Profile</h1>
  <div class="grid-container">
    <div class="grid-item1">
      <img src="@/assets/6130200145.jpg" width="200" height="250" />
      <p2><br /><br />ประวัติส่วนตัว</p2>
      <p>
        ชื่อจริง : {{ profile.first_name }}<br />
        ชื่อเล่น : {{ profile.nick_name }}<br />
        วันเกิด : {{ profile.bd }}<br />
        อายุ : {{ profile.age }}<br />
        เพศ : {{ profile.sex }}<br />
        ที่อยู่: {{ profile.location }}<br />
        การศึกษา : {{ profile.education }}<br />
        GPA: {{ profile.gpa }}
      </p>
    </div>
    <div class="grid-item2">
      <h1>Skills&Soft Skill</h1>
      <p>
        Skills : {{ profile.code }}<br />
        Soft Skill : {{ profile.skill }}<br />
      </p>
      <img src="@/assets/giphy.gif" width="250" height="250" />
      <div style="position: relative; left: 650px; top: 60px">
        <p>
          Contact Click Here
          <button @click="goToContact()">
            <img
              src="@/assets/030onnvptu6j2izibkbi_28_contact-us.png"
              width="200"
              height="50"
            />
          </button>
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    profile: {
      first_name: " ขวัญชัย เสนศรี",
      nick_name: " แน็ต",
      bd: " 17 มกราคม 2543",
      age: 21,
      sex: " ชาย",
      location:
        " 154/290 ซ.ศิริชัย ถ.ศรีสุริยวงศ์ ต.หน้าเมือง อ.เมือง จ.ราชบุรี 70000",
      education:
        "2561-ปัจจุบัน มหาวิทยาลัยเกษตรศาสตร์ วิทยาเขตศรีราชา,สาขาวิทยาการคอมพิวเตอร์",
      gpa: 2.71,
      skill:
        " มีทัศนคติที่ดีและเปิดใจยอมรับสิ่งใหม่,สามารถสร้างความสัมพันธ์ที่ดีกับเพื่อนร่วมงาน,มีความรับผิดชอบสูง",
      code: " HTML/php,JAVA,C#/C++,SQL",
    },
  }),
  methods: {
    goToContact() {
      this.$router.push("/contact");
    },
  },
};
</script> 
<style >
p {
  color: #2196F3;
  font-size: 24px;
  text-align: left;
  padding-left: 20px;
}
p2 {
  color: #2196F3;
}
h1 {
  color: #2196F3;
  text-align: center;
  font-size: 50px;
}
.grid-container {
  display: grid;
  grid-template-columns: auto auto;
  background-color: #2196F3;
  padding: 10px;
  width: 100%;
  height: 100%;
}
.grid-item1 {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 50px;
  font-size: 30px;
  text-align: center;
  width: 600px;
  height: 600px;
}
.grid-item2 {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 50px;
  font-size: 30px;
  text-align: center;
  width: 1060px;
  height: 600px;
}
</style>