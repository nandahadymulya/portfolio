<template>
  <div>
    <div class="nav--container">
      <navbar-app />
      <icon-app />
    </div>
    <div class="content--container">
      <slot />
    </div>

    <div class="footer--container">
      <footer-app />
    </div>
  </div>
</template>
<style scoped>
.nav--container,
.content--container,
.footer--container {
  padding: 1rem;
  justify-content: space-between;
}

.nav--container,
.footer--container {
  display: flex;
  align-items: center;
}

.nav--container {
  background-color: var(--color-primary);
  top: 0;
  width: 100%;
  position: fixed;
}

.content--container {
  color: var(--color-primary);
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: calc(100vh);
  background-color: var(--color-light);
}

.footer--container {
  color: var(--color-light);
  background-color: var(--color-dark);
  bottom: 0;
  width: 100%;
  position: fixed;
  justify-content: center;
}
</style>
