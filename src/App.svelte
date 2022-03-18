<script lang="ts">
  import Router from "svelte-spa-router";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  import Contact from "./pages/Contact.svelte";
  import Donation from "./pages/Donation.svelte";
  import NotFound from "./pages/NotFound.svelte";

  let routes = {
    "/": Home,
    "/about": About,
    "/donation/:id": Donation,
    "/contact": Contact,

    "*": NotFound,
  };
</script>

<main>
  <Router {routes} />
</main>
