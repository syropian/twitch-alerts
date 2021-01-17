<template>
  <div class="widget-AlertBox">
    <div class="widget-container">
      <div class="widget">
        <div class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 48 44"
          >
            <path
              fill="#fff"
              d="M45.587 15.23h-15.56L25.3 1.122C25.067.434 24.422 0 23.692 0c-.73 0-1.375.434-1.607 1.121l-4.728 14.11H1.692c-.93 0-1.692.761-1.692 1.692 0 .095.01.201.032.286.02.37.19.782.708 1.195l12.788 9.011L8.62 41.684c-.243.687 0 1.46.582 1.904.307.222.592.412.952.412.349 0 .761-.18 1.057-.38l12.481-8.896 12.481 8.895c.296.212.709.381 1.058.381.36 0 .645-.18.941-.413a1.676 1.676 0 00.582-1.903l-4.908-14.269 12.682-9.096.307-.264c.275-.296.55-.698.55-1.132 0-.93-.868-1.692-1.798-1.692z"
            />
          </svg>
        </div>
        <div class="label">
          <span>Resubscriber</span>
          <span class="label-section">&mdash; {{ amount }} months!</span>
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
      default: 2,
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
</style>
