<template>
  <div>
    <h1>
      Đây là số: {{$route.params.id}}
    </h1>
    <button>
      <nuxt-link to='/MyPage'>
        Quay Lại
      </nuxt-link>
    </button>
  </div>

</template>


<script>
export default ({
  // cái này là ROUTE
})
</script>

