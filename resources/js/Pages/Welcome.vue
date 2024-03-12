<script setup>
import { Head, Link } from '@inertiajs/vue3';
import PublicLayout from '@/Layouts/PublicLayout.vue';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: String,
    phpVersion: String,
});
</script>

<template>
    <PublicLayout title="Homepage">
        <div data-bs-spy="scroll" data-bs-target="homenav" data-bs-smooth-scroll="true">
            <div id="homepage" class="header-2 section-home">
                <div class="page-header min-vh-75 relative">
                    <div class="container">
                        <div class="row align-items-center justify-content-between">
                            <div class="col col-lg-6">
                                <h2>Welcome to MinaDev</h2>
                                <p>Your premier destination for cutting-edge web application development! At MinaDev, we are dedicated to elevating your digital presence through innovative and customized web solutions. As specialists in web application development, we bring a wealth of expertise to the table, ensuring your business stands out in the ever-evolving online landscape.</p>
                            </div>
                            <div class="col-auto">
                                <img src="assets/img/web-design.png" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div id="about" class="section-about py-5 min-vh-75 d-flex align-items-center">
                <span class="imgbg-repeat" style="background-image: url('assets/img/bluedots.jpg');"></span>
                <div class="container">
                    <div class="row align-items-center justify-content-between">
                        <div class="col-auto">
                            <img src="assets/img/ab-test.png" />
                        </div>
                        <div class="col col-lg-6 text-center">
                            <h2>About MinaDev</h2>
                            <p>MinaDev is more than just a developer; we're your strategic partner in harnessing the full potential of the web. Whether you're launching a new project, revamping an existing platform, or seeking seamless integrations, our team of skilled developers is committed to delivering solutions that exceed your expectations.</p>
                            <p>Why choose MinaDev for your web application needs? Our approach is rooted in collaboration, creativity, and a deep understanding of your unique requirements. We take pride in crafting user-friendly, scalable, and robust web applications that not only meet industry standards but also set new benchmarks for excellence.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div id="service" class="section-service py-5 min-vh-75 d-flex align-items-center">
                <div class="container">
                    <div class="row align-items-center justify-content-between">
                        <div class="col col-lg-6">
                            <h2>Our Services</h2>
                            <p>We have several services to be your one stop web application development.</p>
                            <ul class="list-group">
                                <li class="list-group-item">
                                    <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                    Fully Customized Web Application
                                </li>
                                <li class="list-group-item">
                                    <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                    Wordpress Development
                                </li>
                                <li class="list-group-item">
                                    <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                    Laravel App Development
                                </li>
                                <li class="list-group-item">
                                    <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                    Web & Server Maintenance
                                </li>
                                <li class="list-group-item">
                                    <i class="material-icons opacity-6 me-2 text-md">thumb_up</i>
                                    Web Deployment
                                </li>
                            </ul>
                        </div>
                        <div class="col-auto">
                            <img src="assets/img/full-stack.png" />
                        </div>
                    </div>
                </div>
            </div>
            <div id="contact" class="section-contact py-5 min-vh-75 d-flex align-items-center">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-7 mx-auto">
                            <h2 class="text-center mb-4">Contact Us</h2>
                            <form>
                                <div class="input-group input-group-outline mb-3">
                                    <label class="form-label" for="fullname">Full Name *</label>
                                    <input type="text" class="form-control" id="fullname">
                                </div>
                                <div class="input-group input-group-outline mb-3">
                                    <label class="form-label" for="email">Email *</label>
                                    <input type="email" class="form-control" id="email">
                                </div>
                                <div class="input-group input-group-outline mb-3">
                                    <label class="form-label" for="phone">Phone No.</label>
                                    <input type="text" class="form-control" id="phone">
                                </div>
                                <div class="input-group input-group-static mb-3">
                                    <label for="message">Message *</label>
                                    <textarea class="form-control" id="message"></textarea>
                                </div>
                                <button type="submit" class="btn btn-outline-info mb-0">Submit</button>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </PublicLayout>
</template>

