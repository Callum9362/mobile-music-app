<template>
  <div id="app">
    <header>
      <h1>My Music</h1>
    </header>
      <main>
        <section class="player">
          <h2 class="song-title">{{ current.title }} - <span>{{current.artist}}</span></h2>
        </section>
      </main>
  </div>
</template>

<script>


export default {
  name: 'App',
  data () {
    return {
      current: {
        title: 'SONG TITLE'
      },
      songs: [
        {
          title: 'A new beginning',
          artist: 'Ben Sound',
          src: require('./assets/bensound-anewbeginning.mp3')
        },
        {
          title: 'Creative Minds',
          artist: 'Ben Sound',
          src: require('./assets/bensound-creativemings.mp3')
        },
        {
          title: 'Ukulele',
          artist: 'Ben Sound',
          src: require('./assets/bensound-ukulele.mp3')
        }
      ]

    }
  }
}


</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
}

header {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 15px;
  background-color: #212121;
  color: white;
}

</style>
