<template>
    <div class="card" style="width: 18rem;">
        <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
        <div class="card-body">
            <p class="card-text">{{ value }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: ['iconUrl', 'value']
};
</script>

<style scoped>
.card {
    margin: 10px;
    display: inline-block;
    width: calc(33% - 20px);
}
</style>
