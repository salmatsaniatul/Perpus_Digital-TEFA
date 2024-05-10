<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <div class="my-3">
          <form @sumbit.prevent="getBooks">
            <input v-model="keyword" type="search" class="form-control rounded-5" placeholder="Mau baca buku apa hari ini?" />
          </form>
        </div>
        <div class="my-3 text-muted">Menampilkan {{ books.length }} dari {{ banyak }}</div>
        <div class="row">
          <div v-for="(book, i) in books" :key="i" class="col-lg-2">
            <nuxt-link :to="`buku/${book.id}`">
              <div class="card mb-4">
                <div class="card-body">
                  <img :src="book.cover" class="cover" alt="cover buku" />
                </div>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="d-flex justify-content-end">
    <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-4 ms-auto">KEMBALI</nuxt-link>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient();

const keyword = ref("");

const books = ref([]);

const banyak = ref([]);

const getBooks = async () => {
  const { data, error } = await supabase.from("buku").select(`*, kategori(*)`).ilike("judul", `%${keyword.value}%`);
  if (error) throw error;
  if (data) books.value = data;
};

const banyakBuku = async () => {
  const { data, count } = await supabase.from("buku").select("*", { count: "exact" });
  if (data) banyak.value = count;
};

onMounted(() => {
  getBooks();
  banyakBuku();
});
</script>

<style scoped>
.card-body {
  width: 100%;
  height: 25rem;
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
