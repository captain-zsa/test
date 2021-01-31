<template functional>
  <path fill-rule="evenodd" clip-rule="evenodd" d="M19 13H13V19H11V13H5V11H11V5H13V11H19V13Z" :fill="props.color"/>
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
