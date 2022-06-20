<template>
  <div>
    <div v-if="sot.status == 'busy'" id="spinner"></div>
    <div v-if="sot.status == 'ok'" id="checkmark"></div>
    <div v-if="sot.status == 'error'" class="close icon"></div>
  </div>
</template>

<script>
export default {
  name: 'status',
  data: function() {
    return {
      sot: this.$root.$data,
    }
  },
}
</script>

<style scoped lang="scss">
@import "../assets/settings.scss";

#spinner {
	display: inline-block;
  border: 2px solid;
  border-color: $color-inactive;
  border-top: 2px solid #FFFFFF;
  border-radius: 50%;
  width: 15px;
  height: 15px;
  animation: spin 0.5s linear infinite;
  margin-top: 10px;
  margin-right: 2px;
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

#checkmark {
  display: inline-block;
  width: 8px;
  height: 16px;
  border: solid;
  border-color: $color-primary;
  border-width: 0 2px 2px 0;
  transform: rotate(45deg);

  margin-top: 10px;
  margin-right: 6px;
}

.close.icon {
  display: inline-block;
  color: $color-alert;
  width: 21px;
  height: 21px;
}

.close.icon:before {
  content: '';
  position: absolute;
  top: 16px;
  width: 21px;
  height: 2px;
  background-color: currentColor;
  -webkit-transform: rotate(-45deg);
          transform: rotate(-45deg);
}
.close.icon:after {
  content: '';
  position: absolute;
  top: 16px;
  width: 21px;
  height: 2px;
  background-color: currentColor;
  -webkit-transform: rotate(45deg);
          transform: rotate(45deg);
}

@media (prefers-color-scheme: dark) {
  #spinner {
    border: 2px solid;
    border-color: $color-accent;
    border-top: 2px solid #211e21;
  }
}


</style>
