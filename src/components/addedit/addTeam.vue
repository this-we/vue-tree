<template>
  <div>
    <Modal :v-model="isTeamShow">
      <Input v-model="value" placeholder="输入节点名称" style="width: 300px" />
      <Button type="primary">确定</Button>
    </Modal>
  </div>
</template>

<script>
export default {
  name: '',
  props: {
    isTeamShow: Boolean
  },
  data () {
    return {
      value: ''
    }
  }
}
</script>

<style scoped>
  
</style>