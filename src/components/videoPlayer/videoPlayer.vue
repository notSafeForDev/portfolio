<script lang="ts">
import "./videoPlayer.css";
export default {
    mounted() {
        let externalScript = document.createElement("script");
        externalScript.setAttribute("src", "//video-player.nyc3.digitaloceanspaces.com/release/bundle.js");
        document.head.appendChild(externalScript);
    }
}
</script>

<template>
    <div class="video_player">
        <img src="https://nyc3.digitaloceanspaces.com/video-player/trailers/JazminLuv-MikeMancini_001.jpg" />
        <web-vr-video-player class="video_player_player"
            coverimage="https://nyc3.digitaloceanspaces.com/video-player/trailers/JazminLuv-MikeMancini_001.jpg"
            hapticscsv="https://video-player.nyc3.digitaloceanspaces.com/trailers/JazminLuv-MikeMancini-180-POV-FPVR-TRAILER_2k.csv">
            <source
                src="https://video-player.nyc3.digitaloceanspaces.com/trailers/JazminLuv-MikeMancini-180-POV-FPVR-TRAILER_2k.mp4"
                data-quality="2K" enableScrollToZoom="false" />
            <source
                src="https://video-player.nyc3.digitaloceanspaces.com/trailers/JazminLuv-MikeMancini-180-POV-FPVR-TRAILER_4k.mp4"
                data-quality="4K" enableScrollToZoom="false" />
            <source
                src="https://video-player.nyc3.digitaloceanspaces.com/trailers/JazminLuv-MikeMancini-180-POV-FPVR-TRAILER_8kHD.mp4"
                data-quality="8K" enableScrollToZoom="false" />
        </web-vr-video-player>
        <slot></slot>
    </div>
</template>