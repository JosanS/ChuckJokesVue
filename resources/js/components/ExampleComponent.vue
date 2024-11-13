<template>
    <div>
        <h1>Chistes de Chuck Norris</h1>
        <div class="card-container">
            <chuck-card
                v-for="joke in jokes"
                :key="joke.value"
                :icon-url="joke.icon_url"
                :value="joke.value"
            />
        </div>
    </div>
</template>

<script>
import ChuckCard from '/resources/js/components/ChuckCard.vue';

export default {
    components: {
        ChuckCard,
    },
    data() {
        return {
            
            jokes: [
                {
                    icon_url: "https://img.europapress.es/fotoweb/fotonoticia_20150310130850-732359_1024.jpg",
                    value: "Chuck Norris can skydive into outer space."
                },
                {
                    icon_url: "https://pbs.twimg.com/media/ErkMbXtUcAELm6O.jpg",
                    value: "The chief export of Chuck Norris is pain."
                },
                {
                    icon_url: "https://www.slashfilm.com/img/gallery/chuck-norris-needed-a-push-from-steve-mcqueen-to-even-consider-a-career-in-acting/l-intro-1662649398.jpg",
                    value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants."
                },
                {
                    icon_url: "https://getwallpapers.com/wallpaper/full/e/3/4/879205-popular-chuck-norris-wallpapers-2048x1536-for-windows-7.jpg",
                    value: "Time waits for no man. Unless that man is Chuck Norris."
                },
                {
                    icon_url: "https://muscleinsider.com/sites/default/files/styles/node_gallery_display/public/Chuck_Norris_Launches_Roundhouse_Provisions_Morning_Kick.jpg?itok=5CsOXuOq",
                    value: "If you spell Chuck Norris in Scrabble, you win. Forever."
                },
            ]
        };
    }
};
</script>
