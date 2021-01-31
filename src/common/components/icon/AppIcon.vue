<template>
  <svg class="icon" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
    <component
      :is="iconComponent"
      :color="colors[color]"
    />
  </svg>
</template>

<script>
import { colors } from '@/common/constants';

export default {
  name : 'AppIcon',

  props : {
    icon : {
      type    : String,
      default : 'close',
    },

    color : {
      type    : String,
      default : 'black',
    },
  },

  data() {
    return {
      colors,
    };
  },

  computed : {
    iconComponent() {
      return () => import(`./${this.icon}`);
    },
  },
};
</script>
