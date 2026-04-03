# Algorithm Visualizer

An interactive sorting and pathfinding algorithm visualizer built with pure HTML, CSS, and JavaScript. No build step required -- just open `index.html` in a browser.

![Sorting and Pathfinding](https://img.shields.io/badge/Algorithms-Visualized-6c63ff)
![HTML CSS JS](https://img.shields.io/badge/Stack-HTML%20%7C%20CSS%20%7C%20JS-f7dc6f)
![No Build Step](https://img.shields.io/badge/Build-None%20Required-2ecc71)

---

## Features

### Sorting Visualizer
- **Bubble Sort** -- O(n^2) simple comparison-based sort
- **Selection Sort** -- O(n^2) in-place comparison sort
- **Insertion Sort** -- O(n^2) adaptive sort, efficient for small/nearly-sorted data
- **Merge Sort** -- O(n log n) stable divide-and-conquer sort
- **Quick Sort** -- O(n log n) average, in-place partition-based sort

Visual feedback:
- **Cyan gradient bars** -- unsorted elements (color shifts by value)
- **Yellow** -- elements being compared
- **Pink** -- elements being swapped
- **Green** -- sorted elements (sweep animation on completion)
- **Purple** -- pivot element (Quick Sort)

Live counters track comparisons and array accesses.

### Pathfinding Visualizer
- **A\* Search** -- optimal pathfinding using Manhattan distance heuristic
- **Dijkstra's Algorithm** -- guaranteed shortest path, explores uniformly

Grid features:
- 25 x 45 interactive grid
- Click and drag to draw or erase walls
- Drag the green (start) and red (end) nodes to reposition them
- Random maze generation
- Clear path (keep walls) or clear entire board

Visual feedback:
- **Light blue** -- visited/explored nodes (animated pop-in)
- **Yellow** -- final shortest path (animated glow)

### Controls
- Adjustable **array size** (10--150) and **animation speed** sliders
- **Stop** button to halt any running algorithm
- **New Array** / **Clear Board** / **Random Maze** buttons

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/<your-username>/algorithm-visualizer.git
cd algorithm-visualizer

# Open in your browser (no server needed)
# Windows:
start index.html
# macOS:
open index.html
# Linux:
xdg-open index.html
```

No dependencies. No build step. No `npm install`.

---

## Project Structure

```
algorithm-visualizer/
├── index.html    # Single self-contained app (HTML + CSS + JS)
├── .gitignore
└── README.md
```

Everything lives in one file for maximum portability. Just copy `index.html` anywhere and open it.

---

## Algorithm Complexity Reference

| Algorithm      | Best Case   | Average Case   | Worst Case     | Space    |
|----------------|-------------|----------------|----------------|----------|
| Bubble Sort    | O(n)        | O(n^2)         | O(n^2)         | O(1)     |
| Selection Sort | O(n^2)      | O(n^2)         | O(n^2)         | O(1)     |
| Insertion Sort | O(n)        | O(n^2)         | O(n^2)         | O(1)     |
| Merge Sort     | O(n log n)  | O(n log n)     | O(n log n)     | O(n)     |
| Quick Sort     | O(n log n)  | O(n log n)     | O(n^2)         | O(log n) |
| A* Search      | --          | O(E)           | O(E)           | O(V)     |
| Dijkstra       | --          | O(E + V log V) | O(E + V log V) | O(V)     |

---

## Technologies

- **HTML5** -- semantic markup
- **CSS3** -- custom properties, keyframe animations, grid layout, transitions
- **Vanilla JavaScript** -- ES6+ async/await for animation control, min-heap priority queue

---

## Browser Support

Works in all modern browsers: Chrome, Firefox, Edge, Safari.

---

## License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).
