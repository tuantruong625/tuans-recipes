<template>
  <view class="container">
    <image
          :style="{width: 300, height: 200}"
          :source="require('./assets/undraw_eating_together_tjhx.png')"
      />
    <text class="text-color-primary">{{ title }}</text>
    <button class="my-first-button" v-bind:title="buttonTitle" v-bind:on-press="handleBtnPress"/>
    </view>
</template>

<script>
export default {
  data() {
    return {
      title: 'Tuans Recipes',
      buttonTitle: 'Click Me'

    }
  },
  methods: {
    handleBtnPress() {
      alert('Hi');
    }
  }
}
</script>


<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  font-size: 25;
  font-weight: 600;
  letter-spacing: 1.5;
  margin-top: 2;
  color: #1c7ed6;
}
</style>
