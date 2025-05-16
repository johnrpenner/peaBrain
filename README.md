peaBrain 8 ©2024 by John Roland Penner
peaBrain 8 is a Human Created UCI Chess Engine written in Swift for macOS
released: July 15, 2024 • toronto island

peaBrain 8 is the UCI version of the engine used in my commercial Chess Meister 
product for the iPhone. it provides a simple pedagogical chess engine written in 
Swift which should be easily comprehensible to anyone interested in getting 
started with chess programming. It can be played in any UCI compatible 
Chess GUI application like HIARCSor peaBoard for macOS. 

peaBrain uses a classic Shannon type MiniMax search with Quiescence extensions 
and Alpha-Beta pruning, SAN Notation, and is written to support Fischer games 
(coming next release), The opening book includes 10,000 moves from the ECO 
(Encyclopedia of Chess Openings). Runs at about 1400 ELO. Comes complete 
with Swift source code. 

peaBrain is the Slowest Engine out there — but at least i wrote the moveGenerator
on my own without stealing someone else's Bitboard like half the Stockfish clones, 
and absolutely without the use of A.I. (peaBrain 8 is in fact it is the last version of 
peaBrain to be written WITHOUT AI — the next version peaBrain 9 will be the first to do so). 

The entire codebase is a functional port of an earlier chess engine i had written in 2010 
in futureBasic called pChess 2.0 — which is still more advanced in its use of hash tables 
for greater speed, and support for fischer random chess. pChess 2.0 came with a 
graphical interface which allowed sound and graphic visualization of the moves in 
real-time as they were being processed by negamax as part of an iMac art installation. 

a separate project — an extension of Chess Meister for the iPad — will be a new UCI GUI 
app called, correspondingly — peaBoard UCI for macOS, and peaBrain 9 (the next project) 
will be its default engine. 

Usage: compile this puppy with: 
swiftc -o pea8 peaBrain8.swift -Ounchecked -suppress-warnings 

and see if you can beat the peabrain! 🤩 

NOTE: you NEEED to use -Ounchecked for 100x the SPEEED!! 
PERFT on M1 with -Ounchecked = depth 5 nodes 4865609✅ time 3.31 nps 1468141.10
PERFT on M1 without -Ounchecked depth 5 nodes 4865609✅ time 917.09 nps 5305.47

john roland penner
toronto island 🇨🇦 


--| HISTORY peaBrain 1-8 |-----

Development Timeline: 
• 2009 - pChess 1.0 
• 2010 - pChess 2.0; dropFour 
• 2011 - pChess UCI; port to C++ 
• 2012 - pea3.4 C++ commandline; [freeSpace] 
• 2013 - peaBrain 4.3 C++ engine 
• 2014 - Chess Meister 1.0 
• 2015 - NEX4 1.0; [OMM elisa clone] 
• 2016 - Music Invaders 1.0 
• 2016 - peaBrain5 Swift Chess Engine 
• 2017 - Chess Meister II for iPhone 
• 2018 - Hnefatafl 0.9.0 
• 2021 - pea3 C++ commandline > GitHub 
• 2023 pseudoEngine UCI 
• 2024 peaBrain 8 UCI > GitHub


--| THANKS |-----------------------------------------------

• Papa Penner Sr. for Games of Real Chess.
• Robert Purves for Mentoring and Recursion.


--| CONTACT |----------------------------------------------

GitHub https://github.com/johnrpenner
Storms Nest https://johnrolandpenner.com/index-chess.html
Facebook https://www.facebook.com/chesschessmeister
