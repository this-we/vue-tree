<template>
  <div>
    <nodeTree :treeData='testData'></nodeTree>
  </div>
</template>
<script>
import nodeTree from './tree/OrgChart'

export default {
  components: {
    nodeTree
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
}
</script>
