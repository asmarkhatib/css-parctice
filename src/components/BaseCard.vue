<template>
  <div class="incoming-load-card">
    <slot></slot>
  </div>
</template>

<style lang="scss" scoped>
.incoming-load-card {
  width:230px;
  background: #fff;
  padding: 16px 24px 16px 24px;
  border-radius: 12px;
  cursor: pointer;
  border: 1px solid white;
}
.incoming-load-card:hover{
    border: 1px solid rgb(72, 72, 250);
}
</style>
