<template>
  <div :class="$style.notFound">
    <vue-icon-vuesion :class="$style.logo" />
    <vue-headline level="1">404</vue-headline>
    <vue-headline level="3">Page not found!</vue-headline>
  </div>
</template>

<script lang="ts">
import VueHeadline from '../../shared/components/VueHeadline/VueHeadline.vue';
import VueIconVuesion from '@/app/shared/components/icons/VueIconVuesion/VueIconVuesion.vue';

export default {
  metaInfo: {
    title: 'vuesion - page not found',
    meta: [
      {
        name: 'robots',
        content: 'NOINDEX,NOFOLLOW',
      },
    ],
  },
  name: 'NotFound',
  components: { VueIconVuesion, VueHeadline },
  props: {},
  data(): any {
    return {};
  },
  computed: {},
  methods: {},
};
</script>

<style lang="scss" module>
@import '~@/app/shared/design-system';

.notFound {
  padding-top: $nav-bar-height;
  text-align: center;
  width: 300px;
  height: 300px;
  margin: auto;
  margin-top: 25%;
}

.logo {
  width: $space-84;
  height: $space-84;
}
</style>
