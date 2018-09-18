<template>
  <view class="container">
    <text class="text-color-primary">{{ app_title }}</text>
    <button v-bind:title="app_title" v-bind:on-press="handleBtnPress" />
    </view>
</template>
 
 <script>
export default {
  data: function() {
    return {
      app_title: "tabula rasa"
    };
  },
  methods: {
    handleBtnPress: function() {
      alert('You have just been alerted.');
    }
  }
};
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
  font-size:30;
}
</style>
