<template>
  <div class="org-chart-container">
    <div class="org-chart-node-children">
      <OrgChartNode
        v-for="(node, index) in treeData"
        :key="index"
        :node="node"
      ></OrgChartNode>
    </div>
  </div>
</template>

<script>
import OrgChartNode from './OrgChartNode'
export default {
  name: 'OrgChart',
  components: {
    OrgChartNode
  },
  props: {
    treeData: {
      required: true
    }
  },
  methods: {
    
  }
  // ,
  // methods: {
  //   getChildren: function (nodes, parentId) {
  //     let result = []
  //     for (let i in nodes) {
  //       let node = nodes[i]
  //       result.push({
  //         id: node.id,
  //         parentId: parentId,
  //         label: node.label
  //       })
  //       result = result.concat(this.getChildren(node.children, node.id))
  //     }
  //     return result
  //   }
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* .org-chart-container {
    display: block;
    width: 100%;
    text-align: center;
  }
  .org-chart-node-children .org-chart-node-children::before {
    content: '';
    position: absolute;
    top: 0;
    left: 50%;
    border-left: 1px solid #ccc;
    width: 0;
    height: 20px;
  } */
</style>
