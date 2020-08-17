<template>
  <div id="app">
    <app-header :items="items"></app-header>
    <app-product :items="items"></app-product>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Products from "./components/Products.vue";
export default {
  name: "App",
  components: {
    appHeader: Header,
    appProduct: Products,
  },
  data() {
    return {
      items: [
        {
          id: 1,
          image:
            "https://vlebazaar.in/image/cache/catalog//B07C2VJFDW/boAt-Rockerz-255-Sports-Bluetooth-Wireless-Earphone-with-Immersive-Stereo-Sound-and-Hands-Free-Mic-Neon-B07C2VJFDW-22-550x550.jpg",
          title: "Boat Earphones",
          desc: "boAt BassHeads 100 in-Ear Wired Earphones with Super...",
        },
        {
          id: 2,
          title: "Apple Earpods",
          image:
            "https://i.insider.com/581114e25124c9f370201c55?width=1100&format=jpeg&auto=webp",
          desc: "Apple 100 in-Ear Wired Earpods with Super...",
        },
        {
          id: 3,
          title: "Samsung Galaxy A1",
          image:
            "https://i.gadgets360cdn.com/large/samsung_galaxy_a50_front_ndtv_1551965564020.jpg",
          desc: "Samsung Galaxy A50s Prism Crush Black...",
        },
        {
          id: 4,
          title: "JBL Speaker",
          image:
            "https://cnet4.cbsistatic.com/img/UHrOFAX8ruHfUiV6BPtLGzPgFV0=/868x488/2013/03/29/a4f4f728-67c2-11e3-a665-14feb5ca9861/JBL_Charge_blue_35613369_04.jpg",
          desc: "All-in-one Soundbar with built-in Dual Bass Port design...",
        },
        {
          id: 5,
          title: "Laptop HP Pavillion",
          image:
            "https://www.windowscentral.com/sites/wpcentral.com/files/styles/w1600h900crop/public/field/image/2019/12/hp-laptop-hero.jpg",
          desc: "The right laptop for a college student depends...",
        },
        {
          id: 6,
          title: "MI LED",
          image:
            "https://5.imimg.com/data5/VO/WZ/QR/SELLER-86986427/mi-led-tv-4-pro-138-88-cm-55-ultras-hd-android-tv-500x500.jpg",
          desc: "Overall the Mi TV 4X 43-inch is a good package...",
        },
        {
          id: 7,
          title: "Sony LED",
          image:
            "https://resize.indiatvnews.com/en/resize/newbucket/715_-/2020/05/sony-bravia-new-1590490254.jpg",
          desc: "Overall the Sony TV 4X 43-inch is a good package...",
        },
        {
          id: 8,
          title: "Power Bank",
          image:
            "https://gadgetviper.com/blog/wp-content/uploads/2017/09/AUKEY-sk-a2-power-bank-bluetooth-speaker-1.jpg",
          desc: "Overall the bluetooth power bank is a good package...",
        },
      ],
    };
  },
};
</script>
