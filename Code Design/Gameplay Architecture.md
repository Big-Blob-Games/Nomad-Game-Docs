
**Philosophy**

1.) Systems should use composition as much as possible for interchangeable parts. 
2.) Be data driven so we can later extract information from each of the components as work through them. 
3.) Decoupled Systems - Lets create a signal bus which will be used for communication between systems. 
4.) State machines for the main enemies, players, game flow etc. 
5.) Always include fail safes, null checks, clear error messaging etc. 
6.) Single responsibility. Each system will do one thing really well.

--------------------------------------------------------------------------

![[Game Layer Bible]]
Game Layer Logic (How we should communicate.)

## Signals as communication haven

![[SignalBus Idea]]

## Simple Game Architecture 


Game World (Node3D)

- Environment
	- Actual Scene Data
	- Lighting
	- Geometry / places to stay
	- NavMeshRegion
- Entitles (Players, enemies, NPCS)
- Systems
	-Save Manager
	-Combat Manager
	-AnythingElse
- Camera
	-Isometric Camera
	-Cinema Camera
- UI

Save data saved in a godot resource and then populated throughout each of the saves in data.

Using Dialogic V2 to setup the data correctly for the dialogue. Create custom save logic for the player and data. Think about this more carefully later on how to do so. 