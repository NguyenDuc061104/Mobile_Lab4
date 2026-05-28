# Lab4 - Real-Time Mobile Game

Project Android Kotlin for Lab 4. The game uses `SurfaceView` and a custom `GameThread`
to update and draw gameplay at about 60 FPS.

Implemented exercises:

1. Show high score using `SharedPreferences`.
2. Give the player 3 lives before game over.
3. Draw a spaceship at the shooting position and move it to each touch location.
4. Upgrade bullets by score; higher levels fire more spread bullets.
5. Give each enemy random health and draw a health bar.
6. Let enemies move in horizontal lanes while falling.
7. Add a Boss that moves left and right near the top and spawns smaller enemies.

Main source files:

- `GameThread.kt`: main loop.
- `GameView.kt`: Android `SurfaceView` lifecycle and touch input.
- `GameState.kt`: score, high score, lives, speeds, object lists, reset state.
- `GameWorld.kt`: gameplay update, collision, enemy spawning, Boss spawning.
- `GameRenderer.kt`: background, player, HUD, and game-over drawing.
- `BulletFactory.kt`: bullet spread and bullet upgrade levels.
- `GameManager.kt`: creates bitmap sprites and enemies.
- `Opponent.kt`: enemy movement, health, health bar, collision hitbox.
- `FiringObject.kt`: bullets with spread velocity.
- `Boss.kt`: Boss movement, health, and enemy spawning position.
