<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <div class="card-body">
                <img src="~/assets/img/bincang.jpg" class="cover" alt="cover 3 " />
              </div>
            </div>
          </div>
          <div class="col-lg-6" style="margin-left: 50px">
            <h1 style="text-align: center">Detail Buku</h1>
            <p>Judul Novel : Bincang Akhlak</p>
            <p>Penulis : Takdir Alisyahbana Ridwan</p>
            <p>Penerbit : Mediakita</p>
            <p>Tahun terbit : 5 November 2019</p>
            <p>Jumlah halaman : 256 halaman</p>
            <p>ISBN : 9789797945954</p>
            <p>
              Deskripsi : Di buku ini menceritakan tentang kehidupannya dari kecil hingga akhirnya menikah dengan “My Love”. Ini bukan cerita kehidupan biasa, Bang Jek akan menulis perjalanan Spiritual nya yang dahulu banyak maksiat sampai
              akhirnya terjadi satu kejadian yang membuatnya hijrah dan meninggalkan segala kemaksiatan.
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
