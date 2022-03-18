<script>
  import { onMount } from "svelte";
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import Welcome from "../components/Welcome.svelte";
  import CharityList from "../components/CharityList.svelte";
  import Promo from "../components/Promo.svelte";

  let charities = [];

  onMount(async function () {
    const res = await fetch("http://charity-api-bwa.herokuapp.com/charities");
    charities = await res.json();
  });
</script>

<Header />

<Welcome />
<CharityList {charities} />
<Promo />

<Footer />
