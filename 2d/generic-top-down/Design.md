## High Level Design
### Premise
Game topdown klasik tentang menjatuhkan zombie. Zombie mengejar player dan player menghindari serangan zombie sambil menembak.
POV Game adalah topdown, dan kamera terkunci ke player saat gameplay.
Style game nya adalah pixelated.

### Map
Gridmap topdown. 64x64. Ada collission. Juga digunakan untuk pathfinding.

### Player
Tidak memiliki animasi. Kamera tepat diatas player. Punya stats (Speed). Bisa bergerak 8 arah menggunakan bind WASD, dan bisa menembak pistol dengan bind Left Mouse Button. Bisa mati

Ketika pistol ditembakan, sebuah object peluru akan spawn dan secara otomatis bergerak ke arah cursor. Pistol memiliki peluru tak terbatas.

### Musuh
Memiliki animasi. punya stats (HP, dan Speed). Musuh menggunakan pathfinding untuk mengejar player diatas map. Jika menabak player, player kena damage dan zombie akan di dorong mundur. Bisa mati
(Atau Ketika dekat dengan player, mereka akan masuk state menyerang)
