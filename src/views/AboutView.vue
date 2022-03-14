<template>
  <div class="about">
    <h1>This is an about page</h1>
    {{address}}
    {{city}}
    {{country}}

  </div>
</template>
<script>
export default {
props: [
  'address',
  'city',
  'country',
]



}
</script>
