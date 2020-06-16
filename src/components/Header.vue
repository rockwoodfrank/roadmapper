<template>
  <header class="blue-1 light-text-1">
    <div class="logo">
      <img src="@/assets/logo.svg" alt="Roadmapper Logo" />
      <router-link :to="{ name: 'MainApp' }" class="logo-text light-text-1"
        >Roadmapper</router-link
      >
    </div>
    <nav>
      <router-link to="?" class="light-text-1">Lorem</router-link>
      <router-link to="?" class="light-text-1">Lorem</router-link>
      <router-link to="?" class="light-text-1">Lorem</router-link>
      <router-link to="?" class="light-text-1">Lorem</router-link>
    </nav>
    <div class="profile">
      <img
        src="@/assets/default-profile-img.jpg"
        alt="Hello"
        class="profile__img"
      />
      <a class="profile__name">Rockwood</a>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss">
header {
  display: flex;
  padding: 1.5em 2em;
  justify-content: space-between;
  align-items: center;

  .logo {
    display: flex;
    align-items: center;
    font-weight: 700;
    .logo-text {
      padding: 0 0 0 0.5em;
      font-size: 1.3em;
    }
    img {
      height: 30px;
    }
  }

  nav {
    a {
      padding: 0 1.5em;
    }
  }

  .profile {
    display: flex;
    align-items: center;
    .profile__name {
      padding: 0 0.5em;
    }

    .profile__img {
      width: 2em;
      height: 2em;
      object-fit: cover;
      border-radius: 2em;
    }
  }
}
</style>
