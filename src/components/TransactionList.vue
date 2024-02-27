<script setup>
  const transactions = [
    { id: 1, text: "Flower", amount: -19.99 },
    { id: 2, text: "Cake", amount: -10.99 },
    { id: 3, text: "Camera", amount: -500.0 },
  ];
</script>

<template>
  <h3>History</h3>
  <ul id="list" class="list">
    <li
      v-for="transaction in transactions"
      :key="transaction.id"
      :class="transaction.amount < 0 ? 'minus' : 'plus'"
    >
      Cash <span>{{ transaction.amount }}</span
      ><button class="delete-btn">x</button>
    </li>
  </ul>
</template>
