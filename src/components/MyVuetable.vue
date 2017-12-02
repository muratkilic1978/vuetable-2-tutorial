// MyVuetable.vue

<template>
  <vuetable ref="vuetable"
    api-url="https://vuetable.ratiw.net/api/users"
    :fields="fields"
  ></vuetable>
</template>

<script>
import Vuetable from 'vuetable-2/src/components/Vuetable'

export default {
  components: {
    Vuetable
  },
  data () {
    return {
      fields: [
        {
          name: 'name',
          titleClass: 'right aligned',
          dataClass: 'right aligned'
        },
        {
          name: 'email',
          titleClass: 'right aligned',
          dataClass: 'right aligned'
        },
        {
          name: 'birthdate',
          titleClass: 'center aligned',
          dataClass: 'center aligned'
        },
        {
          name: 'nickname',
        },
        {
          name: 'gender',
          titleClass: 'center aligned',
          dataClass: 'center aligned'
        },
        {
          name: 'salary',
          titleClass: 'center aligned',
          dataClass: 'right aligned'
        }
      ]
    }
  }
}
</script>