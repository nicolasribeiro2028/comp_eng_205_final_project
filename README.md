# Mario & Hamster Pong: 

## Overview
This project implements a Pong-style arcade game:  
Mario must bounce a moving hamster back toward an opponent hamster.  

The objective is simple:
Be the first to reach 60 points to win the game.

The game introduces dynamic physics, increasing difficulty, and visual feedback to enhance gameplay.

---

## How to play

- Download the assembly file
- Go to https://cpulator.01xz.net/](https://cpulator.01xz.net/?sys=arm-de1soc
- Upload the file and press continue
- Locate the Push buttons in the Devices Section
- Press accordingly

---

## 🎮 Gameplay

- Control Mario’s paddle to hit the ball (hamster)
- Use the controls from the input file native to CPUlator
- The opponent is another hamster with selectable speed
- Each rally increases difficulty and scoring potential
- First player to 60 points wins

---

## 🚀 Features

### Special Visual Effects
- GreenScoreFlash  
  - Triggered when Mario scores  
  - Screen briefly turns green  
  - Displays a happy sprite  

- RedLoseBlink  
  - Triggered when the opponent scores  
  - Screen blinks red 3 times  
  - Displays a sad sprite  

- Both effects are implemented using:
  - ClearVGA for background manipulation

---

### Physics & Game Mechanics
- Ball movement is updated every frame using:
  - ball_dx (horizontal velocity)
  - ball_dy (vertical velocity)

- Dynamic rebounds:
  - Bounce angle depends on where the ball hits the paddle
  - Offset from paddle center determines trajectory

- Collision zones:
  - Different zones produce shallow or steep angles
  - Creates more skill-based and varied gameplay

---

### Advanced Scoring System
- Score gained equals the current ball velocity
- Ball speed increases after each paddle hit

This means:
- Longer rallies = higher speed = more points

---

## Controls

- Select opponent speed: 0, 1, or 3  
- Move Mario paddle: 2  
- Restart game (after game over): 0  

---

## Game Flow

1. Start the game  
2. Choose opponent velocity (0, 1, or 3)  
3. Play using paddle controls  
4. Game ends when a player reaches 60 points  
5. Press 0 to restart  



---

## 📌 Future Improvements

- Add sound effects
- Multiple difficulty levels
- Power-ups (speed boost, paddle size, etc.)
