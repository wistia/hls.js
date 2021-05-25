# Developing Locally 👩‍💻

To change and develop HLS.js locally, the follow steps are required

## In this repository

1. run `yarn link` - https://classic.yarnpkg.com/en/docs/cli/link/
1. run `yarn run build:watch` <- this will start up the HLS.js server and watch for changes

## In player-modern

1. stop your local server if running
1. run `yarn link @wistia/hls.js`
1. start your player-modern server as normal

## When you're finished

https://classic.yarnpkg.com/en/docs/cli/unlink

1. stop your player-modern server and the hls.js server
1. run `yarn unlink @wistia/hls.js` from player-modern
   1. you could also run `yarn unlink` from this repository
1. run `yarn` in player-modern before restarting
   1. if you get compilation errors you may need to run `yarn install --force`
