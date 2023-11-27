<template>
  <div>
    <div>
      <Head>
        <Title>Contact LD Legenda Kozi Square Apartment Kuching | LD Legenda @ Kozi Square for Sale & Rent</Title>
        <Meta name="description" :content='"Contact us for more info"' />
      </Head>
      
    </div>

    <div class="py-8 select-none bg-gradient-to-b from-theme-500 to-theme-200 pb-20 h-10">
          <div class="text-xl font-semibold text-center text-white sm:text-4xl">
          Contact Us
        </div>
      </div>
    <section>
      <div class="max-w-6xl px-4 py-12 mx-auto space-y-6">
        <form-book-appoinment />
      </div>
    </section>
  </div>
</template>

<script>

import FormBookAppoinment from '~/components/FormBookAppoinment.vue'
export default {
  mounted() {
    // Load Google Analytics script
    const script = document.createElement('script');
    script.async = true;
    script.src = 'https://www.googletagmanager.com/gtag/js?id=G-JS59WSZ932';
    document.head.appendChild(script);

    script.onload = () => {
      // Initialize Google Analytics after script has loaded
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-JS59WSZ932');
    };
  },
  
  components: { FormBookAppoinment },
}
</script>
