<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">ISI BUKU KUNJUNGAN</h2>
        <form>
          <div class="mb-3">
            <input type="text" class="form-control form-control-lg rounded-4" placeholder="Nama..." />
          </div>
          <div class="mb-3">
            <select class="form-control form-control-lg form-select rounded-4">
              <option value="">KEANGGOTAAN</option>
              <option value="Siswa">Siswa</option>
              <option value="Guru">Guru</option>
              <option value="Staf">Staf</option>
              <option value="Umum">Umum</option>
            </select>
          </div>
          <div class="mb-3">
            <div class="row">
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-4 mb-2">
                  <option value="">TINGKAT</option>
                  <option value="X">X</option>
                  <option value="XI">XI</option>
                  <option value="XII">XII</option>
                </select>
              </div>
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-4 mb-2">
                  <option value="">JURUSAN</option>
                  <option value="PPLG">PPLG</option>
                  <option value="TJKT">TJKT</option>
                  <option value="TSM">TSM</option>
                  <option value="DKV">DKV</option>
                  <option value="TOI">TOI</option>
                </select>
              </div>
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-4 mb-2">
                  <option value="">KELAS</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>
                </select>
              </div>
            </div>
          </div>
          <div class="col-mb-3">
            <select class="form-control form-control-lg form-select rounded-4">
              <option value="">KEPERLUAN</option>
              <option value="baca">Baca Buku</option>
              <option value="pinjam">Pinjam Buku</option>
              <option value="kembalikan">Mengembalikan Buku</option>
            </select>
          </div>
          <div class="d-flex justify-content-between">
            <nuxt-link to="../pengunjung" class="btn btn-dark btn-lg rounded-4 px-5" style="margin-top: 10px">KIRIM</nuxt-link>
            <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-4" style="margin-top: 10px">KEMBALI</nuxt-link>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<style scoped>
.btn-dark {
  box-shadow: 1px 1px 10px #e4ecea !important;
}
.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
