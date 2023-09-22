
<script>
    // @ts-ignore
    import Form from './Form.svelte';
  
    let formData = null;
  
    // @ts-ignore
    function handleFormSubmit(data) {
      // Handle the form data received from the child component
      formData = data;
      console.log('Form Data:', formData);
    }
  </script>
  
  <main>
    <!-- Other content or components -->
    <h1>Create Something</h1>
  
    <!-- Include the Form component here and handle form submission -->
    <Form on:submit={handleFormSubmit} />
  </main>
  