<template>
  <div class="widget-AlertBox">
    <div class="widget-container">
      <div class="widget">
        <div class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 49 43"
          >
            <path
              fill="#fff"
              fill-rule="evenodd"
              d="M29.572 7.74h16.723c1.218 0 2.205.985 2.205 2.2v28.6c0 1.215-.987 2.2-2.205 2.2h-2.204c0 1.215-.987 2.2-2.205 2.2h-4.409a2.202 2.202 0 01-2.204-2.2H13.227c0 1.215-.987 2.2-2.204 2.2h-4.41a2.202 2.202 0 01-2.204-2.2H2.205A2.202 2.202 0 010 38.54V9.94c0-1.215.987-2.2 2.205-2.2h18.003L15.211 4c-2.351-1.76.294-5.28 2.646-3.52l7.288 5.455 3.058-3.051C30.28.81 33.398 3.921 31.32 5.995L29.572 7.74zm14.519 8.8a2.202 2.202 0 002.204-2.2c0-1.215-.987-2.2-2.204-2.2a2.202 2.202 0 00-2.205 2.2c0 1.215.987 2.2 2.205 2.2zM8.705 13.51c-1.54.38-2.779 1.635-3.246 3.29-.7 2.48-1.05 4.96-1.05 7.439 0 2.48.35 4.959 1.05 7.438.467 1.655 1.705 2.91 3.246 3.29 3.712.914 8.527 1.372 13.34 1.372 4.814 0 9.629-.458 13.341-1.372 1.54-.38 2.779-1.635 3.246-3.29.7-2.48 1.05-4.959 1.05-7.438 0-2.48-.35-4.96-1.05-7.438-.467-1.656-1.705-2.911-3.246-3.29-3.712-.915-8.141-1.372-13.34-1.372-5.2 0-9.63.457-13.341 1.371z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <div class="label">
          <span>New Host</span>
          <span class="label-section">&mdash; {{ amount }} viewers!</span>
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
      default: 600,
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
  left: 103px;
}
</style>
