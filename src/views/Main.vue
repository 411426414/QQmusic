<template>
  <div class="main">
    <main-header
      title='Function Music'
      @nav-click='toPath'
    >
    </main-header>
    <router-view></router-view>
  </div>
</template>

<script>
import MainHeader from '@/components/Main/MainHeader'

export default {
  methods: {
    toPath(path) {
      this.$router.push(path);
    }
  },
  components: {
    MainHeader
  }
}
</script>