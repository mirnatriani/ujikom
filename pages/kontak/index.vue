<template>
  <div class="container pt-5 pb-5">
    <div class="row">
      <form>
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label">Nama</label>
          <input
            type="email"
            class="form-control"
            id="exampleInputEmail1"
            aria-describedby="emailHelp"
          />
          <div id="emailHelp" class="form-text"></div>
        </div>
        <div class="mb-3">
          <label for="exampleInputPassword1" class="form-label">Email</label>
          <input
            type="password"
            class="form-control"
            id="exampleInputPassword1"
          />
        </div>
        <div class="mb-3">
          <label for="exampleInputPassword1" class="form-label">Pesan</label>
          <input
            type="password"
            class="form-control"
            id="exampleInputPassword1"
          />
        </div>
        <button type="submit" class="btn btn-primary">Kirim Pesan</button>
      </form>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "Kontak Page",
  meta: [
    {
      name: "description",
      content: "Kontak Page",
    },
  ],
});
</script>

<!-- <template>
  <div class="container pb-5">
    <h2 class="text-center">Galeri</h2>
    <div class="row">
      <div v-for="(data, i) in galeri" :key="i" class="col-lg-3 pt-3">
        <div class="card" style="width: 18rem">
          <img :src="data.poto" class="card-img-top" alt="..." />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "Galeri Page",
  meta: [
    {
      name: "description",
      content: "Galeri Page",
    },
  ],
});
const supabase = useSupabaseClient();

const galeri = ref([]);

const getData = async () => {
  const { data, error } = await supabase.from("galeri").select(`*`);
  if (data) galeri.value = data;
};

onMounted(() => {
  getData();
});
</script> -->
