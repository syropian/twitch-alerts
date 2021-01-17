<template>
  <div class="widget-AlertBox">
    <div class="widget-container">
      <div class="widget">
        <div class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 44 44"
          >
            <path
              fill="#fff"
              d="M22 44C9.85 44 0 34.15 0 22S9.85 0 22 0s22 9.85 22 22-9.85 22-22 22zm-7.7-17.6v4.4h5.5v4.4h4.4v-4.4h2.2a5.5 5.5 0 100-11h-8.8a1.1 1.1 0 010-2.2h12.1v-4.4h-5.5V8.8h-4.4v4.4h-2.2a5.5 5.5 0 100 11h8.8a1.1 1.1 0 010 2.2H14.3z"
            />
          </svg>
        </div>
        <div class="label">
          <span>New Tip</span>
          <span class="label-section">&mdash; {{ currency }}{{ amount }}!</span>
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
    currency: {
      type: String,
      default: "$",
    },
    amount: {
      type: Number,
      default: 10,
    },
  },
};
</script>

<style scoped>
.widget .icon {
  animation: slideLeft 0.6s cubic-bezier(0.87, 0, 0.13, 1) 1s;
  animation-fill-mode: forwards;
}

.widget svg {
  animation: spin 0.6s cubic-bezier(0.87, 0, 0.13, 1) 1s;
}

.widget .name {
  left: 95px;
}
</style>
