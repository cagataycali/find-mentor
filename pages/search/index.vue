<template>
  <div class="page search-main-page">
    <div class="pw-100 vh-100 d-flex align-items-center">
      <div class="col-md-6 mx-auto">
        <h1 class="mb-4">Search</h1>
        <app-search-input @searchTriggered="searchPerson" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    searchPerson(keyword) {
      this.$router.push({
        name: 'search-keyword',
        params: { keyword },
      })
    },
  },
}
</script>
