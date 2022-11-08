<template>
  <section class="container">
    <slot />
    <div class="item grow1 basis-auto" v-for="item in list" :key="item.id">
      {{ item.name }}
    </div>
    <div class="item grow2 basis-auto">10</div>
  </section>
</template>

<script>
export default {
  setup() {
    const list = [
      { id: 1, name: "1" },
      { id: 2, name: "2" },
      { id: 3, name: "3" },
      { id: 4, name: "4" },
      { id: 5, name: "5" },
      { id: 6, name: "6" },
      { id: 7, name: "7" },
      { id: 8, name: "8" },
      { id: 9, name: "9" },
    ];

    return { list };
  },
};
</script>

<style>
.base-container {
  @apply grid gap-4 sm:grid-cols-2 md:grid-cols-3 container mx-auto;
}

/*itens*/

.basis-auto {
  flex-basis: auto;
}

.grow0 {
  flex-grow: 0;
}

.grow1 {
  flex-grow: 1;
}

.grow2 {
  flex-grow: 2;
}

.align-flex-end {
  align-content: flex-end;
}

.align-flex-start {
  align-content: flex-start;
}

/*conteúdo*/
.stretch {
  align-content: stretch;
}

.flex-start {
  justify-content: flex-start;
}

.flex-end {
  justify-content: flex-end;
}

.flex-center {
  justify-content: center;
}

.flex-space-between {
  justify-content: space-between;
}

.flex-space-around {
  justify-content: space-around;
}

.nonwrap {
  flex-wrap: nowrap;
}

.wrap {
  flex-wrap: wrap;
}

.wrap-reverse {
  flex-wrap: wrap-reverse;
}

.row {
  flex-direction: row;
}

.row-reverse {
  flex-direction: row-reverse;
}

.column {
  flex-direction: column;
}

.column-reverse {
  flex-direction: column-reverse;
}

.flex {
  display: flex;
}

.flex-wrap {
  flex-wrap: wrap;
}

.flex-item-1 {
  flex: 2;
}

/* Flex Item */
.item {
  margin: 5px;
  background: tomato;
  text-align: center;
  font-size: 1.5em;
}

.container {
  max-width: 400px;
  margin: 0 auto;
  display: flex;
  border: 1px solid #ccc;
}

h1 {
  text-align: center;
  margin: 20px 0 0 0;
  font-size: 1.25em;
  font-weight: normal;
}

body {
  font-family: monospace;
  color: #333;
}
</style>
