<script setup>
  import {NDropdown,NButton} from 'naive-ui'
  const options = [
  {
    label: "杰·盖茨比",
    key: "jay gatsby",
  },
  {
    type: "divider",
    key: "d1",
  },
  {
    label: "尼克·卡拉威",
    key: "nick carraway",
  },
  {
    label: "第一级菜单1",
    key: "others1",
    children: [
      {
        label: "乔丹·贝克1",
        key: "jordan baker",
      },
      {
        label: "汤姆·布坎南1",
        key: "tom buchanan",
      },
    ],
  },
  {
    label: "尼克1",
    key: "nick1",
  },
  {
    label: "尼克2",
    key: "nick2",
  },
  {
    label: "第一级菜单3",
    key: "others3",
    children: [
      {
        label: "乔丹·贝克",
        key: "jordan baker",
      },
      {
        label: "汤姆·布坎南",
        key: "tom buchanan",
      },
    ],
  },
  {
    label: "尼克3",
    key: "nick3",
  },

  {
    label: "第一级菜单4",
    key: "others4",
    children: [
      {
        label: "乔丹·贝克2",
        key: "jordan baker",
      },
      {
        label: "汤姆·布坎南2",
        key: "tom buchanan",
      },
    ],
  },
];
  const handleSelect = (value)=>{
    console.log(value);
  }
</script>

<template>
  <n-dropdown trigger="click" :options="options" placement="top" @select="handleSelect">
    <n-button>点击！</n-button>
  </n-dropdown>
</template>

<style scoped>
</style>
