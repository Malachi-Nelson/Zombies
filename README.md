# Fliegerhorst 935

A WW2 round-based zombies prototype that runs in the browser, with online co-op.

**Play:** https://malachi-nelson.github.io/Zombies/

## Co-op

1. Everyone opens the page. The line under the lobby buttons should turn green and say "Online · public room".
2. Type a callsign. One player clicks **Open lobby**; everyone else clicks **Join lobby**, then **Ready up**.
3. The lobby leader clicks **Start match**.

Everyone on the plain link shares one public room. **Make a private room** gives you a link with a code for just your group.

Each player's browser posts its state to a free public MQTT relay, which passes it to the others in the room. There is no game server and nothing connects browser to browser.

`mqtt.min.js` is MQTT.js 4.3.7 (MIT licence).

Needs a keyboard and mouse.
