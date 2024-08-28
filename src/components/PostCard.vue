<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Officia do esse cillum minim nisi quis consectetur ad ullamco anim aute.</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue'
</script>

<style scope>

.post-card {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}

</style>