<template lang="pug">
  #App
    Top
    Marquee
    #Content
      Content
      Msgboard(v-if="page =='Msgboard'")
    //- 在子元件裡面再去定義某個子元件 使用 v-slot  可以傳入 html
    //- https://medium.com/unalai/%E8%A4%87%E7%94%A8%E5%85%83%E4%BB%B6%E7%9A%84%E5%A5%BD%E5%B9%AB%E6%89%8B-vue-slot-v-slot-scoped-slots-5364a0048ab7

    Footer

</template>

<script>
import Top from './components/Top'
import Marquee from './components/Marquee'
import Content from './components/Content'
import Msgboard from './components/Msgboard'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Top,
    Marquee,
    Content,
    Msgboard,
    Footer
  },
  data () {
    return {
      page: 'Msgboard'
    }
  }

}
</script>
