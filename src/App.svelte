<script lang="ts">
  import router from "page";
  import Router from "svelte-spa-router";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  import Contact from "./pages/Contact.svelte";
  import Donation from "./pages/Donation.svelte";
  import NotFound from "./pages/NotFound.svelte";
  import Success from "./pages/Success.svelte";

  let params;
  let routes = {
    "/": Home,
    "/about": About,
    "/donation/:id": Donation,
    "/contact": Contact,
    "/Success": Success,

    "*": NotFound,
  };
</script>

<main>
  <Router {routes} />
</main>
