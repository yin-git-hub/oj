<template>
  <div class="layout-demo">
    <a-layout style="height: 400px;">
      <a-layout-header>Header</a-layout-header>
      <a-layout-content>

        <div style="background-color: aquamarine;">
          <basic-left></basic-left>
        </div>

      </a-layout-content>
      <a-layout-footer>Footer</a-layout-footer>
    </a-layout>
    <br />

  </div>
</template>
<script>
import BasicLeft from './BasicLeft.vue';
export default {

  components: {
    BasicLeft,
  }
}
</script>
<style scoped>
.layout-demo :deep(.arco-layout-header),
.layout-demo :deep(.arco-layout-footer),
.layout-demo :deep(.arco-layout-sider-children),
.layout-demo :deep(.arco-layout-content) {
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: var(--color-white);
  font-size: 16px;
  font-stretch: condensed;
  text-align: center;
}


.layout-demo :deep(.arco-layout-header),
.layout-demo :deep(.arco-layout-footer) {
  height: 64px;
  background-color: var(--color-primary-light-4);
}

.layout-demo :deep(.arco-layout-sider) {
  width: 206px;
  background-color: var(--color-primary-light-3);
}

.layout-demo :deep(.arco-layout-content) {
  background-color: rgb(var(--arcoblue-6));
}
</style>