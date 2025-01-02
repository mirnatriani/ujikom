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
    <h2 class="text-center pt-3">Ekstrakurikuler</h2>
    <div class="row flex justify-content-center">
      <div v-for="(eskul, i) in cover" :key="i" class="col-lg-3">
        <div class="card mb-5" style="width: 18rem">
          <img :src="eskul.poto" class="card-img-top" alt="..." />
          <div class="card-body">
            <h5 class="card-title">{{ eskul.nama }}</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "Ekstrakurikuler Page",
  meta: [
    {
      name: "description",
      content: "Ekstrakurikuler Page",
    },
  ],
});
const supabase = useSupabaseClient();

const cover = ref([]);

const getCover = async () => {
  const { data } = await supabase.from("eskul").select("*");
  if (data) cover.value = data;
};

onMounted(() => {
  getCover();
});
</script> -->
