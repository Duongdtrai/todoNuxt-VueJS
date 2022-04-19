<template>
  <div>
    <div>
      <h1>Router</h1>
      <nuxt-link to='/settings'>
        MySettings
      </nuxt-link>
     
      <nuxt-link to='/MyUser'>
        MyUser
      </nuxt-link>
       <!-- <nuxt-link to='/MyHeader'>
        MyHeader
      </nuxt-link>
      <nuxt-link to='/MyPage'>
        MyPage
      </nuxt-link> -->
    </div>
    <Introduce />
  </div>
</template>

<script>
import Introduce from "../components/Introduce.vue"
export default {
  name: 'IndexPage',
  components:{
    Introduce
  },
}

</script>

