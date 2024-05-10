<template>
  <div class="container-fluid">
    <div class="row">
      <h3 class="t" style="text-align: center">Detail buku</h3>
      <div class="col-lg-2">
        <div class="card mt-5">
          <div class="card-body">
            <img :src="buku.cover" class="cover" alt="cover" />
          </div>
        </div>
      </div>
      <div class="col-lg-4">
        <div class="row">
          <ul class="list-group list-group-flush">
            <li class="list-group-item">Judul : {{ buku.judul }}</li>
            <li class="list-group-item">Penulis : {{ buku.penulis }}</li>
            <li class="list-group-item">Penerbit : {{ buku.penerbit }}</li>
            <li class="list-group-item">Tahun Terbit : {{ buku.tahun_terbit }}</li>
            <li class="list-group-item">Kategori : {{ buku.kategori }}</li>
            <li class="list-group-item">Rak : {{ buku.rak }}</li>
            <li class="list-group-item">Isbn : {{ buku.isbn }}</li>
            <li class="list-group-item">Jumlah Halaman : {{ buku.jumlah_halaman }}</li>
            <li class="list-group-item">Deskripsi : {{ buku.deskripsi }}</li>
          </ul>
        </div>
      </div>
      <div class="d-flex justify-content-end">
        <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-5 ms-auto">KEMBALI</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient();

const route = useRoute();

const buku = ref([]);

const getBookById = async () => {
  const { data, error } = await supabase.from("buku").select(`*, kategori(*)`).eq(`id`, route.params.id);
  if (data) buku.value = data[0];
};

onMounted(() => {
  getBookById();
});
</script>

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
