<template functional>
  <path fill-rule="evenodd" clip-rule="evenodd" d="M7 10L12 15L17 10H7Z" :fill="props.color"/>
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
