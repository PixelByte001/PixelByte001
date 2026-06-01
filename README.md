<style>
:root {
  --custom-gradient-color-1: #9e6bff;
  --custom-gradient-color-2: #9fc1ff;
  --custom-gradient-color-3: #9e6bff;/*
  --custom-gradient-color-1: #a9c9ff;
  --custom-gradient-color-2: #ffbbec;
  --custom-gradient-color-3: #ffc3a0;*/
}

/* Page styling */

/* Base username */
.username {
  position: relative;
  font-size: 2rem;
  font-weight: 500;
  display: inline-block;
}

/* Gradient text */
.usernameGradient {
  background: linear-gradient(
    -30deg,
    var(--custom-gradient-color-1),
    var(--custom-gradient-color-2),
    var(--custom-gradient-color-3)/*,
    var(--custom-gradient-color-1)*/
  );
  background-size: 100px auto;

  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;

  animation: gradientUsernameAnimation 1.5s linear infinite;
}

/* Glow container */
.glowWrapper {
  position: relative;
  z-index: 0;
}

/* Glow layer */
.glowWrapper::after {
  content: attr(data-text);
  position: absolute;
  inset: 0;

  background: inherit;
  background-clip: text;
  -webkit-background-clip: text;

  -webkit-text-fill-color: transparent;

  filter: blur(6px);
  opacity: 0.7;
  z-index: -1;
}

/* Animation */
@keyframes gradientUsernameAnimation {
  0% {
    background-position: 0;
  }
  100% {
    background-position: 100px;
  }
}
</style>

<div class="username glowWrapper usernameGradient" data-text="Data Science">
  Data Science
</div>

![snake gif](https://github.com/PixelByte001/PixelByte001/blob/output/github-contribution-grid-snake.svg)

<!--
**PIxelByte001/PixelByte001** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
