<template>
    <div class="container max-w-4xl flex">
        <div class="w-1/3">
            <img class="w-full rounded-lg h-auto shadow-lg" src="https://via.placeholder.com/500" alt="Profile Pic">
        </div>
        <div class="w-full pl-4">
            <div class="flex">
                <div class="w-1/2 text-left">
                    <h1 class="text-2xl md:text-4xl text-gray-900">
                        John Watson
                    </h1>
                    <span class="text-md text-gray-700">
                        <i><b>London, UK</b></i>
                    </span>
                </div>
                <div class="w-1/2 mt-2">
                    <RouterLinkButton btnText="Edit Profile" color="green" url="/account/edit-profile" />
                </div>
            </div>
            <ProfileInfoSection />
            <ProfileAboutSection />
        </div>
    </div>
    <SongsSection />
    <YoutubeVideosSection />
    <PostsSection />
</template>

<script setup>
    import ProfileInfoSection from '../../components/partials/profile/ProfileInfoSection.vue'
    import ProfileAboutSection from '../../components/partials/profile/ProfileAboutSection.vue'
    import SongsSection from '../../components/partials/profile/SongsSection.vue'
    import YoutubeVideosSection from '../../components/partials/profile/YoutubeVideosSection.vue'
    import PostsSection from '../../components/partials/profile/PostsSection.vue'
    import RouterLinkButton from '../../components/global/RouterLinkButton.vue'
</script>