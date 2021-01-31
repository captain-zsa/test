<template functional>
  <path d="M8.58997 16.58L13.17 12L8.58997 7.41L9.99997 6L16 12L9.99997 18L8.58997 16.58Z" :fill="props.color"/>
</template>

<script>
export default {
  props : {
    color : {
      type     : String,
      required : true,
    },
  },
};
</script>
