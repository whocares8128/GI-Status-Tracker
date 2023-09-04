# GI-Status-Tracker
3dmigoto config that defines global variables which track various player states.

This config was created to provide outside support for tracking various conditions in Genshin Impact, including:
	$underwater	Player is underwater (only possible in Fontaine)
	$swimming	Player is swimming (either on the surface or underwater)
	$wet		Player is Wet (generally, on the surface this relies on detection of water drips and any status effect applied to the player)
	$raining	Raindrops are detected in view
	$gliding	Player is using the glider
	$climbing	Player is climbing

To test these conditions in your own mod, e.g. underwater, you can use the following syntax:
	if $\global\tracking\underwater
		<logic here>
	endif

All of these variables are 1 when the condition is found, 0 otherwise.

DISABLED DEBUG Tracking.ini has been included to enable easy tracking of which conditions are present, provided the help module is installed in ShaderFixes.  Only one of the two Tracking.ini's should be enabled at any given time.
