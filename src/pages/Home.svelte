<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import Welcome from "../components/Welcome.svelte";
  import CharityList from "../components/CharityList.svelte";
  import Promo from "../components/Promo.svelte";

  import { charities } from "../data/charities";
</script>

<Header />

<Welcome />
<CharityList {charities} />
<Promo />

<Footer />
