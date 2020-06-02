## Road-Map

#### Development/Internal
- [ ] Implement and provide exports for other resources to use, will open doors for potential community contribution for those with experience with FiveM programming.
- [ ] Refactor the current changelog to auto-post to Discord each time version number is changed, saves rewriting every change. Maybe also use `git shortlog`.
- [x] Elaborate on `/extensive-data.json` endpoint - this extends the current /players.json endpoint, providing authorization level and other useful information.
- [ ] Use player identifiers to store in-memory for jailing, this way we can ensure players cannot bypass jailing through leaving the server.
- [x] Introduce a RNG for robbery system.
- [x] Remove radio message for notifying on-duty officers that a player has left the area of a robbery.
- [ ] Focus on providing in-depth purpose for economy.
- [ ] Add more proofing to (a)filming mode.
- [x] Fix some `s_mysql.lua` error.
- [x] Merge `feat/better-globals` branch and ensure no regressions are introduced.

#### User Interface
- [x] Introduce new UI on production.

#### Discord Bot
- [ ] Save sticky data to a JSON file to retain data between restarts.
- [ ] Authorization level setting: Use `/extensive-data.json` endpoint to get the target player's auth level, compare that with auth of target using `hsgRoleMap`, ensure auth of self is higher than target before proceeding.