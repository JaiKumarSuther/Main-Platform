<template>
  <div class="supportTicket-cont">
    <h2>What do you need help with?</h2>
    <form>
      <div class="form-group">
        <label for="title">Write a descriptive title</label>
        <input
          type="text"
          id="title"
          placeholder="I'm having trouble with..."
          maxlength="100"
          required
        />
      </div>
      <div class="form-group">
        <label for="related">Related to</label>
        <select id="related">
          <option value="">select</option>
          <option value="billing">Billing</option>
          <option value="technical">Technical Issue</option>
          <option value="account">Account Access</option>
        </select>
      </div>
      <div class="form-group">
        <label for="issue">Explain the issue</label>
        <textarea id="issue" rows="5" placeholder="" required></textarea>
      </div>

      <div class="attach-photo">
        <img src="/src/images/upload-svgrepo-com.svg" alt="" width="20px" />
        attach photo
      </div>
    </form>
    <button class="open-ticket" type="submit">open ticket</button>
  </div>
</template>
