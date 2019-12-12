<template>
  <div class="content-area">
    <b-table
      stacked
      :items="items"
      :fields="fields"
    >
    </b-table>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      fields: [
        {
          key: 'id',
          label: '商品コード'
        },
        {
          key: 'name',
          label: '商品名'
        },
        {
          key: 'group',
          label: '菓子'
        },
        {
          key: 'allergies',
          label: 'アレルギー'
        },
      ],
      items: [
        {
          id: '628402942632',
          name: 'えびおかき',
          group: '菓子',
          allergies: 'えび'
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content-area {
  width: 700px;
  margin: auto;
}
</style>
