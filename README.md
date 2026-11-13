# Catadoption
Create a game that catches cats with treats so they can be adopted.  The game has to have Cabrillo College in the title page.  Call the game Pounce Patrol
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="theme-color" content="#10182b" />
    <title>Pounce Patrol | Cabrillo College</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <main class="game-shell">
      <header class="hud">
        <div>
          <p class="eyebrow">Cabrillo College</p>
          <h1>Pounce Patrol</h1>
        </div>

        <div class="stats" aria-label="Game statistics">
          <div class="stat">
            <span>Treats given</span>
            <strong id="treatsGiven">0</strong>
          </div>
          <div class="stat">
            <span>Cats caught</span>
            <strong id="catsCaught">0</strong>
          </div>
          <div class="stat">
            <span>Cats adopted</span>
            <strong id="catsAdopted">0</strong>
          </div>
          <div class="stat">
            <span>Time</span>
            <strong id="time">60</strong>
          </div>
        </div>
      </header>

      <p class="instructions">
        Click or tap near a cat to toss it a treat. A treated cat is caught and
        taken to the adoption center!
      </p>

      <canvas
        id="gameCanvas"
        width="960"
        height="540"
        aria-label="Pounce Patrol game area"
      ></canvas>

      <div id="overlay" class="overlay visible">
        <section
          class="panel"
          role="dialog"
          aria-labelledby="panelTitle"
          aria-describedby="panelDescription"
        >
          <p class="eyebrow">Cabrillo College Cat Rescue</p>
          <h2 id="panelTitle">Pounce Patrol</h2>
          <p id="panelDescription">
            Give treats to wandering cats, catch them, and help them find loving
            homes at the adoption center.
          </p>
          <button id="startButton" type="button">Start Game</button>
        </section>
      </div>
    </main>

    <script src="script.js"></script>
  </body>
</html>
