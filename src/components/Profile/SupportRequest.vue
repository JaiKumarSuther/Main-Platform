<template>
  <div class="mysupportReq-container">
    <h2>My Support Tickets</h2>

    <div class="filter-bar">
      <div class="tabs">
        <button class="tab active">open</button>
        <button class="tab">closed</button>
      </div>
      <button class="sort-btn">
        <span class="icon"
          ><img src="/src/images/sort by icon.svg" alt=""
        /></span>
        sort by
      </button>
    </div>

    <div class="supportReq-card">
      <div class="details">
        <div class="label open">Open</div>
        <span class="name"
          >Urgent Issue with my tour booking as the operator is asking me to
          cancel the booking.</span
        >
      </div>
    </div>

    <div class="supportReq-card">
      <div class="details">
        <div class="label open">Open</div>
        <span class="name">Some Problem</span>
      </div>
    </div>
  </div>
</template>
