# 🌍 Map Coloring using CSP (Australia)

## 📌 Overview
This project solves the Map Coloring Problem using Constraint Satisfaction Problem (CSP) techniques in Python. The goal is to assign colors to regions such that no two adjacent regions share the same color.

---

## 🗺️ Problem Description
We consider the map of Australia with the following states:

- WA (Western Australia)
- NT (Northern Territory)
- Queensland
- SA (South Australia)
- NSW (New South Wales)
- V (Victoria)
- T (Tasmania)

Each state must be colored using:
- Red
- Green
- Blue

---

## 🔗 Adjacency Constraints

- WA → NT, SA  
- NT → WA, SA, Queensland  
- SA → WA, NT, Queensland, NSW, V  
- Queensland → NT, SA, NSW  
- NSW → Queensland, SA, V  
- V → SA, NSW  
- T → (no neighbors)

---

## ⚙️ Approach

This solution uses the Backtracking Algorithm:

1. Start with an empty assignment  
2. Select a state  
3. Assign a color  
4. Check if it is valid (no neighbor has the same color)  
5. If valid, continue to the next state  
6. If not, backtrack and try another color  
7. Repeat until all states are assigned  

---

## 🧠 Functions Used

- **is_valid()** → Checks if a color assignment is valid  
- **solve_map_coloring()** → Uses backtracking to find a solution  

---

## ▶️ How to Run

1. Save the code in a file named `map_coloring.py`  
2. Run:

```
python map_coloring.py
```
