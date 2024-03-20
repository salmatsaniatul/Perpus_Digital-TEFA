<template>
  <div class="header">
    <div class="a-img">
      <img src="~/assets/img/LOGO-SMK4.png" alt="logo" />
    </div>

    <div class="a-text">
      <div class="i-judul">
        <p>Perpus Digital</p>
      </div>
      <p>SMKN 4 Tasikmalaya</p>
      <p>JL.Depok, Sukamenak, Purbaratu</p>
    </div>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  height: 140px;
  width: 100%;
  align-items: center;
  background-color: #265cb5;
  color: #fff;
}
.a-img > img {
  width: 60%;
}
.a-text {
  margin-left: -10px;
  line-height: 10px;
}
.i-judul {
  font-size: 35px;
  line-height: 1em;
  font-weight: 600;
}
</style>
