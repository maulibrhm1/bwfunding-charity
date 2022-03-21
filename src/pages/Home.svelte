<script>
  import { onDestroy } from "svelte";
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import Welcome from "../components/Welcome.svelte";
  import CharityList from "../components/CharityList.svelte";
  import Promo from "../components/Promo.svelte";
  import BackToTop from "../components/BackToTop.svelte";

  onDestroy(function () {
    window.scrollTo(0, 0);
  });
</script>

<BackToTop />
<Header />

<Welcome />
<CharityList />
<Promo />

<Footer />
