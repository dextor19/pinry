<template>
  <div class="profile-container">
    <div class="card">
      <header class="card-header">
        <p class="card-header-title">
          Token
        </p>
      </header>
      <div class="card-content">
        <div class="content">
          <p>Your Token is:</p>
          <pre>{{ token }}</pre>
          Please read <a target="_blank" href="https://www.django-rest-framework.org/api-guide/authentication/#tokenauthentication">DRF API Documentation</a> for more detail to know how to use it.
          <br>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'profile',
  props: ['token'],
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
.profile-container {
  margin-top: 2rem;
  margin-left: auto;
  margin-right: auto;
  box-shadow: 5px 5px 2px 1px rgba(0, 0, 255, .1);
}

@import '../utils/grid-layout';
@include screen-grid-layout(".profile-container");
</style>
