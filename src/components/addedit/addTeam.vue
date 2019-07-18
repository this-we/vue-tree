<template>
  <div>
    <Modal :v-model="teamShow">
      <Input v-model="value" placeholder="输入节点名称" style="width: 300px" />
      <Button type="primary">确定</Button>
    </Modal>
  </div>
</template>

<script>
export default {
  name: '',
  props: {
    teamShow: Boolean
  },
  data () {
    return {
      teamshow: false,
      value: ''
    }
  }
}
</script>

<style scoped>
  
</style>