<template>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{ name: 'JobDetails', params: { id: job.id } }">
      <h2>{{ job.title }}</h2>
    </router-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        { title: "Ninja UX Designer", id: 1, details: "lorem" },
        { title: "Ninja web Developer", id: 2, details: "lorem" },
        { title: "Ninja vue Developer", id: 3, details: "lorem" },
      ],
    };
  },
};
</script>

<style></style>
