<template>
  <div>
      <Head>
        <Title>LD Legenda Kozi Square Apartment Kuching | LD Legenda @ Kozi Square for Sale & Rent</Title>
        <Meta name="description" :content='"Explore a wide range of real estate options for sale and rent. Find your perfect property with our expert guidance."' />
      </Head>
    </div>
  <div>
    <div class="space-y-12">
      <MainBanner />
      <section>
    
      </section>

    
    </div>
  </div>
</template>

<script>
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
};
</script>

<script setup>

function currentDateAndTime() {
  const months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
  const current = new Date();
  let hours = current.getHours();
  let minutes = current.getMinutes();
  let seconds = current.getSeconds();

  // Add leading zeros if hours, minutes or seconds are less than 10
  hours = (hours < 10) ? "0" + hours : hours;
  minutes = (minutes < 10) ? "0" + minutes : minutes;
  seconds = (seconds < 10) ? "0" + seconds : seconds;

  const date = `${current.getDate()} ${months[current.getMonth()]} ${current.getFullYear()} || ${hours}:${minutes}:${seconds}`;
  return date;
}


function oneMonthAgo() {
  const months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
  const current = new Date();
  current.setMonth(current.getMonth() - 1);
  const date = `${current.getDate()} ${months[current.getMonth()]} ${current.getFullYear()}`;
  return date;
}

function twoMonthsAgo() {
  const months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
  const current = new Date();
  current.setMonth(current.getMonth() - 2);
  const date = `${current.getDate()} ${months[current.getMonth()]} ${current.getFullYear()}`;
  return date;
}

function twoWeeksAgo() {
  const months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
  const current = new Date();
  current.setDate(current.getDate() - 14);
  const date = `${current.getDate()} ${months[current.getMonth()]} ${current.getFullYear()}`;
  return date;
}

</script>
