<template>
  <q-page class="flex flex-center text-h5 relative-bottom q-gutter-md">
    <div class="row q-pa-md flex-center text-h5 relative-bottom">
      <h4> Quem está assitindo? </h4>

      <div class="row col-md-12 col-sm-4 col-xs-2 q-gutter-xl flex-center text-h5 relative-bottom">
        <cardProfile
          v-for="(item, key) in cont"
          :key="key"
        />
        <q-btn
          flat
          class="flex flex-center"
          round
          color="red"
          icon="add"
          label="Adicionar"
        />
      </div>
    </div>

  </q-page>
</template>

<script>
import cardProfile from 'components/selectProfile/cards'
export default {
  components: { cardProfile },
  name: 'PageIndex',
  data () {
    return {
      cont: 3
    }
  }
}
</script>
