<template>
  <div class="widget-AlertBox">
    <div class="widget-container">
      <div class="widget">
        <div class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 47 44"
          >
            <path
              fill="#fff"
              d="M13.16 0h.11c4.367 0 8.228 2.31 10.45 5.72C25.942 2.31 29.803 0 34.17 0h.11C41.089.066 46.6 5.599 46.6 12.43c0 4.07-1.782 9.845-5.258 14.597C34.72 36.08 23.72 44 23.72 44s-11-7.92-17.622-16.973C2.622 22.275.84 16.5.84 12.43.84 5.599 6.351.066 13.16 0z"
            />
          </svg>
        </div>
        <div class="label">
          <span>New Follower</span>
          <span class="label-section">&mdash; Thank you!</span>
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
  },
};
</script>

<style scoped>
.widget .icon {
  animation: slideLeft 0.6s cubic-bezier(0.87, 0, 0.13, 1) 1s,
    heartbeat 1.4s linear 3.7s infinite;
  animation-fill-mode: forwards;
}
</style>
