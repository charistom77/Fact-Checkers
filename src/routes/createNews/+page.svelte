<script>
// @ts-nocheck

	import ToolbarGroup from './../../../node_modules/flowbite-svelte/dist/toolbar/ToolbarGroup.svelte';
	import { Input, Label } from 'flowbite-svelte';
  import { Textarea, Toolbar, ToolbarButton, Button } from 'flowbite-svelte';
  import { PaperClipOutline, MapPinAltSolid, ImageOutline, CodeOutline, FaceGrinOutline, PapperPlaneOutline } from 'flowbite-svelte-icons';
  
</script>

<div class="sm:hidden" margin-button="50px" >
  <label for="tabs" class="sr-only">Select your country</label>
  <select id="tabs" class="bg-white-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
      <option>Profile</option>
      <option>Canada</option>
      <option>France</option>
      <option>Germany</option>
  </select>
</div>
<ul class="hidden text-sm font-medium text-center text-dark-500 divide-x divide-gray-200 rounded-lg shadow sm:flex dark:divide-gray-700 dark:text-gray-400">
  <li class="w-full">
      <a href="accunt" class="inline-block w-full p-4 text-gray-900 bg-gray-100 rounded-l-lg focus:ring-4 focus:ring-blue-300 active focus:outline-none dark:bg-gray-700 dark:text-white" aria-current="page">Profile</a>
  </li>
  <li class="w-full">
      <a href="dashboard" class="inline-block w-full p-4 bg-white hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:ring-blue-300 focus:outline-none dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">Dashboard</a>
  </li>
  <li class="w-full">
      <a href="createNews" class="inline-block w-full p-4 bg-white hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:ring-blue-300 focus:outline-none dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">Create News</a>
  </li>
  <li class="w-full">
      <a href="viewNews" class="inline-block w-full p-4 bg-white rounded-r-lg hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">View News</a>
  </li>
  <li class="w-full">
    <a href="faq" class="inline-block w-full p-4 bg-white rounded-r-lg hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">FAQs</a>
</li>
<li class="w-full">
  <a href="contactUs" class="inline-block w-full p-4 bg-white rounded-r-lg hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">Contact Us</a>
</li>
</ul>


<form action="#" class="relative">
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
