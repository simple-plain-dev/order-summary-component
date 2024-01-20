<script lang="ts">
  import banner from "$lib/images/illustration-hero.svg"
  import musicIcon from "$lib/images/icon-music.svg"
</script>

<main>
  <img src={banner} alt="banner" class="banner">
  <section class="content">
    <header class="overview">
      <h1>Order Summary</h1>
      <p>You can listen to millions of songs, audiobooks, and podcast on any device anywhere you like!</p>
    </header>
    <div class="plan">
      <img src={musicIcon} alt="music icon" class="icon">
      <p class="bold plan-period">Annual Plan</p>
      <p class="plan-price">$59.99/year</p>
      <a class="plan-action bold" href="#" >Change</a>
    </div>
    <footer class="action">
      <button class="order">Proceed to Payment</button>
      <button class="cancel">Cancel Order</button>
    </footer>
  </section>
</main>

<style>
  main {
    background-color: var(--clr-neutral-1);
    margin: 2rem;
    border-radius: 1rem;
    overflow: hidden;
    max-width: 20rem;
  }

  .content {
    padding: 2rem;
    line-height: 1.5rem;
    text-align: center;
  }

  .overview{
    display: grid;
    gap: 1rem;
  }

  h1 {
    font-weight: var(--fw-bolder);
  }

  p {
    color: var(--clr-neutral-2);
  }

  .plan {
    display: grid;
    grid-template-columns: auto 1fr auto;
    grid-template-rows: 1fr 1fr;
    align-items: center;
    margin-block: 2rem;
  }

  .icon {
    grid-row: 1/3;
  }

  h1, .plan-period{
    color: var(--clr-neutral-3);
  }

  .bold {
    font-weight: var(--fw-bold);
  }

  .plan-price {
    grid-column: 2/3;
    grid-row: 2/3;
  }

  .plan-action {
    grid-column: 3/4;
    grid-row: 1/3;
  }

  .action {
    display: grid;
    gap: 0.5rem;
  }

  button {
    border: transparent;
    padding: 1rem;
    border-radius: 1rem;
  }

  .order {
    background-color: var(--clr-primary-2);
    font-weight: var(--fw-bold);
    color: var(--clr-neutral-1);
  }

  .order:hover{
    opacity: 0.8;
  }

  .cancel {
    font-weight: var(--fw-bold);
    background-color: var(--clr-neutral-1);
    color: var(--clr-neutral-2)
  }

  .cancel:hover {
    color: var(--clr-neutral-4);
  }

</style>