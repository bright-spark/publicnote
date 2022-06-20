<template>
  <div>
    <logo/>
    <br>
    Enter any title above to access a note. No account required.<br>
    <br>
    Every note is public.  You are free to modify any note you find.<br>
    <br>
    Every note is encrypted.  You must know the title to see the note.<br>
    <br>
    There are a variety of uses for publicnote:<br>
    <br>
    • personal note-taking<br>
    • copy-pasting between devices<br>
    • private messaging<br>
    • chatting with strangers<br>
    • letting out feelings<br>
    • jokes and ASCII art<br>
    • puzzles and scavenger hunts<br>
    • espionage dead drops<br>
    • wasting time<br>
    <br>
    Do not use publicnote to store sensitive information. By using publicnote, you are agreeing to our <div class="link" @click="sot.title = 'terms'">terms of service</div>.<br>
    <br>
    Publicnote is <a class="link" href="https://github.com/routman/publicnote" target="_blank" rel="noopener">open source</a> for full transparency. Convert your messages into encrypted emoji using <a class="link" href="https://cryptoji.com" target="_blank" rel="noopener">cryptoji.com</a>.<br>
    <br>
    daniel@ncrypt.org<br>
    1HrQfojcRt4gGEZntEwp24KVrSch8mtqMk<br>
    <br>
    publicnote &copy; {{ new Date().getFullYear() }}<br>
    <br>
  </div>
</template>

<script>
import logo from './logo.vue'
export default {
  name: 'home',
  components: {
    logo
  },
  data: function() {
    return {
      sot: this.$root.$data
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/settings.scss";

.ios {
  display: inline-block;
}

.android {
  display: inline-block;
  margin-left: 12px;
}

</style>
