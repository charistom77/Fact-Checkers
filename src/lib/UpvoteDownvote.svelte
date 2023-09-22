<script>
    import { writable } from 'svelte/store';
  
    // Create writable stores for upvotes and downvotes
    const upvoteStore = writable(0);
    const downvoteStore = writable(0);
  
    // Initialize variables to track whether a user has voted
    let upvoted = false;
    let downvoted = false;
  
    // Function to handle upvote
    function handleUpvote() {
      if (!upvoted) {
        // If not already upvoted, increment upvote count
        upvoteStore.update((n) => n + 1);
        upvoted = true;
  
        // If previously downvoted, cancel the downvote
        if (downvoted) {
          downvoteStore.update((n) => n - 1);
          downvoted = false;
        }
      }
    }
  
    // Function to handle downvote
    function handleDownvote() {
      if (!downvoted) {
        // If not already downvoted, increment downvote count
        downvoteStore.update((n) => n + 1);
        downvoted = true;
  
        // If previously upvoted, cancel the upvote
        if (upvoted) {
          upvoteStore.update((n) => n - 1);
          upvoted = false;
        }
      }
    }
  </script>
  
  <style>
    /* Add CSS styles as needed */
    .icon-button {
      display: inline-flex;
      align-items: center;
      padding: 8px 12px;
      margin: 20px; /* Add a margin of 20px on all sides */
      background-color: #007bff; /* Button background color */
      color: #fff; /* Text color */
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
  
    .icon {
      margin-right: 8px; /* Adjust spacing between icon and text */
    }
  </style>
  
  <!-- Include the FontAwesome library in your HTML if you haven't already -->
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    integrity="sha512-dTzgd/2n1jv0e5D8Fszaxv2Ga8nQNK5a6oq5FzChZ1nOm4KcNxSJ8wJqZfM0VfBDC7BnKjM6stv7sfE4vOCblfw=="
    crossorigin="anonymous"
  />
  
  <!-- Upvote button with count -->
  <button class="icon-button" on:click={handleUpvote}>
    <span class="icon"><i class="fas fa-thumbs-up"></i></span>
    Upvote ({$upvoteStore})
  </button>
  
  <!-- Downvote button with count -->
  <button class="icon-button" on:click={handleDownvote}>
    <span class="icon"><i class="fas fa-thumbs-down"></i></span>
    Downvote ({$downvoteStore})
  </button>
  