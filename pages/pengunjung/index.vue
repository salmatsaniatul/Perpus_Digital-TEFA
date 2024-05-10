<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
        <div class="my-3">
          <input type="search" class="form-control form-control-lg rounded-4" placeholder="Filter..." />
        </div>
        <div class="my-3 text=muted">menampilkan {{ visitors.length }} dari {{ banyak }}</div>
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
            <tr v-for="(visitor, i) in visitors" :key="i">
              <td>{{ i + 1 }}.</td>
              <td>{{ visitor.nama }}</td>
              <td>{{ visitor.keanggotaan.nama }}</td>
              <!-- <td>{{ visitor.tingkat.nama }}</td>
              <td>{{ visitor.jurusan.nama }}</td>
              <td>{{ visitor.kelas.nama }}</td> -->
              <td>{{ visitor.tanggal }},{{ visitor.waktu }}</td>
              <td>{{ visitor.keperluan.nama }}</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
  <div class="d-flex justify-content-end">
    <nuxt-link to="/" class="btn btn-light btn-lg rounded-4 px-4 ms-auto">KEMBALI</nuxt-link>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient();

const keyword = ref([]);

const visitors = ref([]);

const banyak = ref([]);

const getPengunjung = async () => {
  const { data, error } = await supabase.from("pengunjung").select(`*,keanggotaan(*),keperluan(*)`).ilike("nama", `%${keyword.value}%`).order("id", { ascending: false });
  if (data) visitors.value = data;
};

const banyakPengunjung = async () => {
  const { data, count } = await supabase.from("pengunjung").select(`*`, { count: "exact" });
  if (data) banyak.value = count;
};

onMounted(() => {
  getPengunjung();
  banyakPengunjung();
});
</script>

<style scoped>
.btn-light {
  background-color: #5fd8fe !important;
  box-shadow: 1px 1px 10px #5fd8fe !important;
}
</style>
