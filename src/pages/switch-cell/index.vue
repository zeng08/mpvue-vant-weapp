<template>
  <div class="container">
    <demo-block title="基础用法">
      <van-cell-group>
        <van-switch-cell
          title="标题"
          :checked="checked"
          @change="onChange"
        />
      </van-cell-group>
    </demo-block>

    <demo-block title="禁用状态">
      <van-cell-group>
        <van-switch-cell
          disabled
          title="标题"
          :checked="checked"
          @change="onChange"
        />
      </van-cell-group>
    </demo-block>

    <demo-block title="加载状态">
      <van-cell-group>
        <van-switch-cell
          loading
          title="标题"
          :checked="checked"
          @change="onChange"
        />
      </van-cell-group>
    </demo-block>
  </div>
</template>

<script>

  export default {
    data () {
      return {
        checked: true
      }
    },
    methods: {
      onChange ({mp}) {
        this.checked = mp.detail
      }
    }
  }
</script>

<style>

</style>
