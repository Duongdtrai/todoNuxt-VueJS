<template>
  <div>
    <nuxt-link to='/settings/Conditional-vuejs'>
        Conditional-vuejs
    </nuxt-link>
    <nuxt-link to='/settings/List-rendering'>
        List-rendering
    </nuxt-link>
    <nuxt-link to='/settings/Watch-Computed'>
        Watch-Computed
    </nuxt-link>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  name: 'Setting',
}
// Tạo 1 file to.vue, sau đó tạo 1 folder đúng tên file to.vue, bên trong là những child
</script>
