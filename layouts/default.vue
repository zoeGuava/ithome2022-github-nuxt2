<template>
  <div>
    <div class="header">
      <div class="link-wrapper">
        <div class="link-container">
          <NuxtLink class="link-item" to="/">Home</NuxtLink>
        </div>
        <div class="link-container">
          <NuxtLink class="link-item" to="/profile">Profile</NuxtLink>
        </div>
        <div class="link-container">
          <NuxtLink class="link-item" to="/profile/login">Login</NuxtLink>
        </div>
      </div>
    </div>
    <Nuxt />
  </div>
</template>

<style lang="scss" scoped>
.link-wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
.link-container {
  padding: 5px;
  border-radius: 4px;
  background-color: #000000;
  transition: all 0.3s;
  cursor: pointer;

  .link-item {
    color: gray;
  }

  &:hover {
    background-color: rgb(191, 188, 188);

    .link-item {
      color: #000000;
    }
  }

}
</style>
