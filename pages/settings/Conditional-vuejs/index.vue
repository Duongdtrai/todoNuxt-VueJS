<template>
    <div>
        <h1>
            Conditional vuejs
        </h1>
        <div>
            <div>
                <div v-show="isShow">
                    Khóa học này của v-show
                </div>
            </div>
            <div>
                <template v-if = "isShow === false ? isShow = true : isShow = true">
                    Khóa học này của v-if
                </template>
            </div>
            <button>

            </button>
        </div>
     </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data () {
    return {
      isShow: true
    };
  },
  methods: {
    
  }
}


// Conditional vuejs là việc xử lí v-if, v-elseif, v-else, v-show
// 1. v-if v-else dùng được trong <template>
// 2. v-show không dùng được trong <template>
</script>

