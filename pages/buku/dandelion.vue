<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <div class="card-body">
                <img src="~/assets/img/dandelion.jpg" class="cover" alt="cover 4 " />
              </div>
            </div>
          </div>
          <div class="col-lg-6" style="margin-left: 50px">
            <h1>Detail Buku</h1>
            <p>Judul Novel : Dandelion Lovers</p>
            <p>Penulis : Fahrul Khakim</p>
            <p>Tahun terbit : 2015</p>
            <p>Jumlah halaman : -</p>
            <p>ISBN : -</p>
            <p>
              Deskripsi : May merasa dirinya bagai setangkai bunga dandelion yang kehilangan mahkotanya. Hampa dan merana. Putik indahnya diterbangkan angin bernama cinta. Bukan angin yang lembut tapi angin yang kacau bernama patah hati.
              Angin yang membuat setangkai dandelion di tepi jalan jadi terlihat sama, tak memikat dan usang. Dandelion itu berusaha berdiri lagi.
            </p>
          </div>

          <div class="d-flex justify-content-between">
            <nuxt-link to="../pengunjung" class="btn btn-dark btn-lg rounded-5 px-5" style="margin-top: 10px">KIRIM</nuxt-link>
            <nuxt-link to="/buku" class="btn btn-light btn-lg rounded-5 px-5" style="margin-top: 10px">KEMBALI</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.cover {
  height: 300px;
  width: 200px;
}
.card.mb-3 {
  margin-top: 50px;
  margin-left: 20px;
  height: 340px;
  width: 235px;
}
h3 {
  margin-top: 50px;
  margin-right: 20px;
}
img {
  height: 300px;
  width: 200px;
}
.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
