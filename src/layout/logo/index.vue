<template>
  <div class="logo">
    <img :src="setting.logo_url" alt="" />
    <h1>{{ setting.title }}</h1>
  </div>
</template>

<script lang="ts" setup>
import setting from '@/setting'
</script>

<style lang="scss" scoped>
.logo {
  height: $base-logo-height;
  padding: 15px;
  display: flex;

  h1 {
    color: #959ea6;
    display: inline-block;
    height: 32px;
    overflow: hidden;
    font-size: $base-logo-size;
    font-weight: 600;
    line-height: 32px;
    text-overflow: ellipsis;
    white-space: nowrap;
    margin-left: 40px;
  }

  img {
    width: 30px;
    height: 30px;
    border-radius: 5px;
  }
}
</style>
