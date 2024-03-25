<footer>
  <div class="footer-container">
    <p class="footer-paragraph">
      990 Stewart Avenue, 1st Floor
      <br />
      Garden City, NY 11530
      <br />
      customerservice@namadr.com
      <br />
      1-800-358-2550
    </p>

    <p class="footer-paragraph">
      All mediation and arbitration services are coordinated through National
      Mediation and Arbitration.
      <br />
      <br />
      No legal advice given without private retainer.
    </p>

    <p class="footer-paragraph">
      Copyright © 2024 Bob Worden Esq. All Rights Reserved.
    </p>
  </div>
</footer>

<style>
  footer {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    background-color: var(--color-blue-4);
    color: var(--color-gray-2);
  }

  .footer-container {
    column-gap: 1rem;
    width: 100%;
    max-width: var(--page-width);
    display: flex;
    padding: 0rem 1rem;
  }

  .footer-paragraph {
    max-width: 20rem;
  }

  @media (max-width: 720px) {
    .footer-container {
      flex-direction: column;
    }
  }
</style>
