<template>
  <div id="app">
    <MonsterAttack/>
    <WonderfulQuotes/>
  </div>
</template>

<script>
import MonsterAttack from './components/MonsterAttack'
import WonderfulQuotes from "./components/WonderfulQuotes";
export default {
  name: 'App',
  components: {
    MonsterAttack,
    WonderfulQuotes
  }
}
</script>

<style>
</style>
