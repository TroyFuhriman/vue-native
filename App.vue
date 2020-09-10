<template>
  <view class="container">
    <text class="text-color-primary">{{ message }}</text>
    <button title="Press me!" @press="exclaim" />
  </view>
</template>

<script>
export default {
  data() {
    return {
      count: 1,
      message: `Hello World `,
    };
  },
  methods: {
    exclaim() {
      this.count++;
    },
  },
};
</script>

<style>
.container {
  flex: 1;
  background-color: white;
  align-items: center;
  justify-content: center;
}
.text-color-primary {
  color: blue;
  font-size: 30;
}
</style>
