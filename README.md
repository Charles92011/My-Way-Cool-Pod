# My-Way-Cool-Pod
A bare-minimum Adobe Connect Pod


It seems like every example of a Pod extension for Adobe Connect uses obfuscated javascript (includingthe examples for learning on the Adobe site), and/or include a flash component for compatibility with pre-html5 versions of Connect.

This example contains the smallest amount of code, all of which is in line with the HTML file, to make understanding it easier.

Simply zip up the contents of this repo and drop the zip file in a share Pod in Connect and it will work.


Custom Pods depend on the library connect_customPodSDK.js, which for some reason Adobe has obfuscated. Considering how little documentation they provide, your only hope is to read the library.
I have extracted some necessary code and I'll document as much as I can here:

==Call Backs==
 init 
 config
 update
 caughtUp
 playStateChanged
 podStateChanged
 podClosed
 podTitleChanged
 pointerToggle
 whiteBoardToggle
 roleChanged
 sizeChanged
 syncMessageReceived
 syncModeChanged
 userDetailsChanged
 userJoined
 userLeft
 userStatusChanged

== Functions ==

 init =>  function (e, t, n) 
 communicateToParent =>  function (e, t) // initiates callback
 processCallback =>  function (e, t) // initiates callback
 invoke =>  function (e, t)
 getConfig =>  function ()
 config =>  function () // initiates callback
 findIndexInUserList =>  function (e)
 getUserDetails =>  function (e) 
 getMeetingInfo =>  function () 
 getPodInfo =>  function () 
 getMyUserDetails =>  function () 
 getUserList =>  function () 
 isBreakOutSessionOn =>  function () 
 isWhiteBoardOn =>  function () 
 maximize =>  function (e)  // initiates callback
 setMenuBarControlsVisibility =>  function (e)  // initiates callback
 setPodControlsVisibility =>  function (e)  // initiates callback
 setMyStatus =>  function (e)  // initiates callback
 getBreakoutRoomDetails =>  function (e) 
 getBreakoutRoomsList =>  function () 
 getMyBreakoutRoomDetails =>  function () 
 allowParticipantPublish =>  function (e, t)  // initiates callback
 update =>  function (e)  // initiates callback
 caughtUp =>  function ()  // initiates callback
 userJoined =>  function (e)  // initiates callback
 userLeft =>  function (e)  // initiates callback
 userStatusChanged =>  function (e)  // initiates callback
 syncMessageReceived =>  function (e)  // initiates callback
 syncModeChanged =>  function (e)  // initiates callback
 userDetailsChanged =>  function (e)  // initiates callback
 sizeChanged =>  function (e)  // initiates callback
 podClosed =>  function (e)  // initiates callback
 podTitleChanged =>  function (e)  // initiates callback
 pointerToggle =>  function (e)  // initiates callback
 whiteBoardToggle =>  function (e)  // initiates callback
 roleChanged =>  function (e)  // initiates callback
 playStateChanged =>  function (e)  // initiates callback
 info =>  function (e) 
 dispatch =>  function (e, t, n)  // initiates callback
 dispatchSyncMessage =>  function (e, t, n, i) 
 podVisible => set: function (e)  // initiates callback
 podHeight => get: function () 
 podWidth => get: function () 
 podMinWidth => get: function () 
 podMinHeight => get: function () 
 podID => get: function () 
 isSynced => get: function () 
 connectVersion => get: function () 
 archiveDuration => get: function () 
 playState => get: function () 
 k_HOST => get: function () 
 k_PARTICIPANT => get: function () 
 k_PRESENTER => get: function () 
 language => get: function () 
 AGREE => get: function () 
 AGREE_DISAGREE_CLEAR => get: function () 
 APPLAUSE => get: function () 
 BUILD_NO => get: function () 
 CLEAR_STATUS => get: function () 
 DATE => get: function () 
 DISAGREE => get: function () 
 LAUGHTER => get: function () 
 LOWER_HAND => get: function () 
 RAISE_HAND => get: function () 
 SLOW_DOWN => get: function () 
 SPEAK_LOUDER => get: function () 
 SPEAK_SOFTER => get: function () 
 SPEED_UP => get: function () 
 STEP_AWAY => get: function () 
 STEP_IN => get: function () 
 VERSION => get: function () 
