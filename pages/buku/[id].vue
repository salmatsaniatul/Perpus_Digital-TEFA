<template>
  <div class="container-fluid">
    <div class="row">
      <h3 class="t" style="text-align: center">Detail buku</h3>
      <div class="col-lg-2">
        <div class="card mt-10">
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
            <li class="list-group-item">
              <span v-if="buku.kategori">Kategori: {{ buku.kategori.nama }}</span>
              <span v-else>loading...</span>
            </li>
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

const buku = ref({});

const getBookById = async () => {
  const { data, error } = await supabase.from("buku").select(`*, kategori(*)`).eq(`id`, route.params.id).single();
  if (data) buku.value = data;
};

onMounted(() => {
  getBookById();
});
</script>

<style scoped>
img {
  width: 100%;
}

.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
