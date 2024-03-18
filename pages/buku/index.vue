<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="my-3">
          <input type="search" class="form-control rounded-5" placeholder="Mau baca buku apa hari ini?" />
        </div>
        <div class="my-3 text-muted">Menampilkan 4 dari 4</div>
        <div class="row">
          <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/buku/ayah">
                <div class="card-body">
                  <img src="~/assets/img/ayah.jpg" class="cover" alt="cover 1" />
                </div>
              </nuxt-link>
            </div>
          </div>
          <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/buku/alaska">
                <div class="card-body">
                  <img src="~/assets/img/alaska.jpg" class="cover" alt="cover 2" />
                </div>
              </nuxt-link>
            </div>
          </div>
          <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/buku/bincang">
                <div class="card-body">
                  <img src="~/assets/img/bincang.jpg" class="cover" alt="cover 3" />
                </div>
              </nuxt-link>
            </div>
          </div>
          <div class="col-lg-2">
            <div class="card mb-3">
              <nuxt-link to="/buku/dandelion">
                <div class="card-body">
                  <img src="~/assets/img/dandelion.jpg" class="cover" alt="cover 4" />
                </div>
              </nuxt-link>
            </div>
          </div>
        </div>
        <div class="d-flex justify-content-end">
          <nuxt-link to="/" class="btn btn-light btn-lg rounded-5 px-5 ms-auto">KEMBALI</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card-body {
  width: 100%;
  height: 30em;
  padding: 0;
}
.cover {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 0 30;
}

.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
