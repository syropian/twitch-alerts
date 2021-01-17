<template>
  <div class="main">
    <NewFollower name="Syropian" />
    <NewSubscriber name="Syropian" />
    <Resubscriber name="Glovelyyy" :amount="12" />
    <SubGifted name="CorruptedG" sender="Glovelyyyy" />
    <NewCheer name="Syropian" :amount="100" />
    <NewTip name="Glovelyyy" :amount="20" />
    <NewHost name="CorruptedG" :amount="600" />
    <NewRaid name="CorruptedG" :amount="1000" />
  </div>
</template>

<script setup>
import NewFollower from "./components/NewFollower.vue";
import NewSubscriber from "./components/NewSubscriber.vue";
import Resubscriber from "./components/Resubscriber.vue";
import SubGifted from "./components/SubGifted.vue";
import NewCheer from "./components/NewCheer.vue";
import NewTip from "./components/NewTip.vue";
import NewHost from "./components/NewHost.vue";
import NewRaid from "./components/NewRaid.vue";
</script>

<style>
html,
body {
  min-height: 100vh;
  overflow-y: auto;
}

#app {
  width: 100vw;
}

.main {
  display: grid;
  grid-template-columns: repeat(2, 498px);
  gap: 20px;
  width: 100%;
  padding: 20px;
}
</style>
