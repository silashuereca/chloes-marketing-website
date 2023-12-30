<template>
  <div id="stay-in-touch">
    <div class="mb-6 flex items-center gap-3">
      <div
        class="flex-none rounded-full p-1 text-primary-500 bg-primary-500/10"
      >
        <div class="h-1.5 w-1.5 rounded-full bg-current"></div>
      </div>
      <h2 class="uppercase text-xs font-semibold text-gray-400">
        STAY IN TOUCH
      </h2>
    </div>
    <p class="mt-2 text-sm text-gray-600 dark:text-gray-400">
      Get notified when I publish something new, and unsubscribe at any time.
    </p>
    <div class="flex items-center gap-3 mt-6">
      <form name="contact" method="POST" data-netlify="true" class="w-full">
        <label class="block text-sm font-medium leading-6 text-gray-900 w-full">Your Name: <input type="text" name="name" required class="block w-full rounded-md border-0 py-1.5 px-2 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-green-600 sm:text-sm sm:leading-6" /></label>
        <label class="block text-sm font-medium leading-6 text-gray-900 w-full mt-4">Your Email: <input type="email" name="email" required class="block w-full rounded-md border-0 py-1.5 px-2 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-green-600 sm:text-sm sm:leading-6" /></label>
        <label class="block text-sm font-medium leading-6 text-gray-900 w-full mt-4">Message: <textarea name="message" rows="4" required class="block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-green-600 sm:text-sm sm:leading-6"></textarea></label>
        <button type="submit" class="mt-4 rounded-md bg-green-600 px-2.5 py-1.5 text-sm font-semibold text-white shadow-sm hover:bg-green-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Send</button>
      </form>
    </div>
  </div>
</template>
