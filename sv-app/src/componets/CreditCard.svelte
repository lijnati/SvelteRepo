<script>
    import CreditCard from "svelte-credit-cards"; 

    let number = ""; 
    let name = "";
    let cvc = ""; 
    let expiry = "";
  </script>


  <div>
    <label for="number">Number</label>
    <input bind:value="{number}" name="number" id="number" />
  </div>
  <div>
    <label for="name">Name</label>
    <input bind:value="{name}" name="name" id="name" />
  </div>
  <div>
    <label for="cvc">CVC</label>
    <input bind:value="{cvc}" name="cvc" id="cvc" maxlength="3" />
  </div>
  <div>
    <label for="expiry">Exp.</label>
    <input bind:value="{expiry}" name="expiry" id="expiry" maxlength="4" />
  </div>
  <CreditCard {number} {name} {cvc} {expiry} preview="{true}" />