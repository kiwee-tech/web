<!--<svelte:head>-->
<!--  &lt;!&ndash; Global site tag (gtag.js) - Google Analytics &ndash;&gt;-->
<!--&lt;!&ndash;  <script async src="https://www.googletagmanager.com/gtag/js?id=G-CZS9SS5KHG"></script>&ndash;&gt;-->
<!--&lt;!&ndash;  <script>&ndash;&gt;-->
<!--&lt;!&ndash;      window.dataLayer = window.dataLayer || [];&ndash;&gt;-->
<!--&lt;!&ndash;      function gtag(){dataLayer.push(arguments);}&ndash;&gt;-->
<!--&lt;!&ndash;      gtag('js', new Date());&ndash;&gt;-->

<!--&lt;!&ndash;      gtag('config', 'G-CZS9SS5KHG');&ndash;&gt;-->
<!--&lt;!&ndash;  </script>&ndash;&gt;-->
<!--</svelte:head>-->

<script>
    import "../app.css";
</script>

<header class="bg-black text-green-400 bg-opacity-50">
  <nav class="px-6 flex">
    <div class="flex-1">
      <a class="p-2" href="/">
        <span class="sr-only">KiWee</span>
        <img class="h-8 w-auto sm:h-8" src="/k.svg" alt="KiWee">
      </a>
    </div>
    <div class="flex-0 pt-10">
        <a class="p-1 hover:text-green-600" href="/">Home</a>
        <a class="p-1 hover:text-green-600" href="/contact">Contact</a>
        <a class="p-1 hover:text-green-600" href="/blog">Blog</a>
    </div>
  </nav>
</header>

<div class="bg"></div>
<div class="bg bg2"></div>
<div class="bg bg3"></div>

<div class="min-h-screen">
  <slot></slot>
</div>

