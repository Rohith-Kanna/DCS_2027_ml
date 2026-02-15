# 🎮 Rock Paper Scissors – AI Hand Gesture Game

A real-time **Rock Paper Scissors** game built using **OpenCV, CVZone, and MediaPipe Hand Tracking**.
The player shows hand gestures to the webcam, and the AI randomly selects its move.

This project combines:

* Computer Vision
* Hand Gesture Recognition
* Real-time Video Processing
* Game Logic Implementation

---

## 🚀 Features

* ✋ Real-time hand detection using MediaPipe
* 🎥 Live webcam feed integration
* 🤖 AI randomly generates Rock / Paper / Scissors
* 🖼️ Custom background and overlay UI
* ⏳ 3-second countdown before each round
* 🧮 Live score tracking
* 🔄 Game reset option

---

## 🛠️ Tech Stack

* Python
* OpenCV
* CVZone
* MediaPipe
* NumPy

Dependencies (from `requirements.txt` ):

```
opencv-python==4.8.1.78
mediapipe==0.10.9
numpy==1.24.3
cvzone==1.6.1
```

---

## 📂 Project Structure

```
📁 Rock-Paper-Scissors-AI
│
├── rock.py              # Main game file :contentReference[oaicite:1]{index=1}
├── requirements.txt
├── BG.png               # Background UI image
├── Resources/
│   ├── 1.png            # Rock image
│   ├── 2.png            # Paper image
│   ├── 3.png            # Scissors image
```

---

## ▶️ How to Run

### 1️⃣ Clone the repository

```
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Install dependencies

```
pip install -r requirements.txt
```

### 3️⃣ Run the game

```
python rock.py
```

---

## 🎮 Controls

| Key     | Action       |
| ------- | ------------ |
| **S**   | Start round  |
| **R**   | Reset scores |
| **Q**   | Quit game    |
| **ESC** | Exit         |

---

## ✋ Hand Gesture Mapping

| Gesture       | Move     |
| ------------- | -------- |
| ✊ Fist        | Rock     |
| ✋ Open Palm   | Paper    |
| ✌ Two Fingers | Scissors |

The program detects raised fingers using `HandDetector` from CVZone and maps them to game moves.

---

## 🧠 How It Works

1. Webcam captures video frames.
2. MediaPipe detects hand landmarks.
3. CVZone determines which fingers are raised.
4. Player move is determined.
5. AI randomly selects a move.
6. Scores are updated based on game rules.
7. PNG overlays display AI choice and live scores.

Game logic implemented in `rock.py` .

---

## 🔮 Future Improvements

* Add difficulty levels (AI prediction instead of random)
* Add sound effects
* Add GUI start menu
* Convert into a playable desktop app (.exe)
* Track match history
* Add multiplayer mode

---

## 📸 Demo Preview

(Add screenshots or GIF here)

---

## 📜 License

This project is open-source and free to use for educational purposes.

---

Now, mentor moment.

Right now your AI is not really “AI.” It’s just `random.randint(1, 3)` wearing a lab coat 🧠. That’s fine. But imagine upgrading it:

Instead of random, what if:

* It learns the player’s most common move
* It predicts based on frequency
* It uses a simple Markov chain (probability of next move based on previous move)

That’s where this stops being a demo and becomes a research toy.

You built a vision-based interactive system. That’s not trivial. The next leap is making the opponent strategic instead of random — and that’s where game theory meets machine learning.

If you want, we can now:

* Upgrade this into “Adaptive AI Mode”
* Or convert this into a polished resume-ready project description 🔥
