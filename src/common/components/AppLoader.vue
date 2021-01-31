<template>
  <svg width="24" height="24" viewBox="0 0 24 24" fill="none" class="loader" xmlns="http://www.w3.org/2000/svg">
    <path d="M12.0198 6.4C8.91935 6.4 6.40594 8.90721 6.40594 12C6.40594 15.0928 8.91935 17.6 12.0198 17.6C14.848 17.6 17.1877 15.5138 17.5768 12.8H20C19.5976 16.8427 16.1783 20 12.0198 20C7.59059 20 4 16.4183 4 12C4 7.58172 7.59059 4 12.0198 4C12.6842 4 13.2228 4.53726 13.2228 5.2C13.2228 5.86274 12.6842 6.4 12.0198 6.4Z" fill="url(#paint0_radial)"/>
    <defs>
      <radialGradient id="paint0_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(19.1975 11.4711) rotate(116.792) scale(19.713 9.86265)">
      <stop
        offset="0.140625"
        :stop-color="stopColor"
        stop-opacity="0"
      />
      <stop
        offset="1"
        :stop-color="stopColor"
      />
    </radialGradient>
    </defs>
  </svg>
</template>

<script>
import { colors } from '@/common/constants';

export default {
  name: 'AppLoader',

  props : {
    color : {
      type    : String,
      defauld : 'primary',
    },
  },

  data() {
    return {
      colors,
    };
  },

  computed : {
    stopColor() {
      const colors = {
        'primary' : this.colors['primary-300'],
        'black'   : this.colors['black-100'],
        'white'   : this.colors.white,
      };

      return colors[this.color];
    },
  },
};
</script>

<style lang="scss">
.loader {
  animation-name: rotation;
  animation-duration: 1s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}

@keyframes rotation {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

</style>
