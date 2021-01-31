<template functional>
  <path fill-rule="evenodd" clip-rule="evenodd" d="M5 9C5 5.125 8.125 2 12 2C15.875 2 19 5.125 19 9C19 14.25 12 22 12 22C12 22 5 14.25 5 9ZM9.49979 8.99979C9.49979 10.3748 10.6248 11.4998 11.9998 11.4998C13.3748 11.4998 14.4998 10.3748 14.4998 8.99979C14.4998 7.62479 13.3748 6.49979 11.9998 6.49979C10.6248 6.49979 9.49979 7.62479 9.49979 8.99979Z" :fill="props.color" />
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

