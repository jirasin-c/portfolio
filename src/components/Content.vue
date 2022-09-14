<script setup>
import { ref } from 'vue';

const workList = ref([
    {
        name: `Online Appointment Scheduling System for Integrated Project Clinics
                                (OASIP)`,
        detail: `This web-application is about scheduling appointments, it is part of
                                the INT 222
                                course.
                                The
                                website uses
                                RESTful APIs and CRUD system and is in developing present.`,
        link: `https://intproj21.sit.kmutt.ac.th/ssi3/`,
        img: "./OASIP.gif",
        id: "oasip"
    },
    {
        name: `ModX-Change`,
        detail: `This web-application is about Currency Converter Exchange Rates, it is
                                part of the
                                INT 203
                                course.
                                The
                                website uses
                                a mockup exchange rates for development.`,
        link: `https://cranky-heyrovsky-613c9f.netlify.app/`,
        img: "./DARKLIGHTMODE.gif",
        id: "modx"
    },
])

const firstBgColor = ref('hero min-h-screen bg-base-200 drop-shadow-xl')
const secondBgColor = ref('hero min-h-screen bg-base-300')
</script>
     
<template>
    <div class="h-full w-full">
        <div class="hero min-h-screen bg-base-200 drop-shadow-xl">
            <div class="hero-content flex-col lg:flex-row-reverse ">
                <img data-aos="fade-left" data-aos-duration="1000" src="../assets/jirasin-profile.jpg"
                    class="max-w-sm rounded-lg shadow-xl md:w-full md:h-full w-full h-full mt-20 hover:shadow-2xl " />
                <div data-aos="fade" data-aos-duration="2000">
                    <h1 class="text-5xl font-bold px-3">Hi, I am Jiras<span class="text-primary">in.</span> </h1>
                    <p class="py-6 px-3">Passionate about doing the <span class="text-secondary font-bold">front-end
                            developer</span> because
                        when
                        it
                        is the time to do
                        this part,
                        felt it was a challenge and so confident that will accomplish it, although encountered some
                        problems while
                        working. I am currently third-year undergraduate student in Information Technology from King
                        Mongkut's
                        University of Technology Thonburi (KMUTT). </p>

                </div>
            </div>
        </div>
        <div class="hero min-h-screen bg-base-300" id="about_web">
            <div class="hero-content flex-col">
                <a href="https://vuejs.org/" target="_blank"><img src="../assets/vue.png" alt="" data-aos="fade-up"
                        data-aos-duration="1000"></a>
                <a href="https://daisyui.com/" target="_blank"><img src="../assets/daisyUi.svg" alt="" class="pb-10"
                        data-aos="fade-up" data-aos-duration="1500"></a>

                <div data-aos="fade-up" data-aos-duration="2000">
                    <h1 class="text-5xl font-bold px-3 md:px-24">About this web</h1>
                    <p class="py-6 px-3 md:px-24">This website was created to collect the work that I did when I was a
                        university
                        student,
                        known as a portfolio. It shows my abilities and interests. The frameworks and library that I
                        using to
                        create
                        this website and the work of portfolio is <span class="text-emerald-600 font-bold">VueJS</span>
                        and <span class="text-primary font-bold">daisy</span><span class="font-bold">UI</span> CSS. </p>
                </div>
            </div>
        </div>
        <div v-for="work,index in workList" :key="index">
            <div :class="[index % 2 == 0 ? firstBgColor: secondBgColor]" :id="work.id">
                <div class="hero-content text-center">
                    <div v-if="index % 2 == 0">
                        <div class="card lg:card-side bg-base-100 shadow-xl">
                            <a :href="work.link" target="_blank">
                                <figure data-aos="fade-in" data-aos-duration="2000"><img :src="work.img" alt="Album"
                                        class="h-full md:h-96"></figure>
                            </a>
                            <div class="card-body" data-aos="slide-up" data-aos-duration="1500">
                                <h2 class="card-title">{{work.name}}</h2>
                                <p class="py-3 md:py-10">{{work.detail}}</p>
                                <div class="card-actions justify-end">
                                    <a :href="work.link" target="_blank" rel="noopener noreferrer"
                                        class="btn btn-primary">Go
                                        to website</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div v-else>
                        <div class="card lg:card-side bg-base-100 shadow-xl">
                            <div class="card-body" data-aos="slide-down" data-aos-duration="1500">
                                <h2 class="card-title">{{work.name}}</h2>
                                <p class="py-3 md:py-10">{{work.detail}}</p>
                                <div class="card-actions justify-start">
                                    <a :href="work.link" target="_blank" rel="noopener noreferrer"
                                        class="btn btn-primary">Go
                                        to website</a>
                                </div>
                            </div>
                            <a :href="work.link" target="_blank">
                                <figure data-aos="fade-in" data-aos-duration="2000"><img :src="work.img" alt="Album"
                                        class="h-full md:h-96"></figure>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
     
<style>

</style>