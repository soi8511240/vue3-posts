<template>
  <div>
    <h2>Home View</h2>
    <p>{{ useRouter.name }}</p>
    <button class="btn btn-primary" @click="goAboutPage">
      About 으로 이동
    </button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();
const goAboutPage = () => {
  router.push('/about');
};
</script>

<style lang="scss" scoped></style>
