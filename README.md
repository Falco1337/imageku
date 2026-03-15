# Imageku

A simple **Python screenshot snipping tool** similar to the Windows Snipping Tool.  
Press **Print Screen** to capture the screen and select the area you want to save.

The tool allows you to **draw, move, and resize the selection box before saving**.

---

## Features

- Capture screenshot using **Print Screen key**
- **Fullscreen snipping overlay**
- **Drag to select screenshot area**
- **Move and resize selection box**
- **8 resize handles (corners + edges)**
- Save screenshot with **timestamp filename**
- Automatically saved to:

```
~/Pictures/imageku/
```

- Simple **GUI**

---

## Demo

### Select Screenshot Area
![Select Area](images/1.png)

### Resize or Move Selection
![Resize Selection](images/2.png)

---

## How It Works

1. Press **Print Screen**
2. A fullscreen screenshot preview appears
3. **Drag your mouse** to select the capture area
4. Adjust the selection if needed:
   - Drag edges/corners to resize
   - Drag center to move
5. Press **Enter** to save the screenshot
6. Press **Esc** to cancel

---

## Controls

| Key | Action |
|----|------|
| `Print Screen` | Start screen capture |
| `Enter` | Save screenshot |
| `Esc` | Cancel snipping |

---

## Requirements

Install dependencies:

```bash
pip3 install pillow pynput
```
```bash
sudo apt update && apt upgrade -y
```

Python version recommended:

```
Python 3.9+
```

---

## Run

```bash
python3 imageku.py
```
0r

---
### Better performance,

can put at **Session and Startup**

---

The program will run in the background and listen for the **Print Screen** key.

---

## Project Structure

```
project/
│
├─ snip.py
├─ README.md
└─ images/
   ├─ select-area.png
   ├─ resize-selection.png
   └─ saved.png
```

---

## Screenshot Naming

Saved screenshots follow this format:

```
imageku_YYYYMMDD_HHMMSS.png
```

Example:

```
imageku_20260315_142530.png
```

---

## Built With

- **Tkinter** – GUI overlay
- **Pillow (PIL)** – image processing
- **pynput** – keyboard listener
- **ImageGrab** – screen capture

---

## License

MIT License
