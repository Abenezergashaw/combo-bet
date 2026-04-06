<script setup>
// Define dynamic, high-ranking SEO variables
const title = "ComboBet Ethiopia | #1 Online Football Betting & Virtual Games";
const description =
  "Join ComboBet Ethiopia for the best football betting odds, virtual games, and exclusive cashback bonuses. Fast Telebirr & CBE payouts with 24/7 gaming.";
const siteUrl = "https://www.combobet.bet";

useHead({
  htmlAttrs: {
    lang: "en-ET", // Specifically target Ethiopia
  },
  meta: [
    { name: "viewport", content: "width=device-width, initial-scale=1" },
    { name: "theme-color", content: "#2A2A2A" }, // Matches your brand color
  ],
  link: [
    { rel: "icon", href: "/favicon.ico" },
    { rel: "canonical", href: siteUrl }, // Prevents duplicate content issues
  ],
});

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogUrl: siteUrl,
  ogType: "website",
  ogImage: "/og-image.png", // Recommended: add a social share image in /public
  twitterCard: "summary_large_image",
});
</script>

<template>
  <UApp>
    <UMain>
      <NuxtLayout>
        <NuxtPage />
      </NuxtLayout>
    </UMain>
  </UApp>
</template>

<style>
/* FIX: '.body' targets a class. 
  Usually, you want to target the actual 'body' tag 
  or use your brand background #2A2A2A.
*/
.body {
  background-color: #2a2a2a;
  color: #ffffff;
  margin: 0;
  padding: 0;
}

/* Custom selection color using your brand orange */
::selection {
  background-color: #db7c2e;
  color: white;
}
</style>
