<template>
    <div v-show="!showMenu" class="fixed bg-black border-2 border-gray-700 rounded-lg ml-2 mt-6 pt-28 py-4 px-3 z-10 drop-shadow-lg">     
        <nav class="flex flex-col items-center space-y-4 justify-around">
            <div class="text-white font-light text-2xl">
                about us
            </div>
            <div  class="text-white font-light text-2xl">
                contact
            </div>
        </nav>
    </div>
</template>

<script>

export default {
    name: "SiteNav",
    props: {
        showMenu: Boolean
    }
}

</script>