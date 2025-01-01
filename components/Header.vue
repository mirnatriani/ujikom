<template>
  <nav class="navbar navbar-expand-lg bg-primary sticky-top">
    <div class="container-fluid">
      <div class="navbar-brand ms-5">
        <img
          src="~/assets/img/logo.png"
          alt="Logo"
          width="50"
          class="d-inline-block align-text-top"
        />
      </div>
      <div class="col-lg-2 text-white">SMKN 4 TASIKMALAYA</div>
      <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button> -->
      <div
        class="justify-content-end me-5 collapse navbar-collapse"
        id="navbarNavDropdown"
      >
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/">Beranda</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/profil">Profil</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/galeri">Galeri</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/eskul">Ekstrakurikuler</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/kontak">Kontak</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
useHead({
  title: "Beranda Page",
  meta: [
    {
      name: "description",
      content: "Beranda Page",
    },
  ],
});
</script>
