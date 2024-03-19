<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <div class="card-body">
                <img src="~/assets/img/ayah.jpg " class="cover" alt="cover 2 " />
              </div>
            </div>
          </div>
          <div class="col-lg-6" style="margin-left: 50px">
            <h1 style="text-align: center">Detail Buku</h1>
            <p>Judul Novel : Ayah</p>
            <p>Penulis : Andrea Hirata</p>
            <p>Penerbit : PT Bentang Pustaka</p>
            <p>Tahun terbit : Pertama, Mei 2015</p>
            <p>Jumlah halaman : 412 halaman</p>
            <p>ISBN : 9786022911029</p>
            <p>
              Deskripsi : Novel Ayah ini mengabarkan bahwa Belitong tidak seindah Laskar Pelangi yang menerangkan panorama alam Belitong. Novel Ayah lebih mengisahkan kondisi sosial dan psikologi manusia Belitong. Membaca Ayah ini seperti
              sedang mendengarkan paparan bagaimana manusia Belitong berinteraksi.
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
