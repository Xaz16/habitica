<template functional>
  <span
    class="message-count"
    :class="{'top-count': props.top === true, 'top-count-gray': props.gray === true}"
  > {{ props.count }} </span>
</template>

<style lang="scss">
@import '~@/assets/scss/colors.scss';

.message-count {
  background-color: $blue-50;
  border-radius: 50%;
  height: 20px;
  width: 20px;
  float: right;
  color: $white;
  text-align: center;
  font-weight: bold;
  font-size: 12px;
}

.message-count.top-count {
  position: absolute;
  right: 0.3em;
  top: -0.8em;
  padding: 0.2em;
  background-color: $red-50;
}

.message-count.top-count-gray {
  background-color: $gray-200;
}
</style>
