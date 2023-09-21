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

  <script>
    import { Card } from 'flowbite-svelte';
  </script>
  
  <Card  padding="none" size="xl" class="grid md:grid-cols-2">
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-t-lg border-b border-gray-200 md:rounded-t-none md:rounded-tl-lg md:border-r dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Very easy this was to integrate</h3>
        <p class="my-4 font-light">If you care for your time, I hands down would go with this."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/karen-nelson.png" alt="Karen profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Bonnie Green</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Developer at Open AI</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-tr-lg border-b border-gray-200 dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Solid foundation for any project</h3>
        <p class="my-4 font-light">Designing with Figma components that can be easily translated to the utility classes of Tailwind CSS is a huge timesaver!"</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/roberta-casas.png" alt="Robert profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Roberta Casas</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Lead designer at Dropbox</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-bl-lg border-b border-gray-200 md:border-b-0 md:border-r dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Mindblowing workflow</h3>
        <p class="my-4 font-light">Aesthetically, the well designed components are beautiful and will undoubtedly level up your next application."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/jese-leos.png" alt="Jese profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Jese Leos</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Software Engineer at Facebook</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-b-lg border-gray-200 md:rounded-br-lg dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Efficient Collaborating</h3>
        <p class="my-4 font-light">You have many examples that can be used to create a fast prototype for your team."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/joseph-mcfall.png" alt="joseph profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Joseph McFall</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">CTO at Google</div>
        </div>
      </figcaption>
    </figure>
  </Card>

  <Card  padding="none" size="xl" class="grid md:grid-cols-2">
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-t-lg border-b border-gray-200 md:rounded-t-none md:rounded-tl-lg md:border-r dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Very easy this was to integrate</h3>
        <p class="my-4 font-light">If you care for your time, I hands down would go with this."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/karen-nelson.png" alt="Karen profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Bonnie Green</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Developer at Open AI</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-tr-lg border-b border-gray-200 dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Solid foundation for any project</h3>
        <p class="my-4 font-light">Designing with Figma components that can be easily translated to the utility classes of Tailwind CSS is a huge timesaver!"</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/roberta-casas.png" alt="Robert profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Roberta Casas</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Lead designer at Dropbox</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-bl-lg border-b border-gray-200 md:border-b-0 md:border-r dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Mindblowing workflow</h3>
        <p class="my-4 font-light">Aesthetically, the well designed components are beautiful and will undoubtedly level up your next application."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/jese-leos.png" alt="Jese profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Jese Leos</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">Software Engineer at Facebook</div>
        </div>
      </figcaption>
    </figure>
    <figure class="flex flex-col justify-center items-center p-8 text-center bg-white rounded-b-lg border-gray-200 md:rounded-br-lg dark:bg-gray-800 dark:border-gray-700">
      <blockquote class="mx-auto mb-4 max-w-2xl text-gray-500 dark:text-gray-400">
        <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Efficient Collaborating</h3>
        <p class="my-4 font-light">You have many examples that can be used to create a fast prototype for your team."</p>
      </blockquote>
      <figcaption class="flex justify-center items-center space-x-3">
        <img class="w-9 h-9 rounded-full" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/joseph-mcfall.png" alt="joseph profile" />
        <div class="space-y-0.5 font-medium dark:text-white text-left">
          <div>Joseph McFall</div>
          <div class="text-sm font-light text-gray-500 dark:text-gray-400">CTO at Google</div>
        </div>
      </figcaption>
    </figure>
  </Card>