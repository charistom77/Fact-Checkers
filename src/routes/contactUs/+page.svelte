<script>
    import { Drawer, Button, CloseButton, Label, Input, Textarea, P, A, Checkbox } from 'flowbite-svelte';
    import { InfoCircleSolid } from 'flowbite-svelte-icons';
    import { sineIn } from 'svelte/easing';
  
    let hidden3 = true;
    let transitionParams = {
      x: -320,
      duration: 200,
      easing: sineIn
    };
  </script>

<div class="sm:hidden">
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
  
  <div class="text-center">
    <Button on:click={() => (hidden3 = false)}>Show contact form</Button>
  </div>
  <Drawer transitionType="fly" {transitionParams} bind:hidden={hidden3} id="sidebar3">
    <div class="flex items-center">
      <h5 id="drawer-label" class="inline-flex items-center mb-6 text-base font-semibold text-gray-500 uppercase dark:text-gray-400">
        <InfoCircleSolid class="w-4 h-4 mr-2.5" />Contact us
      </h5>
      <CloseButton on:click={() => (hidden3 = true)} class="mb-4 dark:text-white" />
    </div>
    <form action="#" class="mb-6">
      <div class="mb-6">
        <Label for="email" class="block mb-2">Your email</Label>
        <Input id="email" name="email" required placeholder="name@company.com" />
      </div>
      <div class="mb-6">
        <Label for="subject" class="block mb-2">Subject</Label>
        <Input id="subject" name="subject" required placeholder="Let us know how we can help you" />
      </div>
      <div class="mb-6">
        <Label for="message" class="mb-2">Your message</Label>
        <Textarea id="message" placeholder="Your message..." rows="4" name="message" />
      </div>
      <Button type="submit" class="w-full">Send message</Button>
    </form>
    <P class="mb-2 text-sm text-gray-500 dark:text-gray-400">
      <A href="/" class="text-primary-600 hover:underline dark:text-primary-500">info@company.com</A>
    </P>
    <P class="text-sm text-gray-500 dark:text-gray-400">
      <A href="/" class="text-primary-600 hover:underline dark:text-primary-500">212-456-7890</A>
    </P>
  </Drawer>