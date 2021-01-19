# ChessRoberta

ChessRoberta is a project to get a Kuka iwaa Robot to play chess with a human opponent. 

## Programm Packages
The program consists of two packages. Our robot is called Roberta. The package **ChessRoberta** is the program for the robot. **ChessRobertaClient** is the program running on a PC and sending moves to the robot via Ethernet. 

###ChessRoberta
The robot is providing a server for the communication. This server is receiving the move commands from ChessRobertaClient. The program is checking if the move is legal an possible with Chesspresso, calculating the position of the pieces to move and calculating and commanding the move of the robot. After this it is sending the new position of the pieces back to the client or a message like "game over", "illegal move" ...

###ChessRobertaClient
This program is communicating with the server in ChessRoberta. It is sending the move commands to the robot. The robot player is played by a stockfish engine, integrated in this program. 

## Robotic setup 
We are using a Kuka iwaa 7 R 800 robot with a media-flansh electric IO. Attached to this is a Zimmer R840 IO gripper. For programingwe are using Kuka Sunrise Workbench 1.16. for the ChessRoberta and Eclipse with java for ChessRobertaClient.

## License
The program is licensed under GNU General Public License v3.0. Chesspresso used in ChessRoberta is under the GNU Library or Lesser General Public License version 2.0.

## Questions
For questions, please contact juergen.schwittek (ad) fhws.de
