<!-- Form.svelte -->

<script>
    let title = "";
    let description = "";
  
    function handleSubmit() {
      // Create an object to store the form data
      const formData = {
        title,
        description,
      };
  
      // You can do something with the formData here, such as sending it to a server
      // or storing it locally.
      console.log("Form Data:", formData);
  
      // Clear the form fields after submission (optional)
      title = "";
      description = "";
    }
  </script>
  
  <form on:submit={handleSubmit} class="relative">
    <div class="overflow-hidden rounded-lg border border-gray-300 shadow-sm focus-within:border-indigo-500 focus-within:ring-1 focus-within:ring-indigo-500">
      <label for="title" class="sr-only">Title</label>
      <input type="text" bind:value={title} id="title" class="block w-full border-0 pt-2.5 text-lg font-medium placeholder:text-gray-400 focus:ring-0" placeholder="Title">
      <label for="description" class="sr-only">Description</label>
      <textarea rows="2" bind:value={description} id="description" class="block w-full resize-none border-0 py-0 text-gray-900 placeholder:text-gray-400 focus:ring-0 sm:text-sm sm:leading-6" placeholder="Write a description..."></textarea>
    </div>
  
    <div class="absolute inset-x-px bottom-0">
      <div class="flex items-center justify-between space-x-3 border-t border-gray-200 px-2 py-2 sm:px-3">
        <div class="flex">
          <button type="button" class="group -my-2 -ml-2 inline-flex items-center rounded-full px-3 py-2 text-left text-green-400" onclick="askForLink()">
            <svg class="-ml-1 mr-2 h-5 w-5 group-hover:text-green-500" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
              <path fill-rule="evenodd" d="M15.621 4.379a3 3 0 00-4.242 0l-7 7a3 3 0 004.241 4.243h.001l.497-.5a.75.75 0 011.064 1.057l-.498.501-.002.002a4.5 4.5 0 01-6.364-6.364l7-7a4.5 4.5 0 016.368 6.36l-3.455 3.553A2.625 2.625 0 119.52 9.52l3.45-3.451a.75.75 0 111.061 1.06l-3.45 3.451a1.125 1.125 0 001.587 1.595l3.454-3.553a3 3 0 000-4.242z" clip-rule="evenodd" />
            </svg>
            <span class="text-sm italic text-white-500 group-hover:text-green-600">Attach a link</span>
          </button>
        </div>
        <div class="flex-shrink-0">
          <button type="submit" class="inline-flex items-center rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Create</button>
        </div>
      </div>
    </div>
  </form>
  