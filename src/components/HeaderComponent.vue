<template>
    <div>
        <div class="flex items-center justify-between py-[1rem] px-4 md:px-[6rem]">
            <!--Brand Logo starts here -->
            <div>
                <h1 class="text-xl font-bold font-signika text-orange-400">Ape<span class="text-orange-600">x</span></h1>
            </div>
            <!--Brand Logo ends here-->
            <!--router link starts here-->
            <div class="md:flex space-x-6 capitalize  hidden">
                <div>
                    <a href="">demos</a>
                </div>
                <div>
                    <a href="">About</a>
                </div>
                <div>
                    <a href="">Blog</a>
                </div>
                <div>
                    <a href="">Pages</a>
                </div>
                <div>
                    <a href="">Contacts</a>
                </div>
            </div>
            <!--router link ends here-->
            <div>
                <div class="md:flex hidden space-x-4 items-center">
                    <a href="">Login</a>
                    <a href="" class="bg-orange-400 rounded-sm shadow-sm shadow-orange-300 text-sm capitalize text-white px-4 py-2">Get started free</a>
                </div>
            </div>
            <div class="md:hidden block" @click="showSidebar">
                <span class="las la-bars text-xl font-extrabold" v-if="!navBarShouldShow"></span>
                <span v-else  class="las la-times text-xl font-extrabold"></span>
            </div>
        </div>
        <div v-if="navBarShouldShow" class="bg-white w-full animate-fade-in-down py-[2rem] shadow-sm shadow-orange-200 relative block md:hidden">
            <div class="divide-y px-[1rem]">
                <div class="py-4 text-lg font-bold">
                    <a href="">Demos</a>
                </div>
                <div class="py-4 text-lg font-bold">
                    <a href="">About</a>
                </div>
                <div class="py-4 text-lg font-bold">
                    <a href="">Blog</a>
                </div>
                <div class="py-4 text-lg font-bold">
                    <a href="">Pages</a>
                </div>
                <div class="">
                <div class="py-4 text-lg font-bold">
                    <a href="">Login</a>
                </div>
                
            </div>
            <div class="py-4 text-lg w-full font-bold">
                    <a href="">
                        <div class="w-full bg-orange-500 text-center text-white py-4 rounded-xl">
                            Get started for free
                        </div>
                    </a>
                </div>
            </div>
            
        </div>
    </div>
</template>

<script setup>
import {ref} from 'vue'

const navBarShouldShow = ref(false);

function showSidebar() {
    navBarShouldShow.value = !navBarShouldShow.value
}

</script>

<style scoped>

</style>
