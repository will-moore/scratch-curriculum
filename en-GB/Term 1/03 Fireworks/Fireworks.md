﻿Level 1

#Fireworks

__Introduction:__



2. Replace the background with outdoor/city-with-water
3. Use the __new sprite from file__ button to add a Rocket sprite
4. Make the rocket hide when the green



```scratch



	when space key pressed
	show
	glide 1 secs to x: mouse x y: mouse y
```
###Test Your Project






	when space key pressed
	go to x: mouse x y: -200
	show
	glide 1 secs to x: mouse x y: mouse y
```
Does the rocket fly towards the mouse from the bottom of the screen? What happens if you move the mouse and press space again?

7. Finally, lets make this work by using the mouse button instead of the space bar. To do this, we can wrap our script in a __forever if mouse down__.
Then swap the __when space key pressed__ control block for __when flag clicked__ and last but not least make


		go to x: mouse x y: -200
		show
		glide 1 secs to x: mouse x y: mouse y
	(end forever)
```
###Test Your Project



￼1. The first step to make the rocket explode is to make it play a bang sound Resources\bang before it starts moving, and then hide itself once it reaches the mouse. To import a sound go

```scratch

		go to x: mouse x y: -200
		play sound bang
		show
		glide 1 secs to x: mouse x y: mouse y
		hide
	(end forever)
```


		go to x: mouse x y: -200
		play sound bang
		show
		glide 1 secs to x: mouse x y: mouse y
		hide
		broadcast explode
	(end forever)
```
###Test Your Project
Make sure the rocket plays a noise and hides when it reaches the mouse.

3. Import a new sprite using Resources/firework1.png
4. When it receives the explode message, it should hide itself and then move to the position of the rocket using the go to block, show itself, and then vanish again a second later.

```scratch






###Test Your Project
Does it get replaced with the explosion graphic when it explodes?











###Test Your Project










	
	repeat 50
		change size by 2
	(end repeat)

###Test Your Project

Does the explosion graphic spread out from the centre of the rocket and slowly grow?

###Things to try


Remember earlier we had a bug involving holding down the mouse button?



		go to x: mouse x y: -200
		play sound bang
		show
		glide 1 secs to x: mouse x y: mouse y
		hide
		broadcast explode and wait
	(end forever)
```
