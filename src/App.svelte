<script>
  import Landing from "./pages/landing-page.svelte";
  import Header from "./components/header.svelte";
  import Calendar from "./components/calendarSearch.svelte";
  import SearchDisplay from "./components/searchDisplay.svelte";
</script>

<main>
  <Header />
  <Calendar />
  <SearchDisplay />
</main>

<style>
  :root {
    background-color: rgb(70, 70, 70);
  }
</style>
