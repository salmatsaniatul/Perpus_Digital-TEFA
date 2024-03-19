<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
        <div class="my-3">
          <input type="search" class="form-control form-control-lg rounded-4" placeholder="Filter..." />
        </div>
        <div class="my-3 text=muted">menampilkan 4 dari 4</div>
        <table class="table">
          <thead>
            <tr>
              <td>NO</td>
              <td>NAMA</td>
              <td>KATEGORI</td>
              <td>WAKTU</td>
              <td>KEPERLUAN</td>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>1.</td>
              <td>salma tsaniatul</td>
              <td>Siswa</td>
              <td>27 februari 2024, 09.22.13</td>
              <td>Pinjam Buku</td>
            </tr>
          </tbody>
          <tbody>
            <tr>
              <td>2.</td>
              <td>dita nursabila</td>
              <td>Siswa</td>
              <td>28 februari 2024, 10.21.03</td>
              <td>mengembalikan buku</td>
            </tr>
          </tbody>
          <tbody>
            <tr>
              <td>3.</td>
              <td>elisa mardiyani</td>
              <td>Siswa</td>
              <td>28 februari 2024, 10.29.13</td>
              <td>mengembalikan buku</td>
            </tr>
          </tbody>
          <tbody>
            <tr>
              <td>4.</td>
              <td>sofwatul jamilah</td>
              <td>Siswa</td>
              <td>18 Maret 2024, 10.22.13</td>
              <td>Pinjam Buku</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
  <div class="d-flex justify-content-end">
    <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-5 ms-auto">KEMBALI</nuxt-link>
  </div>
</template>

<style scoped>
.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
