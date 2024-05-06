<script setup>
import { onMounted, ref } from 'vue';
import AOS from 'aos'
import 'aos/dist/aos.css'
const workList = ref([
    {
        name: `Health Movement Campaign System for Active Living (Mod Campaign)`,
        detail: `Mobile-App and Web-App to promote physical activity and healthy living within a university community. It tackles the challenge of sedentary lifestyles among students and staff by offering a gamified system for exercise, progress tracking. `,
        link: `https://capstone23.sit.kmutt.ac.th/tt1/`,
        img: "/src/assets/modcampaign.png",
        id: "modcampaign"
    },
    {
        name: `Online Appointment Scheduling System for Integrated Project Clinics
                                (OASIP)`,
        detail: `This web-application is about scheduling appointments, it is part of
                                the INT 222
                                course.
                                The
                                website uses
                                RESTful APIs and CRUD system`,
        link: `https://intproj21.sit.kmutt.ac.th/ssi3/`,
        img: "/src/assets/OASIP.gif",
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
        img: "/src/assets/DARKLIGHTMODE.gif",
        id: "modx"
    },
    {
        name: `Kashino-125`,
        detail: `This web-application is a cards game, it is
                                part of the
                                INT 203
                                course.
                                The
                                website uses
                                JSON-Server that is a RESTful APIs mockup for development.`,
        link: `https://kashino-125.netlify.app/`,
        img: "/src/assets/kashino.gif",
        id: "kashino"
    },
])
onMounted(() => {
    AOS.init({
        once: false
    })
})
</script>

<template>
    <div class="h-full w-full">
        <div class="hero min-h-screen bg-base-200 drop-shadow-xl">
            <div class="hero-content flex-col lg:flex-row-reverse space-y-10">
                <img data-aos="fade-left" data-aos-duration="1000" src="../assets/jirasin-profile.jpg"
                    class="max-w-sm rounded-xl shadow-xl md:w-full md:h-full w-full h-full mt-20 lg:mt-0 hover:shadow-2xl " />
                <div data-aos="fade" data-aos-duration="2000" class="mr-0 lg:mr-20">
                    <h1 class="text-5xl font-bold px-3">Hi, I am Jiras<span class="text-primary">in.</span> </h1>
                    <p class="py-6 px-3">Passionate about doing the <span class="text-secondary font-bold">full-stack
                            developer</span> because
                        I have
                        seen it was a challenge when doing all this part and I’m confident that would accomplish it,
                        although encountered some problems while working. I am currently fourth-year undergraduate
                        student in
                        Information Technology from King
                        Mongkut's
                        University of Technology Thonburi (KMUTT). </p>

                </div>
            </div>
        </div>
        <div class="w-full h-full flex items-center justify-center bg-base-300 px-8 lg:px-52 py-20 lg:py-52"
            id="about_web">
            <div class="flex flex-col space-y-24">

                <div data-aos="fade-up" data-aos-duration="1000">
                    <h1 class="text-5xl font-bold px-3 md:px-24">About this website</h1>
                    <p class="py-6 px-3 md:px-24">This website is about my journey as a developer, where each project is
                        a brushstroke painting the picture of my skills and passion for crafting digital experiences and
                        it created to collect the work that I did when I was a
                        university
                        student,
                        known as a portfolio. It shows my abilities and interests.</p>
                </div>
                <div class="flex flex-col space-y-10" data-aos="fade-up" data-aos-duration="1500">
                    <h1 class="text-5xl font-bold px-3 md:px-24">Framework skills</h1>
                    <div class="flex flex-row w-full h-full justify-center">
                        <div
                            class="flex flex-row flex-wrap space-x-2 space-y-4 lg:space-x-4 bg-base-200 w-full mx-0 lg:mx-52 p-10 rounded-3xl justify-center items-center">
                            <img src="/src/assets/react-2.svg" class="w-32 h-32" alt="">
                            <img src="/src/assets/react-native-1.svg" class="w-32 h-32" alt="">
                            <img src="/src/assets/nuxtLogo.svg" class="w-56 h-32" alt="">
                            <img src="/src/assets/vue.png" class="w-56 h-32" alt="">
                            <img src="/src/assets/ExpressJs-logo.png" class="w-96 h-28" alt="">
                            <img src="/src/assets/springio-ar21.svg" class="w-60 h-28" alt="">
                        </div>

                    </div>
                </div>
                <!-- <div class="flex flex-col space-y-10">
                    <h1 class="text-5xl font-bold px-3 md:px-24" data-aos="fade-up" data-aos-duration="1500">Framework
                        Skills</h1>
                    <div class="flex flex-row px-28 w-full h-full justify-center" data-aos="fade-up"
                        data-aos-duration="2000">
                        <div
                            class="flex flex-row flex-wrap space-x-4 space-y-4 lg:space-x-4 bg-base-200 w-full mx-0 lg:mx-24 p-10 rounded-3xl justify-center items-center">
                            <img src="/src/assets/react-2.svg" class="w-32 h-32" alt="">
                            <img src="/src/assets/react-native-1.svg" class="w-32 h-32" alt="">
                            <img src="/src/assets/nuxtLogo.svg" class="w-32 h-32" alt="">
                            <img src="/src/assets/vue.png" class="w-56 h-32" alt="">
                            <img src="/src/assets/ExpressJs-logo.png" class="w-96 h-28" alt="">
                            <img src="/src/assets/springio-ar21.svg" class="w-60 h-28" alt="">
                        </div>
                    </div>
                </div> -->
            </div>
        </div>
        <div class="w-full h-full py-20 bg-base-200 drop-shadow-xl flex items-center">
            <div class="w-full flex-col space-y-10 flex items-center h-full justify-center px-8 lg:px-20">
                <h1 class="text-5xl font-bold px-3" data-aos="fade-up" data-aos-duration="1000">My Works</h1>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10 w-full h-full" data-aos="fade-in"
                    data-aos-duration="2000">
                    <div v-for="work, index in workList" :key="index" class="w-full h-full">
                        <div data-aos="fade-up" data-aos-duration="1500"
                            class="bg-base-100 shadow-xl w-full h-full rounded-xl flex-col relative">
                            <img :src="work.img" alt="Album" class="w-full h-[320px] rounded-tl-lg rounded-tr-lg">
                            <div class="p-4 flex flex-col justify-between space-y-8 h-[350px] lg:h-[280px]">
                                <div class="w-full h-full">
                                    <h2 class="card-title">{{ work.name }}</h2>
                                    <p class="py-3">{{ work.detail }}</p>
                                </div>
                                <div class="card-actions absolute z-50 bottom-3 right-3">
                                    <a :href="work.link" target="_blank" rel="noopener noreferrer"
                                        class="btn btn-primary">More Detail</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style></style>