# Gikohun (gikopoi2 fork)
## ABOUT

This is a fork of gikopoi2 with the following changes currently:
- 5 more themes (lohere, dream, butter, bubblegum, toxic),
- 2 more characters from [gikopoi3](https://github.com/153/gikopoi3),
- Hungarian language enforced on local area (international language can be changed),
- [mana point system](https://visualchat.hu/gikohu-mana-guide.pdf),
- #rula requiring mana,
- dice rolling command (in the following format: #xdy(+-)z where x is the number of dice, y is the mandatory side count, z is the modifier eg. #5d10+5),
- individual results for dice rolling if you use the #xDy+z format (capital letter d),
- experimental #whisper command for all the psychic giko!
- silly HP counter with the original trigger words,
- experimental #shout command/spell,
- #afk command to intentionally set yourself flagged inactive,
- you can read and write postit notes with #write and #read,
- additional languages translated by ChatGPT,
- random chance to spawn between two maps when entering,
- XP counter to count your steps,
- optional ambient sounds in seashore, hilltop, convenience store and train

See the live instance at https://gikopoi.hu

I'm trying my best to keep up with any development happening on gikopoi2 and update accordingly. 

**Important:** At the moment some things are hardcoded to work with our local settings, so in general I don't recommend to use this repository for your custom instance for the time being.

## INSTALL

to start server, run:

``$ yarn``
``$ yarn build``
``$ yarn start``

for local debugging:
``$ yarn dev``

to enable automatic version bump run:

``$ git config core.hooksPath .githooks``

With setting up janus for streams see the [docs](https://github.com/ieksobeh/gikopoihun/tree/master/docs) folder and [this document](https://janus.conf.meetecho.com/docs/auth.html) about auth options

## MISC SERVER STUFF

Generate a message log

``$ cat nohup.out | grep "MSG:" > msglog.txt``

Start up giko on ssh as background process

``$ nohup yarn start &``

Start up janus on ssh as background process

``$ /opt/janus/bin/janus -a changeme &``

## EXPERIMENTAL-POIPOI

My instance has been added to the [experimental-poipoi](https://github.com/iwamizawa-software/experimental-poipoi) addition, there are no extra steps for you to take.
