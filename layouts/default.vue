<template>
  <div>
    <div class="nav--container">
      <navbar-app />
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
  justify-content: space-between;
  padding: 1rem;
}

.nav--container,
.footer--container {
  align-items: center;
  display: flex;
}

.nav--container {
  background-color: var(--color-primary);
  position: fixed;
  top: 0;
  width: 100%;
}

.content--container {
  align-items: center;
  background-color: var(--color-light);
  display: flex;
  justify-content: center;
  min-height: calc(100vh);
}

.footer--container {
  color: var(--color-light);
  background-color: var(--color-dark);
  bottom: 0;
  justify-content: center;
  position: fixed;
  width: 100%;
}
</style>
