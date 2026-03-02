# a log

## 2026-02-22

i set op so the client can and will create a reconnect.bin file when it connect to the
server at get a ACK_CONNECTION back from the server with the user's uuid
when the client start is gona try to read 36 charter from the reconnect.bin file
if i does it sends a reconnect requst to the server

the server at the moment just prints the uuid it gets from a reconnect attemp the plan is 
it gona try to find a player with the matching uuid maby make the client as no reponse for securty
then it need to replace the current pollfd with the new one from the reconnect

## 2026-02-25
made it so a client can reconnect to the game server and get it old player back 
need to make it so if a client try to reconnect but they fail to do so and a game is not start they connect insted of a crash
maby save they old name and use that so they don't have to type it in a again we can store it with the reconnect id maby a line for name and 
one for uuid

## 2026-03-02
i the server at the moment is blocking on recv i want to change that so if i ever make this to a game server that can host multiple games at once with out thread it does not block all games.
i fixed client did not get a id, need to refater my net.c or make multiple files is gona get to big
