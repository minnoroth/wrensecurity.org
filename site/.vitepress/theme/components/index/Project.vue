<template>
  <section class="project-wrapper">
    <h1>
      <slot name="title" />
    </h1>
    <p>
      <slot name="description" />
    </p>
    <div class="project-features">
      <slot name="features" />
    </div>
  </section>
</template>

<style scoped>
.project-wrapper {
  padding-top: 80px;
  /* border-top: 1px solid var(--vp-c-divider); */
}
.project-features {
  /* display: flex;
  column-gap: 28px;
  margin-top: 28px; */
}
.project-features :slotted(ul) {
  display: grid;
  /* flex-wrap: wrap; */
  list-style: none;
  padding-left: 0;
  /* column-gap: 28px; */
  /* row-gap: 14px; */
  margin-top: 42px;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
  justify-items: stretch;
  align-items: stretch;
}
</style>
