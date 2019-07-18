<template>
  <div>
    <OrgChart :treeData = "testData"></OrgChart>
  </div>
</template>
<script>
import OrgChart from './tree/OrgChart'

export default {
  components: {
    OrgChart
  },
  provide: {
    nodeObj: { value: 'hhhh' }
  },
  watch: {
    nodeObj () {
      alert('123')
    }
  },
  data () {
    return {
      testData: [
        {
          id: '1',
          label: 'Hello',
          children: [
            {
              id: '2',
              label: 'World',
              children: [
                {
                  id: '4',
                  label: '44444',
                  children: []
                },
                {
                  id: '5',
                  label: '44444',
                  children: []
                }
              ]
            },
            {
              id: '3',
              label: 'Vue',
              children: [
                {
                  id: '6',
                  label: '123123',
                  children: []
                },
                {
                  id: '6',
                  label: '123123',
                  children: []
                },
                {
                  id: '6',
                  label: '123123',
                  children: []
                },
                {
                  id: '6',
                  label: '123123',
                  children: []
                },
                {
                  id: '6',
                  label: '123123',
                  children: []
                },
                {
                  id: '6',
                  label: '123123',
                  children: [
                    {
                      id: '6',
                      label: '123123',
                      children: []
                    }
                  ]
                }
              ]
            }
          ]
        }
      ]
    }
  }
  // methods: {
  //   handleClick: function (node) {
  //     alert(node.label)
  //   }
  // }
}
</script>
