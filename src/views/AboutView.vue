<script setup>
import Footer from '../components/FooterComponent.vue'
import Nav from '../components/NavComponent.vue'
import Profile from '../components/ProfileComponent.vue'
</script>

<template>
    <Nav />

    <main class="bg-white dark:bg-gray-900">
        <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-8">
            <h1
                class="mb-4 text-4xl font-extrabold leading-none tracking-tight text-gray-900 md:text-5xl lg:text-6xl dark:text-white">
                About <span class="text-blue-600 dark:text-blue-500">Hall of Codes</span>.</h1>
            <p class="text-lg font-normal text-gray-500 lg:text-xl dark:text-gray-400">Here at Hall of Codes we share our
                passion for coding and fostering collaboration among developers worldwide. Discover our journey, mission,
                and commitment to advancing coding knowledge and skills in an inclusive and supportive environment.</p>

            <div class="mt-10 grid md:grid-cols-3 gap-8">

                <Profile :profilePhoto="mrepol742">
                    <template #position>Founder</template>
                    <template #name>Melvin Jones Gallano Repol</template>
                    <template #bio>Freelance Software & Web Developer</template>
                </Profile>

                <Profile :profilePhoto="samiunnafis">
                    <template #position>Co-Founder</template>
                    <template #name>Samiun Nafis</template>
                    <template #bio>Sussy baka. UwU</template>
                </Profile>
            </div>

            <div role="status"
                class="mt-10 space-y-8 animate-pulse md:space-y-0 md:space-x-8 rtl:space-x-reverse md:flex md:items-center">
                <div class="flex items-center justify-center w-full h-48 bg-gray-300 rounded sm:w-96 dark:bg-gray-700">
                    <svg class="w-10 h-10 text-gray-200 dark:text-gray-600" aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 18">
                        <path
                            d="M18 0H2a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2Zm-5.5 4a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3Zm4.376 10.481A1 1 0 0 1 16 15H4a1 1 0 0 1-.895-1.447l3.5-7A1 1 0 0 1 7.468 6a.965.965 0 0 1 .9.5l2.775 4.757 1.546-1.887a1 1 0 0 1 1.618.1l2.541 4a1 1 0 0 1 .028 1.011Z" />
                    </svg>
                </div>
                <div class="w-full">
                    <div class="h-2.5 bg-gray-200 rounded-full dark:bg-gray-700 w-48 mb-4"></div>
                    <div class="h-2 bg-gray-200 rounded-full dark:bg-gray-700 max-w-[480px] mb-2.5"></div>
                    <div class="h-2 bg-gray-200 rounded-full dark:bg-gray-700 mb-2.5"></div>
                    <div class="h-2 bg-gray-200 rounded-full dark:bg-gray-700 max-w-[440px] mb-2.5"></div>
                    <div class="h-2 bg-gray-200 rounded-full dark:bg-gray-700 max-w-[460px] mb-2.5"></div>
                    <div class="h-2 bg-gray-200 rounded-full dark:bg-gray-700 max-w-[360px]"></div>
                </div>
                <span class="sr-only">Loading...</span>
            </div>

        </div>
    </main>
    <Footer />
</template>
<script>
export default {
  components: {
    Profile
  },
  data() {
    return {
      mrepol742: 'https://avatars.githubusercontent.com/u/62317165?v=4',
      samiunnafis: 'https://avatars.githubusercontent.com/u/56390452?v=4'
    };
  }
};
</script>