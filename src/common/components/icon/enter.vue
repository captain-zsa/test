<template functional>
  <g>
    <path d="M12 16L16 12L12 8L12 16Z" :fill="props.color"/>
    <rect x="6" y="11" width="9" height="2" :fill="props.color"/>
    <path d="M7 9H9V6H17V18H9V15H7V20H19V4H7V9Z" :fill="props.color"/>
  </g>
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
