<template>
  <section class="bg-[#816c65]">
    <div class="flex flex-col items-center w-2/3 py-10 my-0 mx-auto">
      <h4 class="text-3xl font-normal text-white mb-1">
        Let's be friends! Subscribe to be among the first to learn about our new
        products and promotions:
      </h4>

      <form action="#" id="newsletter" method="POST">
        <div class="flex flex-col">
          <input
            type="text"
            class="p-4 my-2"
            id="newsletter_email"
            value=""
            placeholder="Your email address"
          />
          <span class="text-white italic my-3">
            Please, mark the check box below in order to be allowed to join.
          </span>
        </div>

        <div class="text-sm">
          <input
            class="cursor-pointer w-3 h-3 bg-white"
            type="checkbox"
            id="newsletter_check"
          />
          <label class="text-white">
            I agree that the email I provide will be used to receive
            notifications for news, gifts and future promotions related to
            COCOSOLIS products in accordance with the Terms of use of the
            website and Privacy Policy*
          </label>
        </div>

        <input
          type="submit"
          class="text-white w-full h-8"
          id="signup_home_submit"
          value="JOIN THE CLUB"
        />
      </form>
    </div>
  </section>
</template>
