<template>
  <div class="container-fluid">
    <div class="row my-5">
      <div class="col-lg-6">
        <nuxt-link to="/pengunjung/tambah">
          <div class="card bg-pengunjung rounded-5">
            <div class="card-body">
              <h2>Pengunjung</h2>
            </div>
          </div>
        </nuxt-link>
      </div>

      <div class="col-lg-6">
        <nuxt-link to="/buku">
          <div class="card bg-buku rounded-5">
            <div class="card-body">
              <h2>Cari Buku</h2>
            </div>
          </div>
        </nuxt-link>
      </div>

      <h2 class="mt-4" style="font-family: ; margin-left=150px;">STATISTIK</h2>
      <div class="col-lg-6">
        <nuxt-link to="/pengunjung">
          <div class="card kunjungan rounded-5 mt-5">
            <div class="card-body text">
              <h1>0</h1>
              <h2 class="pt-5">pengunjung</h2>
            </div>
          </div>
        </nuxt-link>
      </div>
      <div class="col-lg-6">
        <nuxt-link to="/buku">
          <div class="card buku rounded-5 mt-5">
            <div class="card-body text">
              <h1>4</h1>
              <h2 class="pt-5">Buku</h2>
            </div>
          </div>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  height: 250px;
  box-shadow: 1px 1px 10px #1a41a5;
}
.card.bg-pengunjung {
  background-image: url("../assets/img/bg-kunjungan.jpeg");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  color: black;
  opacity: 50%;
}
.card.bg-buku {
  background: url("../assets/img/bg-cari buku.jpeg") no-repeat center center;
  background-size: cover;
  color: black;
  opacity: 50%;
}
.card.kunjungan {
  background-color: #f4eb0f;
  opacity: 50%;
  color: black;
}

.card.buku {
  background-color: #5fbb8f;
  opacity: 50%;
  color: black;
}
.text {
  display: flex;
  align-items: center;
}
.text > h1 {
  font-size: 7rem;
}
</style>
