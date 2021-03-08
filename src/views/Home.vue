<template>
  <div>
    <hello />
    <portfolio />
    <users/>
    <foot/>
  </div>
</template>

<script>
import Hello from '@/components/Hello'
import Portfolio from '@/components/Portfolio'
import Users from '@/components/Users'
import Foot from '@/components/Foot'

export default {
  name: 'Home',
  components: {
    Hello,
    Portfolio,
    Users,
    Foot
  }
}
</script>
