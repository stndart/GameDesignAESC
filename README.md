# GameDesignAESC

Interactive streaming control points io-like game

Using:
Unreal Engine 4 (C++)
mixer.com
interactive unreal mixer plugin (github.com/mixer/interactive-unreal-plugin)

Map consists of two cores and points in the middle.
The game is played by AI vs. players
Each player controls a unit (warrior / archer) and orders him where to go.
Each unit battles automatically, with constant distance-relative priority target.
After death, unit is shortly respawned in the core and continues the last order.

For controlling a point team receives win points. When point is contested, it does not give any points.
The more units are contesting a point, the faster it is contested.
If there are both sides units near the point, it is contested with speed, depening on difference of each team units number.
Core is also contestable.
Victory for contesting the core / points domination.

AI learns from scratch. Further - stronger.
AI places each unit for each opposite side unit.
Learning balance is needed to be corrected based on game statistics.
