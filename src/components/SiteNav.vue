<template>
    <header>
        <nav class="fixed w-full text-white mx-0 px-3 z-50">
            <div class="flex flex-row items-center justify-between font-Plus drop-shadow-xl text-3xl">
                <div class="bg-black rounded-full p-3 w-16 text-center text-4xl cursor-pointer transition-all duration-500 active:text-black">
                    <div v-if=showMenu>
                        <font-awesome-icon icon="fa-bars"  @click="$emit('menuToggle')" class="hover:text-green-300" />
                    </div>
                    <div v-else>
                        <font-awesome-icon icon="fa-xmark" @click="$emit('menuToggle')" class="hover:text-red-400"  />
                    </div>
                </div>
                <div v-show="showMenu">
                    <h3 class="hidden bg-black font-light rounded-full p-3 text-3xl tracking-wider transition-all duration-500 sm:block md:tracking-widest">
                        architecture<Featured />
                    </h3>
                </div>
                <router-link to="/">
                    <div class="bg-black rounded-full p-3">
                        <p class="text-6xl font-light text-black bg-white rounded-full px-3 py-7 transition-all duration-500 hover:bg-green-300">W2</p>
                    </div>
                </router-link>
                <div v-show="showMenu">
                    <h3 class="hidden bg-black font-light rounded-full py-3 px-4 text-3xl tracking-wider transition-all duration-500 sm:block md:tracking-widest">
                        engineering
                    </h3>
                </div>
                <router-link to="/about">
                    <div class="bg-black rounded-full p-4 text-4xl transition-all duration-500 hover:text-green-300">
                        <font-awesome-icon icon="fa-regular fa-address-card" />
                    </div>
                </router-link>
            </div>
        </nav>
    </header>
</template>

<script>

export default {
    name: "SiteNav",
    props: {
        showMenu: Boolean
    }
}

</script>