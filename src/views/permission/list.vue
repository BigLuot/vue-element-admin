<template>
  <div class="app-container">
    <el-row :gutter="20">
      <el-col :span="10">
        <permission :business-type="1" :business-id="1"/>
      </el-col>
    </el-row>

    <el-tooltip placement="top" content="去顶部">
      <back-to-top :visibility-height="300" :back-position="50" transition-name="fade"/>
    </el-tooltip>
  </div>
</template>

<script>
import BackToTop from '@/components/BackToTop'
import Permission from '@/components/Permission'

export default{
  name: 'PermissionList',
  components: { BackToTop, Permission }
}
</script>

