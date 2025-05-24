<template>
  <div class="payments-container">
    <h2>My payments & refunds</h2>

    <div class="filter-bar">
      <div class="tabs">
        <button class="tab">Payments</button>
        <button class="tab active">Refunds</button>
      </div>
    </div>

    <div class="Payments-table-container">
      <table>
        <thead>
          <tr>
            <th>Date</th>
            <th>Booking ID</th>
            <th>Amount</th>
            <th>Status</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>25 Sep 2025</td>
            <td>TN1239-2391</td>
            <td class="amount">434,000</td>
            <td class="status">Processed</td>
          </tr>
          <tr>
            <td>2 Nov 2025</td>
            <td>TN1486-1957</td>
            <td class="amount">95,002</td>
            <td class="status">Processed</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
