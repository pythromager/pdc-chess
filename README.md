# Piece Disability Chess (PDC) – Rules

## Core Principle
All standard chess rules apply unless explicitly overridden below. This includes castling, en passant, promotion, stalemate, and insufficient material draws.

* **Default Rule:** No piece may capture, except as specified per piece below.

---

## Piece Rules

### Pawn
* **Movement:** Standard pawn movement applies.
* **Capturing:** May only capture other pawns (standard diagonal capture).
* **The River Exception:** A pawn may also capture an enemy **Knight** if that knight is in **"the river"** (squares **c4, d4, e4, f4, c5, d5, e5, f5**). The pawn must still be diagonally adjacent to the knight to capture it.

### Rook
* **Obligation:** **Must capture** if any capture is available within range.
* **Range:** Capturing range is limited to **3 squares**. The rook cannot capture a piece more than 3 squares away.
* **Movement:** The rook may still move beyond 3 squares if it is not capturing. Any piece within the path blocks further captures as normal.

### Knight
* **Capturing:** Can optionally capture any piece that is currently **giving check** to your king—and **only** those pieces. No other captures are permitted.
* **Defense:** The knight may also block check by moving between the checking piece and the king. Neither of these is forced.

### Bishop
* **Capturing:** The bishop **cannot** capture any piece.
* **Obligation:** If the bishop can legally move to a square that gives check, it **must** do so.
* **Checkmate Clause:** If your bishop must give check but cannot (because your king is in check and the king must move instead), that is checkmate, unless the **M1 Special Rule** applies.
* **Note:** A discovered check created by another piece moving does not trigger the must-check obligation.

### Queen
* **Capturing:** The queen may capture any piece.
* **Obligation:** It **must capture** any non-knight piece it attacks. It has no obligation to capture knights, though it may do so freely.
* **Stacking Musts:** Each non-knight enemy piece the queen attacks is its own separate must-obligation.
* **Checkmate Clause:** If the queen must capture a piece but cannot (because the king is in check), that is checkmate, unless the **M1 Special Rule** applies.

### King
* **While in Check:** The king **must move**. You cannot block or capture the checking piece. This counts as one must-obligation.
* **While Not in Check:** The king moves and captures normally.

---

## Loss Conditions

### Double Must = Loss
If a player has **two or more** simultaneous must-obligations that cannot all be satisfied in a single move, that player loses immediately—unless the **M1 Special Rule** applies.

**Individual obligations count separately:**
* Queen attacking two pawns = **2 musts**
* Queen attacking two pawns + a rook also attacking those same two pawns = **4 musts**
* Being in check = **1 must** (king must move)
* A rook with two capturable enemies within range = **2 musts**

### Standard Checkmate
If a player has no legal moves and is in check, that is checkmate as in standard chess.

---

## Special Rules

### M1 Special Rule
If a player has at least one must-obligation, any piece may **ignore all must-obligations** for that move, provided:
1.  The move is legal in standard chess (does not leave your own king in check).
2.  The move results in **checkmate in 1** for the opponent under PDC rules.

---

## Draw & Win Conditions

### 2-Move Repetition Draw
There is no 3-fold repetition rule. If the same position occurs for the **second time**, a draw may be claimed before the repeated move is played—even if that move is forced.

### 15-Move Space Win
If 15 consecutive moves pass with no captures, the player controlling more space on the opponent's half wins. This replaces the 50-move rule.

**Space Calculation (+1 per square):**
* **Physical:** +1 per piece physically located on the opponent's half.
* **Ghost Capture:** +1 per square on the opponent's half reachable via the piece's PDC capture pattern. 
    * **Pawn:** Two forward diagonal squares (if empty or containing a pawn).
    * **Rook:** Up to 3 squares per direction (blocked by any piece).
    * **Knight:** All 8 jump squares (only if empty or a piece checking your king).
    * **Bishop:** All diagonal squares until the first piece (empty squares only).
    * **Queen:** All 8 directions until the first piece.
    * **King:** Adjacent empty squares only.

---

## Quick Reference

| Piece | Can Capture? | Must? | Notes |
| :--- | :--- | :--- | :--- |
| **Pawn** | Enemy pawns / Knights in "River" | No | En passant vs pawns only. |
| **Rook** | Yes (max 3 squares) | **Yes** | Every capturable enemy = 1 must. |
| **Knight** | Only pieces checking King | No | Can also block check. |
| **Bishop** | No | **Yes** | Must give check if able. |
| **Queen** | Yes (Any) | **Yes** | Must take non-knights. |
| **King** | Only when NOT in check | **Yes** | Must move when in check (1 must). |
