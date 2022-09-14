<script setup>
import { ref } from 'vue';

const isSearch = ref(false)
const searchWord = ref('')
</script>
 
<template>
    <div>
        <div class="navbar bg-base-200 fixed z-10 hidden md:block shadow-2xl">
            <div class="flex ml-20">
                <div class="flex-none">
                    <button @click="isSearch = !isSearch" class="btn btn-ghost btn-circle">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                        </svg>
                        <span class="badge badge-xs badge-primary indicator-item"></span>
                    </button>
                    <input v-if="isSearch" type="text" placeholder="Type" class="input input-bordered input-sm ml-2"
                        v-model="searchWord">
                </div>

                <div class="flex-1">
                    <a v-if="!isSearch" class="btn btn-ghost normal-case text-xl" href="">Portfolio | Jirasin</a>
                </div>

                <div class="justify-end mr-20">
                    <a class="btn btn-ghost" href="#about_web">About web</a>
                    <a class="btn btn-ghost" href="#oasip">OASIP</a>
                    <a class="btn btn-ghost" href="#modx">ModX-Change</a>
                    <a class="btn btn-ghost" href="#contact">Contact</a>
                </div>
            </div>
        </div>

        <div class="md:hidden navbar bg-base-100 fixed z-10 shadow-2xl">
            <div class="navbar-start">
                <div class="dropdown">
                    <label tabindex="0" class="btn btn-ghost btn-circle">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M4 6h16M4 12h16M4 18h7" />
                        </svg>
                    </label>
                    <ul tabindex="0"
                        class="menu menu-compact dropdown-content mt-3 p-2 shadow bg-base-100 rounded-box w-52">
                        <li><a href="#about_web">About web</a></li>
                        <li><a href="#oasip">OASIP</a></li>
                        <li><a href="#modx">ModX-Change</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
            </div>
            <div class="navbar-center">
                <input v-if="isSearch" type="text" placeholder="Type" class="input input-bordered input-sm"
                    v-model="searchWord">
                <a v-else class="btn btn-ghost normal-case text-xl" href="">Portfolio | Jirasin</a>
            </div>
            <div class="navbar-end">
                <button class="btn btn-ghost btn-circle" @click="isSearch = !isSearch">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                        stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                    </svg>
                    <span class="badge badge-xs badge-primary indicator-item"></span>
                </button>
            </div>
        </div>
    </div>
</template>
 
<style>

</style>