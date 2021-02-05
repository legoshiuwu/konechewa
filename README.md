# konechewa

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Snake Game</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <header>
      <p>Now: <span id="current-score"></span></p>
      <p>Best: <span id="best-score"></span></p>
    </header>
    <div id="container"></div>
  </body>
  <script src="main.js"></script>
</html>
html {
  height: 100%;
  --text-color: #ecf0f1;
}

* {
  box-sizing: border-box;
  outline: 0;
  margin: 0;
}

body {
  height: 100%;
  background: #2c3e50;
  padding: 60px;
  font-family: sans-serif;
  display: flex;
  flex-direction: column;
}

canvas {
  border: 2px solid var(--text-color);
}

#container {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
}

header {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  color: var(--text-color);
}

p {
  font-size: 3vmin;
  margin: 2%;
}
// #region general utils
// #endregion

// #region geometry
// #endregion

// #region constants
// #endregion

// #region game core
// #endregion

// #region rendering
// #endregion

// #region main
// #endregion
// #region general utils
const getRange = length => [...Array(length).keys()]
const getRandomFrom = array => array[Math.floor(Math.random() * array.length)]
const getWithoutLastElement = array => array.slice(0, array.length - 1)
const getLastElement = array => array[array.length - 1]
const areEqual = (one, another) => Math.abs(one - another) < 0.000000000001
// #endregion
