<template>
  <div class="container">
    <demo-block title="基础用法">
      <van-cell-group>
        <van-cell title="单元格" value="内容"/>
        <van-cell title="单元格" value="内容" label="描述信息" :border="false"/>
      </van-cell-group>
    </demo-block>
    <demo-block title="展示图标">
      <van-cell-group>
        <van-cell title="单元格" icon="location" :border="false" />
      </van-cell-group>
    </demo-block>

    <demo-block title="展示箭头">
      <van-cell-group>
        <van-cell title="单元格" is-link />
        <van-cell title="单元格" is-link value="内容" />
        <van-cell
          title="单元格"
          is-link
          arrow-direction="down"
          value="内容"
          :border="false"
          url="/pages/dashboard/main"
        />
      </van-cell-group>
    </demo-block>

    <demo-block title="高级用法">
      <van-cell-group>
        <van-cell value="内容" icon="shop" is-link>
          <view slot="title">
            <view class="title">单元格</view>
            <van-tag type="danger">标签</van-tag>
          </view>
        </van-cell>
        <van-cell title="单元格" icon="location" is-link />
        <van-cell title="单元格" :border="false">
          <van-icon slot="right-icon" name="search" />
        </van-cell>
      </van-cell-group>
    </demo-block>
  </div>
</template>

<script>

  export default {
    data () {
      return {}
    },
    methods: {}
  }
</script>

<style lang="less">
  .title {
    margin-right: 5px;
    display: inline-block;
    vertical-align: middle;
  }
</style>
