<template>
  <button class="btn btn-primary">
      <i :class="autoIcon"></i>
  </button>
</template>

<script>
export default {
    props: {
        icon: {
            type: String,
            default: 'fa-plus',
        },
    },
    computed: {
        autoIcon() {
            return `fa fa-2x ${this.icon}`
        }
    },
}
</script>

<style lang="scss" scoped>
    button{
        border-radius: 100%;
        bottom: 2rem;
        position: fixed;
        right: 2rem;
        border: lightseagreen 3px solid;
    }
</style>