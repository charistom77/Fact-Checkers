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