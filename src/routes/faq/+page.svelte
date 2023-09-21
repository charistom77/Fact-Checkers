<script>
    import { AccordionItem, Accordion } from 'flowbite-svelte';
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

  
  <Accordion>
    <AccordionItem>
      <span slot="header">My Header 1</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p>
    </AccordionItem>

    <AccordionItem>
      <span slot="header">What is the site about</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p>
    </AccordionItem>

    <AccordionItem>
      <span slot="header">How can i partae</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p>
    </AccordionItem>

    <AccordionItem>
      <span slot="header">What can i do to improve my knowlwdgw in programing</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p>
    </AccordionItem>

    <AccordionItem>
      <span slot="header">How can i partae</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p>
    </AccordionItem>

    <AccordionItem>
      <span slot="header">What is the most porpular frame work</span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo ab necessitatibus sint explicabo ...</p>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Learn more about these technologies:</p>
      <ul class="list-disc pl-5 dark:text-gray-400 text-gray-500">
        <li>
          <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> Lorem ipsum </a>
        </li>
        <li>
          <a href="https://tailwindui.com/" rel="noreferrer" target="_blank" class="text-blue-600 dark:text-blue-500 hover:underline"> Tailwind UI </a>
        </li>
      </ul>
    </AccordionItem>
  </Accordion>
