<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <div class="card-body">
                <img src="~/assets/img/alaska.jpg" class="cover" alt="cover 1 " />
              </div>
            </div>
          </div>
          <div class="col-lg-6" style="margin-left: 50px">
            <h1 style="text-align: center">Detail Buku</h1>
            <p>Judul Novel : Teluk Alaska</p>
            <p>Penulis : Eka Aryani</p>
            <p>Penerbit : Bumi Semesta Media</p>
            <p>Tahun terbit : 24 Juli 2019</p>
            <p>Jumlah halaman : 408 halaman</p>
            <p>ISBN : 978602550888</p>
            <p>
              Deskripsi : Alister Reygan, cowok yang selalu menjadi idaman para wanita. Bukan hanya sekadar tampan, ia juga memiliki sebuah geng yang sering disebut sebagai ‘Penguasa Sekolah’.Nasib sial menimpa cewek teman sekelasnya. Ia
              selalu menjadi objek bullying oleh gengnya. Allister sebagai ketua selalu paling kasar dan semangat dalam mem-bully cewek tersebut.
            </p>
          </div>
          <div class="d-flex justify-content-end">
            <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-5 ms-auto">KEMBALI</nuxt-link>
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
