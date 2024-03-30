<script>
  let rooms = [
    { name: 'Standard Room', price: '$100', description: 'A cozy room with a comfortable bed.' },
    { name: 'Deluxe Room', price: '$150', description: 'A spacious room with a view.' },
    { name: 'Suite', price: '$200', description: 'Luxurious accommodation with separate living area.' }
  ];
</script>

<main>
  <header>
    <h1>Welcome to Our Hotel</h1>
    <p>Experience comfort and luxury during your stay.</p>
  </header>

  <section>
    <h2>Our Rooms</h2>
    <ul>
      {#each rooms as room}
        <li>
          <h3>{room.name}</h3>
          <p>{room.description}</p>
          <p>{room.price} per night</p>
        </li>
      {/each}
    </ul>
  </section>

  <section>
    <h2>Book Now</h2>
    <p>Plan your stay with us and enjoy our excellent services.</p>
    <a href="/booking" class="button">Book Now</a>
  </section>

  <footer>
    <p>&copy; 2024 Our Hotel. All rights reserved.</p>
  </footer>
</main>

<style>
  main {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }

  header {
    text-align: center;
    margin-bottom: 40px;
  }

  section {
    margin-bottom: 40px;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  li {
    margin-bottom: 20px;
  }

  .button {
    display: inline-block;
    padding: 10px 20px;
    background-color: #007bff;
    color: white;
    text-decoration: none;
    border-radius: 5px;
  }

  footer {
    text-align: center;
    margin-top: 40px;
    padding-top: 20px;
    border-top: 1px solid #ddd;
  }
</style>

