<template>
    <h1>this is rahelpage template!</h1>
    <h2> This should be…</h2>
    <p>Title: <br>{{data.title}}</p>
    <p>Titelbild: <br><img :src="$withBase(data.heroImage)" alt="hero"></p>
    <p>Bildunterschrift: <br>{{data.bildunterschrift}}</p>
    <p>INhalt: <br>{{data.inhalt}}</p>
    

</template>

<script>
export default {
  computed: {
    data() {
      return this.$page.frontmatter;
    }
  }
};
</script>


// 