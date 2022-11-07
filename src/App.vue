<template>
  <section class="grid gap-4 sm:grid-cols-2 md: grid-cols-3 container mx-auto">
    <p v-for="item in list" :key="item.id">{{ item.name }}</p>
  </section>
</template>

<script>
export default {
  setup() {
    const list = [
      { id: 1, name: "Tailwind CSS" },
      { id: 2, name: "Tailwind CSS" },
      { id: 3, name: "Tailwind CSS" },
      { id: 4, name: "Tailwind CSS" },
      { id: 5, name: "Tailwind CSS" },
      { id: 6, name: "Tailwind CSS" },
      { id: 7, name: "Tailwind CSS" },
      { id: 8, name: "Tailwind CSS" },
      { id: 9, name: "Tailwind CSS" },
    ];

    return { list };
  },
};
</script>

<style lang="scss"></style>
