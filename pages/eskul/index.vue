<template>
  <div class="container pb-5">
    <h2 class="text-center pt-3">Ekstrakurikuler</h2>
    <div class="row flex justify-content-center">
      <div class="col-lg-3">
        <div class="card" style="width: 18rem">
          <img src="/assets/img/laskar.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <p class="card-text">Laskar Pustaka</p>
            <p>
              Meningkatkan minat baca dan pengelolaan perpustakaan untuk
              mendukung literasi siswa.
            </p>
          </div>
        </div>
      </div>
      <div class="col-lg-3">
        <div class="card" style="width: 18rem">
          <img src="/assets/img/pmr.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <p class="card-text">Palang Merah Remaja</p>
            <p>
              Melatih siswa untuk siap siaga dalam memberikan pertolongan
              pertama dan kegiatan kemanusiaan.
            </p>
          </div>
        </div>
      </div>
      <div class="col-lg-3">
        <div class="card" style="width: 18rem">
          <img src="/assets/img/pks.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <p class="card-text">Patroli Keamanan Sekolah</p>
            <p>
              Menanamkan disiplin dan tanggung jawab untuk menjaga ketertiban di
              lingkungan sekolah.
            </p>
          </div>
        </div>
      </div>
      <div class="col-lg-3">
        <div class="card" style="width: 18rem">
          <img src="/assets/img/pd.jpg" class="card-img-top" alt="..." />
          <div class="card-body">
            <p class="card-text">Perisai Diri</p>
            <p>
              Ekstrakurikuler seni bela diri tradisional untuk melatih fisik dan
              mental sekaligus menjaga warisan budaya.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient();

const cover = ref([]);

const getCover = async () => {
  const { data } = await supabase.from("eskul").select('*');
  if (data) cover.value = data;
};

onMounted(() => {
  getCover();
})
</script>
