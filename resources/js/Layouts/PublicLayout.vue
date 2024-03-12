<script setup>
import { ref } from 'vue';
import { Head, Link, router } from '@inertiajs/vue3';
import ApplicationMark from '@/Components/ApplicationMark.vue';
import Banner from '@/Components/Banner.vue';
import Dropdown from '@/Components/Dropdown.vue';
import DropdownLink from '@/Components/DropdownLink.vue';
import NavLink from '@/Components/NavLink.vue';
import ResponsiveNavLink from '@/Components/ResponsiveNavLink.vue';

defineProps({
    title: String,
});

const showingNavigationDropdown = ref(false);
</script>

<template>
    <div>
        <Head :title="title" />

        <div class="container position-sticky z-index-sticky top-0">
            <div class="row">
                <div class="col-12">
                    <nav id="homenav" class="navbar navbar-expand-lg  blur border-radius-xl top-0 z-index-fixed shadow position-absolute my-3 py-2 start-0 end-0 mx-4">
                        <div class="container-fluid px-0">
                            <a class="navbar-brand font-weight-bolder ms-sm-3" href="#">MinaDev</a>
                            <button class="navbar-toggler shadow-none ms-2" type="button" data-bs-toggle="collapse" data-bs-target="#navigation" aria-controls="navigation" aria-expanded="false" aria-label="Toggle navigation">
                                <span class="navbar-toggler-icon mt-2">
                                    <span class="navbar-toggler-bar bar1"></span>
                                    <span class="navbar-toggler-bar bar2"></span>
                                    <span class="navbar-toggler-bar bar3"></span>
                                </span>
                            </button>
                            <div class="collapse navbar-collapse pt-3 pb-2 py-lg-0 w-100" id="navigation">
                                <ul class="navbar-nav navbar-nav-hover ms-auto">
                                    <li class="nav-item mx-2">
                                        <a href="#homepage" class="nav-link ps-2 d-flex cursor-pointer align-items-center">
                                            <i class="material-icons opacity-6 me-2 text-md">home</i>
                                            Home
                                        </a>
                                    </li>
                                    <li class="nav-item mx-2">
                                        <a href="#about" class="nav-link ps-2 d-flex cursor-pointer align-items-center">
                                            <i class="material-icons opacity-6 me-2 text-md">info</i>
                                            About
                                        </a>
                                    </li>
                                    <li class="nav-item mx-2">
                                        <a href="#service" class="nav-link ps-2 d-flex cursor-pointer align-items-center">
                                            <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                            Our Services
                                        </a>
                                    </li>
                                    <li class="nav-item mx-2">
                                        <a href="#contact" class="nav-link ps-2 d-flex cursor-pointer align-items-center">
                                            <i class="material-icons opacity-6 me-2 text-md">contact_mail</i>
                                            Reach Us
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </nav>
                    <!-- End Navbar -->
                </div>
            </div>
        </div>

        <main>
            <slot />
        </main>

        <div class="footer py-3">
            <div class="container">
                <div class="row align-items-center justify-content-between">
                    <div class="col text-center">
                        &copy; MinaDev {{ new Date().getFullYear() }}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
