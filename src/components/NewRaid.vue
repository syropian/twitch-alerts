<template>
  <div class="widget-AlertBox">
    <div class="widget-container">
      <div class="widget">
        <div class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 52 44"
          >
            <path
              fill="#fff"
              d="M23.744 32.075a13.932 13.932 0 01-6.904 1.82c-2.511 0-4.867-.662-6.904-1.819C4.53 33.725 1.22 39.187 0 44h33.68c-1.22-4.813-4.531-10.277-9.936-11.925zM16.84 6.418c-6.702 0-12.134 5.431-12.134 12.13 0 6.7 5.432 12.13 12.133 12.13 6.702 0 12.134-5.43 12.134-12.13 0-6.699-5.432-12.13-12.134-12.13zm0 21.37c-3.859 0-7.156-2.58-8.48-5.79H25.32c-1.324 3.21-4.621 5.79-8.48 5.79zM33.3 36.666h18.037c-1.22-4.813-4.53-9.36-9.936-11.009a13.93 13.93 0 01-6.904 1.82c-1.699 0-3.326-.305-4.832-.86-.854 1.43-1.94 2.933-3.206 4 3.019 1.162 5.3 3.757 6.841 6.05z"
            />
            <path
              fill="#fff"
              d="M31.46 15.582h11.516c-1.324 3.208-4.621 5.763-8.48 5.763a8.714 8.714 0 01-2.907-.517 14.715 14.715 0 01-.747 2.878c1.153.364 2.38.557 3.655.557 6.7 0 12.133-5.433 12.133-12.132C46.63 5.431 41.198 0 34.497 0 30.2 0 26.427 2.258 24.27 5.625a14.992 14.992 0 017.19 9.957z"
            />
          </svg>
        </div>
        <div class="label">
          <span>Incoming Raid</span>
          <span class="label-section">&mdash; party of {{ amount }}!</span>
        </div>
        <div class="name" id="username-container">{{ name }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: "xX420FazeIt69Xx",
    },
    amount: {
      type: Number,
      default: 1000,
    },
  },
};
</script>

<style scoped>
.widget .icon {
  animation: slideLeft 0.6s cubic-bezier(0.87, 0, 0.13, 1) 1s;
  animation-fill-mode: forwards;
}

.widget .name {
  left: 106px;
}
</style>
