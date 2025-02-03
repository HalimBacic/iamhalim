<template>
    <div class="main">
      <div class="container">
        <div class="horizontal-line">
          <!-- Prva linija -->
          <div class="vertical-line top"></div>
          <div class="text top left">
            <strong>2010 - 2014</strong><br />
            <em>Gimnasium Gradiska</em>
          </div>
  
          <!-- Druga linija -->
          <div class="vertical-line bottom"></div>
          <div class="text bottom right">
            <strong>2014 - 2021</strong><br />
            <em>Faculty of Electroengineering Banja Luka</em>
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
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .container {
    position: relative;
    width: 80%;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .horizontal-line {
    width: 100%;
    height: 2px;
    background-color: black;
    position: relative;
  }
  
  /* Stil za vertikalne linije */
  .vertical-line {
    width: 2px;
    background-color: black;
    position: absolute;
  }
  
  /* Prva vertikalna linija (levo, gore) */
  .vertical-line.top {
    top: -40px;
    left: 25%;
    height: 40px; /* Postavljeno da ne prelazi horizontalnu liniju */
  }
  
  /* Druga vertikalna linija (desno, dole) */
  .vertical-line.bottom {
    bottom: -40px;
    left: 75%;
    height: 40px; /* Postavljeno da ne prelazi horizontalnu liniju */
  }
  
  /* Stil za tekst */
  .text {
    position: absolute;
    font-size: 16px;
    color: black;
    background-color: white;
    padding: 8px 12px;
    border-radius: 5px;
    width: 200px;
    text-align: center;
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
  }
  
  /* Tekst iznad linije (gore) */
  .text.top {
    top: -100px;
  }
  
  /* Tekst ispod linije (dole) */
  .text.bottom {
    bottom: -150px;
  }
  
  /* Pozicioniranje teksta */
  .text.left {
    left: 15%;
  }
  
  .text.right {
    left: 65%;
  }
  </style>
  