<!-- Copyright 2025 Ibrahim Ansari -->
<!-- SPDX-License-Identifier: Apache-2.0 -->

<!-- Source: https://cssloaders.github.io/ -->
<!-- Indeterminate only -->
<span class="loader"></span>

<style lang="scss">
  .loader {
    width: 100%;
    height: 4.8px;
    display: inline-block;
    position: relative;
    background: rgba(255, 255, 255, 0.15);
    overflow: hidden;
  }
  .loader::after {
    content: '';
    width: 192px;
    height: 4.8px;
    background: #fff;
    position: absolute;
    top: 0;
    left: 0;
    box-sizing: border-box;
    animation: animloader 2s linear infinite;
  }

  @keyframes animloader {
    0% {
      left: 0;
      transform: translateX(-100%);
    }
    100% {
      left: 100%;
      transform: translateX(0%);
    }
  }
</style>
