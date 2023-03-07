<template>
    <div class="bg-green-500 rounded">
        <div id="aplayer">
        </div>
    </div>
</template>

<script setup>
    import { onMounted } from 'vue';
    import APlayer from 'aplayer';
    import 'aplayer/dist/APlayer.min.css';

    onMounted(() => {
        thePlayer();
    })

    const thePlayer = () => {
        new APlayer({
            container: document.getElementById('aplayer'),
            audio: [
                {
                    name: 'First Song',
                    artist: 'artist',
                    url: '../../../../music/a-small-miracle.mp3',
                    cover: 'cover.jpg'
                },
                {
                    name: 'Second Song',
                    artist: 'artist',
                    url: '../../../../music/lifelike.mp3',
                    cover: 'https://player.dogecloud.com/img/logo_with_product3.png'
                },
            ]
        });
    }
</script>