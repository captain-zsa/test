<template functional>
  <path d="M17 10L12 15L7 10" :stroke="props.color" stroke-width="1.5"/>
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
