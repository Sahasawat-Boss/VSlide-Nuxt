<template>
    <Nav />
    <div class="relative h-screen w-full bg-cover bg-center text-white"
        style="background-image: url('/images/book2/img9.jpg')">
        <!-- Overlay -->
        <div class="absolute inset-0 bg-black/35 backdrop-blur-[6px]"></div>

        <!-- Centered content -->
        <div class="relative z-10 flex flex-col items-center justify-center h-full text-center px-4 fade-in">
            <h1 class="text-3xl md:text-4xl font-semibold hover" style="text-shadow: 2px 3.5px 6px rgba(0,0,0,0.6);">
                Book 2</h1>
            <div class="mt-1.5 flex md:text-xl font-bold font-serif opacity-50">
                <AnFilledLock class="text-lg m-1 text-yellow-400" />
                <p class="text-yellow-300">Locked</p>
            </div>
            <p class="mt-8 text-base md:text-xl italic max-w-lg tracking-wider">
                Book 2 is exclusive to subscribers.
            </p>
            <p class="font-bold text-xl mt-14">Consider Subscription?</p>

            <!-- Contact Link -->
            <a href="https://bossbsynth.com" target="_blank"
                class="text-white text-lg my-3underline underline-offset-4 hover:text-blue-300 mb-14">
                <div class="flex hover">
                    <span class="text-blue-400 ">Contact: bossbsynth.com</span>
                    <span class="float-x mt-1.5 ml-1 text-xl text-blue-400">
                        <FlFilledCallOutbound />
                    </span>
                </div>
            </a>

            <NuxtLink to="/"
                class="bg-white/20 px-4 py-1 rounded-lg text-white text-base hover:bg-white/40  fade-in-up2">
                ⟵ Back to Menu
            </NuxtLink>

            <!-- bossbsynth.com - External Link -->
            <a href="https://bossbsynth.com/"
                class="fixed bottom-5 text-xs md:text-sm text-white/65 hover italic mt-1 fade-in"
                style="text-shadow: 2px 3px 7px rgba(0,0,0,0.6);">
                bossbsynth.com
            </a>
        </div>
    </div>
</template>

<script setup>
import { Nav } from "#components";
import { FlFilledCallOutbound, AnFilledLock } from '@kalimahapps/vue-icons';
</script>