<script>
  export let segment;
</script>

<style lang="scss">
  @import "../style/themes.scss";
  nav {
    border-bottom: 1px solid rgba(255, 62, 0, 0.1);
    font-weight: 300;
    padding: 0 1em;
    position: sticky;
    top: 0;
    z-index: 2;
    background-color:#3b3b3b;
    color: gainsboro;
      display: flex;
      justify-content: space-between;
      align-items:center;
    ul {
      margin: 0;
      padding: 0;
    }
    /* clearfix */
    ul::after {
      content: "";
      display: block;
      clear: both;
    }

    li {
      display: block;
      float: left;
      text-transform: capitalize;
    }

    [aria-current] {
      position: relative;
      display: inline-block;
      color: $accent;
    }

    [aria-current]::after {
      position: absolute;
      content: "";
      width: calc(100% - 1em);
      height: 3px;
      background-color:$accent;
      display: block;
      bottom: -1px;
    }

    a {
      text-decoration: none;
      padding: 1em 0.5em;
      display: block;
    }
    .site-logo {
      font-size: 1.2em;
      font-weight: bold;
      font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
      padding: 0;
        color: white;
      &:hover {
        color: $accent;
      }
    }
  }


</style>

<nav>
  <a href="." class="site-logo">
    SeanParker.dev
  </a>
  
  <ul>
    <li>
      <a
        aria-current="{segment === 'portfolio' ? 'page' : undefined}"
        href="portfolio"
        >portfolio</a
      >
    </li>
    <li>
      <a
        aria-current="{segment === 'resume' ? 'page' : undefined}"
        href="resume"
        >resume</a
      >
    </li>

    <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
          the blog data when we hover over the link or tap it on a touchscreen -->
    <li>
      <a
        rel="prefetch"
        aria-current="{segment === 'blog' ? 'page' : undefined}"
        href="blog"
        >blog</a
      >
    </li>
  </ul>
</nav>
