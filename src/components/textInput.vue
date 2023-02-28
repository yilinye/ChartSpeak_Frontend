<!--
 * @Author: 秦少卫
 * @Date: 2022-09-03 19:16:55
 * @LastEditors: 秦少卫
 * @LastEditTime: 2022-09-06 23:20:40
 * @Description: 图层面板
-->

<template>
  <div class="textInput">
    <el-divider content-position="bottom" style="margin-top:0px"> Text Input </el-divider>

  </div>
</template>

<script setup>
import { useI18n } from 'vue-i18n'
// const { t } = useI18n()
// let mSelectMode = inject('mSelectMode')
// let mSelectId = inject('mSelectId')
// let mSelectIds = inject('mSelectIds')
// const canvas = inject("canvas")

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
:deep(.ivu-tooltip-inner) {
  white-space: normal;
}

:deep(.ivu-tooltip) {
  display: block;
}

:deep(.ivu-tooltip-rel) {
  display: block;
}

.textInput {
  width: 100%; height: 28%;margin-top:10px; background:#fff;
}
.layer-box {
  max-height: 170px;
  height: auto;
  overflow-y: auto;
  margin-bottom: 5px;

  .ellipsis {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    cursor: pointer;
  }

  &>div {
    padding: 0px 5px;
    margin: 3px 0;
    background: #f7f7f7;
    color: #c8c8c8;
    border-radius: 3px;
    font-size: 12px;
    line-height: 28px;

    &.active {
      color: #2d8cf0;
      background: #f0faff;
      font-weight: bold;
    }
  }
}

svg {
  vertical-align: text-top;
}
</style>

<style lang="less">
span.active {
  svg.icon {
    fill: #2d8cf0;
  }
}
</style>
