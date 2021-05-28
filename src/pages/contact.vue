<template>
  <h1>Contacts</h1>
  <div class="grid-container1">
    <div class="grid-item3">
      <p>
        <a href="mailto:admin.readtolisten@gmail.com"
          >Email : {{ contact.email }} <br
        /></a>
        phone : {{ contact.phone }} <br />
        line : {{ contact.line }} <br />
        <a href="https://www.facebook.com/nattxkw"
          >Facebook : {{ contact.fb }}<br
        /></a>
      </p>
      <h1>Thank You For Watching!!!</h1>
      <img src="@/assets/giphy1.gif" width="400" height="400" />
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    contact: {
      email: "kwanchai.se@ku.th",
      phone: "0822987233",
      line: "n7233",
      fb: "Nattx",
    },
  }),
};
</script>

<style >
h1 {
  text-align: center;
  font-size: 50px;
}
.grid-container1 {
  display: grid;
  grid-template-columns: auto;
  background-color: #2196F3;
  padding: 10px;
  width: 100%;
  height: 100%;
}
.grid-item3 {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 50px;
  font-size: 30px;
  text-align: center;
  width: 94%;
  height: 87%;
}
</style>
