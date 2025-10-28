Tags:

 - Button
 - DeadlyThing
 - BlueButton
 - Teleport
 - Coin
 - Gat
 - PPS
 - Combo
 - BackSpeed
 - SlowDown
 - GenPoint
 - HEAL
 - YellowButton
 - PinkButton
 - MagicStar
 - Secret
 - GoinUp
 - MenuMoney
 - SmileCollectable
 - Throwable
 - ButtonThings
 - Costumer
 - ItemCollect
 - DoorS
 - XPcollect
 - PauseMenuTag
 - EnemySee
 - OneEnterBlock
 - Death
 - DeathLower25
 - DeathLower50
 - 2Sped
 - Win
 - Back2Sped
 - 3Sped
 - 1Sped
 - 4Sped
 - AnyAllowed
 - GhostPlayer
 - FinishRed
 - Item
 - RightHand
 - Boss
 - SpeedUp
 - Batut
 - Sword
 - Food
 - Lock
 - CD
 - Enemy
 - Canvasus
 - ButtonAlt
 - FinishAlt
Layers:
 - Default - BuiltIn. Used in GroundLayer as default.
 - TransparentFX - BuiltIn. no clue.
 - Ignore Raycast - BuiltIn. Name says for itself.
 - Water - BuiltIn. ???
 - UI - BuiltIn. UI.
 - pp - You can't jump with it. Used in game in Light Blue square objects.
 - Slide - if touched, player slides.
 - Minigame - ???
 - MinigamePP - ???
 - OnlyMainCam - ???

^PB^ - public

^PR^ - private

PlayerMovement.cs:

	 ^PB^ |float| moveSpeed - Player's Speed (unless set before scene runs, replace with static variable CheatsHandler.CheatsSpeed)
 
	 ^PB^ |float| jumpForce - Player's Jump Height (unless set before scene runs, replace with static variable CheatsHandler.CheatsJumpForce)
 
	 ^PR^ |Rigidbody2D| rb - Rigidbody2D.
 
  	 ^PR^ |float| moveInput - Left & Right movement variable.
 
	 ^PB^ |bool| isGrounded - if Player's on the ground, true, if not, false.
 
	 ^PR^ |bool| isWalledLeft - if Player's touching left wall, true, if not, false.
 
	 ^PR^ |bool| isWalledRight - if Player's touching right wall, true, if not, false. 
 
	 ^PR^ |bool| isCeilied - if Player's close (like really close) to the ceiling, true, if not, false.
 
	 ^PB^ |Transform| groundCheck - object that checks the ground (it's important for isGrounded variable).
 
	 ^PB^ |LayerMask| groundLayer - on which layers can Player jump.
 
	 ^PB^
 
	 ^PB^
 
	 ^PB^
 
