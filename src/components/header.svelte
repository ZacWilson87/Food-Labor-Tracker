<script>
  import { Router } from "svelte-router-spa";
  import routes from "../routes";
  import { link } from "svelte-router-spa";
</script>

<header>
  <Router {routes} />
  <div class="nav-links">
    <a href="/enter-record" use:link id="newRecord"><p>Create New Record</p></a>
    <a href="/search" use:link id="search"><p>Search</p></a>
  </div>
  <h4 id="headerTitle">Food & Labor Tracker</h4>
</header>
<hr />

<style>
  header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    height: auto;
    border-bottom: 1px;
  }

  header .nav-links {
    margin-left: 3%;
    display: flex;
    flex-direction: row;
    text-decoration: none;
    justify-content: space-between;
    width: 15%;
  }
  .nav-links a {
    text-decoration: none;
    color: rgb(194, 194, 194);
    display: flex;
    flex-direction: row;
  }
  #headerTitle {
    margin-right: 3%;
    color: rgb(194, 194, 194);
  }
  hr {
    width: 98%;
  }
</style>
