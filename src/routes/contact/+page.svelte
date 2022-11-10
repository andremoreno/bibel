<svelte:head>
    <title>Kontak</title>
</svelte:head>

<div class="max-w-screen-md mx-auto">
  <div class="text-center mb-10">
      <h3 class="text-3xl sm:text-4xl leading-normal font-extrabold tracking-tight text-gray-900">
        Kontak <span class="text-indigo-600">Kami</span>
      </h3>
  </div>


  <form action="/thanks" id="contact-form" name="contact-form" class="w-full" method="POST" netlify-honeypot="hpfield" data-netlify="true">
  <input type="hidden" name="form-name" value="contact-form">
  <input class="invisible" name="hpfield">
  <div class="flex flex-wrap -mx-3 mb-6">
    <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
      <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
        First Name
      </label>
      <input class="peer appearance-none block w-full text-gray-700 border border-gray-200 rounded py-3 px-4 mb-1 leading-tight focus:outline-none" name="first-name" type="text" required>
      <p class="invisible peer-invalid:visible text-red-700 font-light text-xs">Please enter your first name</p>
    </div>
    <div class="w-full md:w-1/2 px-3">
      <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-last-name">
        Last Name
      </label>
      <input class="peer appearance-none block w-full text-gray-700 border border-gray-200 rounded py-3 px-4 mb-1 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" name="last-name" type="text" required>
      <p class="invisible peer-invalid:visible text-red-700 font-light text-xs">Please enter your last name</p>
    </div>
  </div>
  <div class="flex flex-wrap -mx-3 mb-6">
    <div class="w-full px-3">
      <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-password">
        Email Address
      </label>
      <input class="peer appearance-none block w-full text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:border-gray-500" name="email" type="email" placeholder="********@*****.**" required>
      <p class="invisible peer-invalid:visible text-red-700 font-light text-xs">Please enter your email</p>
    </div>
  </div>
    
    <div class="flex flex-wrap -mx-3 mb-6">
    <div class="w-full px-3">
      <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-password">
        Your Message
      </label>
      <textarea rows="8" name="message" class="peer appearance-none block w-full text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:border-gray-500" required></textarea>
      <p class="peer invisible peer-invalid:visible text-red-700 font-light text-xs">Please enter your message</p>
    </div>
    <div class="flex justify-between w-full px-3">
      <div class="md:flex md:items-center">
        &nbsp;
      </div>
      <button class="shadow focus:shadow-outline focus:outline-none text-indigo-600 bg-gray-100 font-semibold hover:bg-indigo-600 hover:text-white transition duration-500 ease-in-out py-2 px-6 rounded" type="submit">
        Send Message
      </button>
    </div>
      
  </div>
    
</form>
</div>