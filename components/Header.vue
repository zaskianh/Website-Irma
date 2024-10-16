<template>
    <nav class="navbar navbar-expand-lg bg-success">
        <div class="container">
            <img src="/assets/img/Logo_Smk.jpg" alt="logo irma" width="100px" height="100px">
            <img src="/assets/img/Logo_Irma.jpg" alt="logo smk" width="100px" height="100px">
            <a class="navbar-brand" href="#">IRMA SMKN4 TASIKMALAYA</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'index' }" to="/">Beranda</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'irma' }" to="/irma">Irma</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'profil-irma' }" to="/profil-irma">Profil</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'anggota' }" to="/anggota">Anggota</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'kegiatan' }" to="/kegiatan">Kegiatan</NuxtLink>
                    </li>
                    <li class="nav-item">
                        <NuxtLink class="nav-link" :class="{ active: route.name == 'dokumentasi' }" to="/dokumentasi">Dokumentasi</NuxtLink>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script setup>
const route = useRoute()

console.log(route.name)
</script>