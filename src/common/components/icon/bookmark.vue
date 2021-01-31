<template functional>
  <g>
    <g filter="url(#filter0_d)">
      <path d="M22 5H8V23L15 20L22 23L22 5Z" :fill="props.color"/>
    </g>
    <defs>
      <filter id="filter0_d" x="-5" y="-3" width="40" height="40" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
        <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"/>
        <feOffset dy="3"/>
        <feGaussianBlur stdDeviation="4"/>
        <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.08 0"/>
        <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
        <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
      </filter>
    </defs>
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

