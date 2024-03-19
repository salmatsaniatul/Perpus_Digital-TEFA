<template>
  <div class="Header">
    <div class="h-img">
      <img src="~/assets/img/LOGO-SMK4.png" />
    </div>
    <div class="h-text">
      <div class="t-judul">
        <p>PERPUS DIGITAL</p>
        <p>SMK NEGERI 4 TASIKMALAYA</p>
      </div>
      <p>Jl.Depok, Sukamenak, Purbaratu</p>
    </div>
  </div>
</template>

<style scoped>
.Header {
  display: flex;
  align-items: center;
  width: 100%;
  height: 150px;
  background-color: #1a41a5 !important;
  color: rgb(255, 255, 255, 100%);
}

.h-img {
  margin-left: 25px;
}

.h-img > img {
  width: 80%;
}

.h-text {
  margin-left: -15px;
  line-height: 10px;
}

.t-judul {
  font-size: 20px;
  font-weight: 500;
}
@media only screen and (max-width: 40em) {
  .h-img {
    margin-left: 0.8rem;
  }

  .h-img > img {
    width: 70%;
  }

  .h-text {
    margin-left: -1.5rem;
    line-height: 5px;
  }

  .t-judul {
    font-size: 15px;
    font-weight: 500;
  }
}
</style>
