<script lang="ts">
import "./heroSection.css";
import ProfilePicture from '../profilePicture/ProfilePicture.vue';

export default {
    components: { ProfilePicture }
}
</script>

<template>
    <div class="hero_section">
        <div class="pitch_black full_width slanted slanted_5 overlap_down_260px"></div>
        <div class="header_grid">
            <div class="main_cell centered_vertically">
                <h1>Tobias Rheindorf</h1>
                <h4>AKA notSafeForDev</h4>
                <h4>Frontend- & Game Developer</h4>
            </div>
            <div>
                <ProfilePicture image-url="portrait.jpg" />
            </div>
        </div>
        <div>
            <div class="spacer_medium"></div>
            <p>I'm Tobias Rheindorf, a developer that really gives it all for exciting projects!</p>
            <p>This site was built from scratch, as a fully responsive website using the <a
                    href="https://vuejs.org/">Vue
                    Framework</a>. The source code can be found on <a href="https://github.com/notSafeForDev/portfolio"
                    target="_blank">Github</a>.</p>
        </div>
    </div>
</template>