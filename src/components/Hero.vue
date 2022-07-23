<template>
    <div class="hero  flex flex-col items-center text-center justify-between p-5">
      <img class="w-[10%] transition-all ease-in-out" src="./../assets/stay-at-home.png" alt="" />
      <div class="info">
        <h2 class="font-semibold text-lg">
          Hey, Welcome to The
          <span class="s1"> Code</span><span class="s2">Addict</span>
          <br />
        </h2>
        <p class="text-slate-400">We'll add some art in your Start</p>
        <button class="rounded-lg bg-black py-1 px-3 text-white mt-2">Start Now</button>
      </div>

    </div>

</template>

<script>
export default {
    name:"HeroComponent"
};
</script>

<style lang="scss" scoped>
  // .hero {
  //   display: flex;
  //   flex-direction: row;
  //   justify-content: space-between;
  //   padding: 25px;
  //   max-width: 1440px;
  //   margin-top: 25px;
  //   .info {
  //     display: flex;
  //     flex-direction: column;
  //     h2 {
  //       font-size: 1.2rem;
  //       span {
  //         font-size: 1.2rem;
  //         color: #36454f;
  //       }
  //       .s2 {
  //         font-size: 1.2rem;
  //         color: #f34336;
  //       }
  //     }
  //     button {
  //       border: none;
  //       margin: 10px auto;
  //       padding: 10px 25px;
  //       border-radius: 0.2rem;
  //       font-size: 0.8rem;
  //       background: white;
  //       color: #36454f;
  //       cursor: pointer;
  //       // color: white;
  //       // background-color: #d5adc8;
  //       // background-image: linear-gradient(90deg, #dd93c4 0%, #ff8489 100%);
  //       border: 1px solid #f34336;
  //       &:hover {
  //         transform: scale(0.99);
  //       }
  //     }
  //   }
  //   p {
  //     padding: 10px;
  //     font-size: 1rem;
  //     text-align: center;
  //   }
  //   img {
  //     height: 15rem;
  //     margin-top: -35px;
  //     animation: floating 3s ease-in-out infinite;
  //   }
  //   @keyframes floating {
  //     0% {
  //       transform: translate(0, 0px);
  //     }
  //     50% {
  //       transform: translate(0, 15px);
  //     }
  //     100% {
  //       transform: translate(0, -0px);
  //     }
  //   }
  // }
</style>