# timer--app
Timer mit Geldzähler
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Timer mit Geldzähler</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: white;
    color: black;
    margin: 0;
    padding: 0 1em 4em 1em;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
  body.dark {
    background-color: #121212;
    color: white;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1em 0;
  }
  button {
    cursor: pointer;
    font-size: 1.2em;
    background: none;
    border: none;
    color: inherit;
  }
  .timer-container {
    margin-top: 1em;
    display: flex;
    flex-wrap: wrap;
    gap: 1em;
  }
  .timer {
    border: 2px solid #ccc;
    border-radius: 6px;
    padding: 1em;
    flex: 1 1 30%;
    min-width: 250px;
    background: #f9f9f9;
  }
  body.dark .timer {
    background: #222;
    border-color: #555;
  }
  .time {
    font-size: 2em;
    color: black;
  }
  body.dark .time {
    color: white;
  }
  .money {
    font-size: 1.5em;
    color: green;
    margin-bottom: 0.5em;
  }
  .controls {
    margin-top: 0.5em;
  }
  .controls button {
    margin-right: 0.5em;
    font-size: 1em;
    padding: 0.3em 0.8em;
    border: 1px solid #888;
    border-radius: 4px;
  }
  body.dark .controls button {
    border-color: #bbb;
  }
  /* Menü */
  .menu-button {
    font-size: 1.5em;
  }
  .menu-content {
    display: none;
    position: absolute;
    top: 3.5em;
    right: 1em;
    background: white;
    border: 1px solid #ccc;
    border-radius: 6px;
    padding: 1em;
    width: 250px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
    z-index: 100;
  }
  body.dark .menu-content {
    background: #222;
    border-color: #555;