<footer class="border-t-2 mt-6">
  <div class="flex p-6">
    <div class="flex-1">
      <a href="/">
        <svg viewBox="0 0 500 500" class="w-8 h-8 fill-current">
          <path d="M250 225C194.772 225 150 180.228 150 125C150 69.7715 194.772 25 250 25C305.228 25 350 69.7715 350 125C350 180.228 305.228 225 250 225Z"></path><path d="M125 0H0V385.276C34.859 309.438 103.211 252.184 186.109 232.46C149.515 210.656 125 170.691 125 125V0Z"></path><path d="M500 125C500 263.071 388.071 375 250 375C180.964 375 125 430.964 125 500H0C0 361.929 111.929 250 250 250C319.036 250 375 194.036 375 125H500Z"></path><path d="M313.891 392.539C359.027 381.8 399.852 359.935 433.305 330.001C474.694 374.609 500 434.349 500 500H375C375 454.309 350.485 414.343 313.891 392.539Z"></path>
        </svg>
      </a>
    </div>

    <div class="flex-0 grid grid-cols-3 gap-6">
      <a href="https://www.facebook.com/kiwee.tech" target="_blank">
        <span class="sr-only">Meta</span>
        <svg viewBox="0 0 80 54" fill="none" class="w-8 h-8 fill-current">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M41.085 11.215C45.725 4.94 50.855 0 57.415 0C69.8 0 80 15.765 80.005 34.535C80.005 45.985 75.075 53.16 66.22 53.16C58.505 53.16 54.245 48.83 46.6 36.04L43.265 30.425L42.675 29.44C41.8053 27.9701 40.9219 26.5084 40.025 25.055L34.135 35.455C25.77 50.08 21.06 53.16 14.52 53.16C5.43 53.16 0 46.085 0 34.865C0 16.94 9.975 0 22.99 0C24.585 0 26.115 0.195 27.61 0.61C29.16 1.04 30.665 1.71 32.175 2.645C35.06 4.44 37.945 7.22 41.085 11.215ZM48.665 22.335C47.405 20.285 46.195 18.4 45.03 16.67L45 16.63C49.225 10.105 52.715 6.86 56.86 6.86C65.475 6.86 72.37 19.545 72.37 35.125C72.37 41.065 70.42 44.51 66.395 44.51C62.53 44.51 60.685 41.96 53.345 30.16L48.66 22.335H48.665ZM24.23 8.78C27.855 9.28 31.155 11.95 35.93 18.785C33.1748 23.0039 30.4498 27.2423 27.755 31.5C20.97 42.13 18.625 44.515 14.85 44.515C10.965 44.515 8.65 41.105 8.65 35.015C8.65 22.005 15.14 8.695 22.88 8.695C23.335 8.695 23.785 8.725 24.23 8.785V8.78Z"></path>
        </svg>
      </a>

      <a href="https://github.com/kiwee-tech" target="_blank">
        <span class="sr-only">Github</span>
        <svg viewBox="0 0 80 79" fill="none" class="w-8 h-8 fill-current">
          <path d="M40 0C17.9 0 0 17.9 0 40C0 57.7 11.45 72.65 27.35 77.95C29.35 78.3 30.1 77.1 30.1 76.05C30.1 75.1 30.05 71.95 30.05 68.6C20 70.45 17.4 66.15 16.6 63.9C16.15 62.75 14.2 59.2 12.5 58.25C11.1 57.5 9.1 55.65 12.45 55.6C15.6 55.55 17.85 58.5 18.6 59.7C22.2 65.75 27.95 64.05 30.25 63C30.6 60.4 31.65 58.65 32.8 57.65C23.9 56.65 14.6 53.2 14.6 37.9C14.6 33.55 16.15 29.95 18.7 27.15C18.3 26.15 16.9 22.05 19.1 16.55C19.1 16.55 22.45 15.5 30.1 20.65C33.3 19.75 36.7 19.3 40.1 19.3C43.5 19.3 46.9 19.75 50.1 20.65C57.75 15.45 61.1 16.55 61.1 16.55C63.3 22.05 61.9 26.15 61.5 27.15C64.05 29.95 65.6 33.5 65.6 37.9C65.6 53.25 56.25 56.65 47.35 57.65C48.8 58.9 50.05 61.3 50.05 65.05C50.05 70.4 50 74.7 50 76.05C50 77.1 50.75 78.35 52.75 77.95C60.6911 75.2699 67.5917 70.1667 72.4801 63.3588C77.3685 56.5509 79.9986 48.3812 80 40C80 17.9 62.1 0 40 0Z"></path>
        </svg>
      </a>

      <a href="https://www.linkedin.com/company/kiwee-tech" target="_blank">
        <span class="sr-only">Linkedin</span>
        <svg viewBox="0 0 80 80" fill="none" class="w-8 h-8 fill-current">
          <path d="M0 5.73C0 2.565 2.63 0 5.875 0H74.125C77.37 0 80 2.565 80 5.73V74.27C80 77.435 77.37 80 74.125 80H5.875C2.63 80 0 77.435 0 74.27V5.73ZM24.715 66.97V30.845H12.71V66.97H24.715ZM18.715 25.91C22.9 25.91 25.505 23.14 25.505 19.67C25.43 16.125 22.905 13.43 18.795 13.43C14.685 13.43 12 16.13 12 19.67C12 23.14 14.605 25.91 18.635 25.91H18.715ZM43.255 66.97V46.795C43.255 45.715 43.335 44.635 43.655 43.865C44.52 41.71 46.495 39.475 49.815 39.475C54.16 39.475 55.895 42.785 55.895 47.645V66.97H67.9V46.25C67.9 35.15 61.98 29.99 54.08 29.99C47.71 29.99 44.855 33.49 43.255 35.955V36.08H43.175C43.2016 36.0383 43.2282 35.9966 43.255 35.955V30.845H31.255C31.405 34.235 31.255 66.97 31.255 66.97H43.255Z"></path>
        </svg>
      </a>
    </div>
  </div>

<!--  <nav>-->
<!--    <a href="/">KiWee</a>-->
<!--    <a href="/contact">Contact</a>-->
<!--    <a href="/blog">Blog</a>-->
<!--  </nav>-->

  <div class="text-center pb-12">KiWee &copy; 2022 - 2024. All rights reserved</div>
</footer>

<style>
  html {
    height:100%;
  }

  body {
    margin:0;
  }

  .bg {
    animation:slide 3s ease-in-out infinite alternate;
    background-image: linear-gradient(-60deg, #6c3 50%, #09f 50%);
    bottom:0;
    left:-50%;
    opacity:.5;
    position:fixed;
    right:-50%;
    top:0;
    z-index:-1;
  }

  .bg2 {
    animation-direction:alternate-reverse;
    animation-duration:4s;
  }

  .bg3 {
    animation-duration:5s;
  }

  @keyframes slide {
    0% {
      transform:translateX(-25%);
    }
    100% {
      transform:translateX(25%);
    }
  }
</style>
