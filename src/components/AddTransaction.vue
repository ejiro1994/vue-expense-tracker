<template>
  <h3>Add new transaction</h3>
  <form id="form">
    <div class="form-control">
      <label for="text">Text</label>
      <input type="text" id="text" placeholder="text" />
    </div>
    <div class="form-control">
        <label for="amount">Amount</label>
        <input type="number" id="amount" placeholder="amount">
        <button class="btn">Add transaction</button>
    </div>
  </form>
</template>