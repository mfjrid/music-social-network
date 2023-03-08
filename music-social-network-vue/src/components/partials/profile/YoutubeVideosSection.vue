<template>
    <div class="mx-auto py-4">
        <div class="flex flex-wrap font-bold text-gray-100">
            <div class="text-gray-900 text-xl">YouTube Videos</div>
            <div class="bg-green-500 w-full h-1"></div>
            <div class="w-full mt-4">
                <RouterLinkButton btnText="Delete YouTube Video" class="ml-2" color="red"
                    url="/account/delete-youtube-video" />
                <RouterLinkButton btnText="Add YouTube Video" color="blue" url="/account/add-youtube-video" />
            </div>
        </div>
    </div>

    <div class="flex flex-wrap mb-4">
        <div class="my-1 px-1 w-full md:w-1/2 lg:w-1/2">
            <div class="text-xl text-gray-900">Video Title</div>
            <iframe src="https://www.youtube.com/embed/gpJdcKp_TrU?autoplay=0" frameborder="0"
                class="w-full h-60"></iframe>
        </div>
    </div>
</template>

<script setup>
    import RouterLinkButton from '../../global/RouterLinkButton.vue'
</script>