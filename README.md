# MiniMax Alpha-Beta Algorithm


Develop the Gomoku AI by MiniMax Alpha-Beta Algorithm.



```
Minimax Alpha-Beta :

function alphabeta(node, depth, α, β, maximizingPlayer)
     if depth = 0 or the terminal node
         return the score calculated from the board

     if maximizingPlayer
         for child of the all child node
             α := max(α, alphabeta(child, depth - 1, α, β, FALSE))
             if β ≤ α
                 break (* β cut-off *)
         return α

     else
         for  child of the all child node
             β := min(β, alphabeta(child, depth - 1, α, β, TRUE))
             if β ≤ α
                 break (* α cut-off *)
         return β
```