<script>
// @ts-nocheck

	import ToolbarGroup from './../../../node_modules/flowbite-svelte/dist/toolbar/ToolbarGroup.svelte';
	import { Input, Label } from 'flowbite-svelte';
  import { Textarea, Toolbar, ToolbarButton, Button } from 'flowbite-svelte';
  import { PaperClipOutline, MapPinAltSolid, ImageOutline, CodeOutline, FaceGrinOutline, PapperPlaneOutline } from 'flowbite-svelte-icons';




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
    <div>
      <Label align="center" for="first_name" class="mb-2">Create your News</Label>
    </div>

    <label for="title" class="sr-only">Title</label>
    <input type="text" name="title" id="title" class="block w-full border-0 pt-2.5 text-lg font-medium placeholder:text-gray-400 focus:ring-0" placeholder="Title">
    <label for="description" class="sr-only">Description</label>

    <div>
      <label for="editor" class="sr-only" placeholder="type news" required>Publish post</label>
      <Textarea id="editor" rows="8" class="mb-4" placeholder="Write a comment">
        <Toolbar slot="header" color="bind:black" embedded>
          <ToolbarGroup>
            <ToolbarButton name="Attach file"><PaperClipOutline class="w-5 h-5 rotate-45" /></ToolbarButton>
            <ToolbarButton name="Embed map"><MapPinAltSolid class="w-5 h-5" /></ToolbarButton>
            <ToolbarButton name="Upload image"><ImageOutline class="w-5 h-5" /></ToolbarButton>
          </ToolbarGroup>
          <ToolbarGroup>
            <ToolbarButton name="Format code"><CodeOutline class="w-5 h-5" /></ToolbarButton>
            <ToolbarButton name="Add emoji"><FaceGrinOutline class="w-5 h-5" /></ToolbarButton>
          </ToolbarGroup>
          <ToolbarButton name="send" slot="end"><PapperPlaneOutline class="w-5 h-5 rotate-45" /></ToolbarButton>
        </Toolbar>
      </Textarea>
    </div>
  <Button type="submit">Submit</Button>
</div>
</form>
