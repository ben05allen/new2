<template>
    <header>
        <nav class="fixed w-full text-white mx-0 px-3 z-50">
            <div class="flex flex-row items-center justify-between font-Plus drop-shadow-xl text-3xl">
                <div class="bg-black rounded-full p-3 w-16 text-center text-4xl cursor-pointer transition-all duration-500 active:text-black">
                    <div v-if=showMenu>
                        <svg height="48" width="48" @click="$emit('menuToggle')" class="fill-white hover:fill-slate-200"><path d="m 7.2957811,34.853101 0.015931,-0.902857 33.3306065,-0.02415 0.04803,0.881867 z M 7.3,25.007148 l -0.033582,-1.074589 33.4495245,-0.01921 -0.0018,1.058029 z M 7.3,15 V 13.9 H 40.7 V 15 Z"/></svg>
                    </div>
                    <div v-else>
                        <svg height="48" width="48" @click="$emit('menuToggle')" class="fill-white hover:fill-red-200 bg-gray-900 rounded-xl"><path d="m12.7 36.1-.8-.8L23.2 24 11.9 12.7l.8-.8L24 23.2l11.3-11.3.8.8L24.8 24l11.3 11.3-.8.8L24 24.8Z"/></svg>
                    </div>
                </div>
                <div v-show="showMenu">
                    <h3 class="hidden bg-black font-light rounded-full p-3 text-3xl tracking-wider transition-all duration-500 sm:block md:tracking-widest">
                        architecture<Featured />
                    </h3>
                </div>
                <router-link to="/">
                    <div class="bg-black rounded-full p-3">
                        <p class="text-6xl font-light text-black bg-white rounded-full px-3 py-7 transition-all duration-500 hover:bg-slate-200">W2</p>
                    </div>
                </router-link>
                <div v-show="showMenu">
                    <h3 class="hidden bg-black font-light rounded-full py-3 px-4 text-3xl tracking-wider transition-all duration-500 sm:block md:tracking-widest">
                        engineering
                    </h3>
                </div>
                <router-link to="/about">
                    <div class="bg-black rounded-full p-4 text-4xl transition-all duration-500">
                        <svg height="48" width="48" class="fill-white hover:fill-slate-200"><path d="M9.3 37.4q-1.15 0-1.925-.775Q6.6 35.85 6.6 34.7V13.3q0-1.15.775-1.925Q8.15 10.6 9.3 10.6h29.4q1.15 0 1.925.775.775.775.775 1.925v21.4q0 1.15-.775 1.925-.775.775-1.925.775ZM24 23.35 7.7 12.4v22.3q0 .7.45 1.15.45.45 1.15.45h29.4q.7 0 1.15-.45.45-.45.45-1.15V12.4Zm0-1.4L39.45 11.7H8.6ZM7.7 12.4v-.7 23q0 .7.45 1.15.45.45 1.15.45H7.7V34.7Z"/></svg>
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