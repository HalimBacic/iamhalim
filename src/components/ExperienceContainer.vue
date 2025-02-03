<template>
    <div class="main">
      <div class="container">
        <div class="horizontal-line">
          <!-- Prva linija -->
          <div class="vertical-line top"></div>
          <div class="text top left">
            <strong>Intern Software Developer</strong><br />
            <em>Alea Partners</em><br />
            <span>2021 - 2022</span><br />
            Refactoring of existing applications.<br />
            Gambling games backend API for three company games.<br />
            Database projection for those games.<br />
            AleaMiddleware application for project communication.
          </div>
  
          <!-- Druga linija -->
          <div class="vertical-line bottom"></div>
          <div class="text bottom right">
            <strong>Software Developer</strong><br />
            <em>Alea Partners</em><br />
            <span>2022 - 2024</span><br />
            Application maintenance for production apps.<br />
            Database maintenance and projections.
          </div>
  
          <!-- Treća linija -->
          <div class="vertical-line extra-top"></div>
          <div class="text top right">
            <strong>Software Developer</strong><br />
            <em>Asseco</em><br />
            <span>2024 - now</span><br />
            Server-side Java projects.
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "AboutContainerTimeline",
  };
  </script>
  
  <style scoped>
  .main {
    width: 100vw;
    height: 90vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .container {
    position: relative;
    width: 100%;
    height: 250px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .horizontal-line {
    width: 80%;
    height: 2px;
    background-color: black;
    position: relative;
  }
  
  /* Stil za vertikalne linije */
  .vertical-line {
    width: 2px;
    height: 60px;
    background-color: black;
    position: absolute;
  }
  
  /* Prva vertikalna linija (levo, gore) */
  .vertical-line.top {
    top: -60px;
    left: 20%;
  }
  
  /* Druga vertikalna linija (desno, dole) */
  .vertical-line.bottom {
    bottom: -60px;
    left: 50%;
  }
  
  /* Treća vertikalna linija (desno, gore) */
  .vertical-line.extra-top {
    top: -60px;
    left: 80%;
  }
  
  /* Stil za tekst */
  .text {
    position: absolute;
    font-size: 14px;
    color: black;
    background-color: white;
    padding: 8px 12px;
    border-radius: 5px;
    width: 180px;
    text-align: center;
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
  }
  
  /* Tekst iznad linije (gore) */
  .text.top {
    top: -250px;
  }
  
  /* Tekst ispod linije (dole) */
  .text.bottom {
    bottom: -200px;
  }
  
  /* Pozicioniranje teksta */
  .text.left {
    left: 12%;
  }
  
  .text.right {
    left: 42%;
  }
  
  .text.right:last-of-type {
    left: 72%;
  }
  </style>
  