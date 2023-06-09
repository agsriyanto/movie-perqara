<template>
  <div class="checkbox text-white items-center flex justify-between">
    <label>{{name}}</label>
    <input type="checkbox" :name="name" v-model="checked" class="checked:bg-[#E74C3C]">
  </div>
</template>

<script>
export default 
{
  props: 
  {
      name: 
      {
          type: String,
          required: true
      },
      val: 
      {
          type: String,
          required: true
      },
      value:
      {
          type: Array,
          default: () => []
      }
  },
  computed: 
  {
      checked: 
      {
          get () 
          {
              return this.value.includes(this.val)
          },
          set (newVal) 
          {
              const current = this.val
              this.$emit('input', newVal ? this.value.concat([current]) : this.value.filter(item => item !== current))
          }
      }
  },
}
</script>