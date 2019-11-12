<template>
  <div>
    <div>記事コード：{{ aid }}</div>
    <span>
      <router-link v-bind:to="'/article/' + aid + '/pages/1'">Page: 1</router-link>
    </span>|
    <span>
      <router-link v-bind:to="'/article/' + aid + '/pages/2'">Page: 2</router-link>
    </span>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "article",
  props: {
    aid: String
  }
};
</script>