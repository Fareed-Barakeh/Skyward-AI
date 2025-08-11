# Skyward-AI
Skyward AI is a two-player strategy game where each player commands airplanes with limited rockets to outmaneuver and destroy the opponent’s fleet. It features a heuristic AI using Minimax, with planned Alpha-Beta pruning and future neuro-symbolic AI integration for deeper, adaptive play.

#Overview
Airplane Tactics is an original, turn-based board game featuring positional movement, directional facing, and ranged attacks. Each player commands a small squadron of aircraft and manages limited rockets to outmaneuver and eliminate the opponent. The last player with at least one airplane on the board wins.
Current AI Work

#Implemented: heuristic AI using the Minimax algorithm.
#In progress: upgrade to Alpha–Beta pruning for deeper search within the same compute budget.
#Planned: neuro-symbolic AI that combines learned evaluation (neural model) with symbolic search (Minimax/Alpha–Beta), enabling stronger heuristics and adaptive strategy.

#Rules (Concise)
Each player starts with 8 airplanes.
Each airplane can carry up to 2 rockets.
Airplanes have facing and can rotate clockwise or counter-clockwise.
You can attack by:
Moving your airplane into an opponent’s airplane (melee), or
Firing a rocket at an opponent’s airplane (ranged).
Win condition: You win if you have one or more airplanes remaining when your opponent has none.

#Controls
Mouse
Left-click empty square: Place a new airplane (newly placed units cannot move until the next turn).
Left-click airplane: Select airplane.
Left-click selected airplane → empty square: Move airplane.
Left-click selected airplane → opponent airplane: Attack (melee).
Middle-click selected airplane: Load one rocket (max 2).
Right-click opponent airplane (with rockets): Fire a rocket (ranged).

#Keyboard
Right Arrow: Rotate clockwise.
Left Arrow: Rotate counter-clockwise.
Space: End turn / Change turn.

#Credits
Game invention: Ammar Hatem
Design & programming: Fareed Barakeh

#Roadmap
Integrate Alpha–Beta pruning with move ordering and transposition tables.
Add neural evaluation head (supervised/self-play) for neuro-symbolic search.
Parameterize heuristics (threats, mobility, facing, ammo, proximity) and expose them for training/tuning.
Optional: opening book and endgame tablebases once rules are finalized.
