<template>
  <div class="container pb-5">
    <h2 class="text-center">Galeri</h2>
    <div class="row">
      <div v-for="(data, i) in galeri" :key="i" class="col-lg-3">
        <div class="card" style="width: 18rem">
          <img :src="data.poto" class="card-img-top" alt="..." />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const supabase = useSupabaseClient();

const galeri = ref([]);

const getData = async () => {
  const { data, error } = await supabase.from("galeri").select(`*`);
  if (data) galeri.value = data;
};

onMounted(() => {
  getData();
});
</script>
