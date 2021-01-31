<template functional>
  <g>
    <rect x="6" y="4" width="16" height="2" :fill="props.color"/>
    <rect x="6" y="11" width="16" height="2" :fill="props.color"/>
    <rect x="6" y="18" width="8" height="2" :fill="props.color"/>
    <rect x="2" y="4" width="2" height="2" :fill="props.color"/>
    <rect x="2" y="11" width="2" height="2" :fill="props.color"/>
    <rect x="2" y="18" width="2" height="2" :fill="props.color"/>
    <path d="M19.4 20.4667C19.2 20.7333 18.8 20.7333 18.6 20.4667L16.6 17.8C16.3528 17.4704 16.588 17 17 17L21 17C21.412 17 21.6472 17.4704 21.4 17.8L19.4 20.4667Z" :fill="props.color"/>
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
