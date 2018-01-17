- With Scratch open, the Pi GPIO extension added, and a button connected to a GPIO pin, find the `when flag clicked`{:class="blockevents"} block and drag it into your Scripts area.

	![flag block](images/flag.png)

- Find the `set gpio ( ) to [output high]`{:class="blockmoreblocks"} block, drag it into you Scripts area, and connect it with the other block.

	![output block](images/output.png)

- Next to the `[output high]`{:class="blockmoreblocks"} field, there is a small arrow which you can click to set the field to `[input]`{:class="blockmoreblocks"}. Doing so tells Scratch that the pin will be connected to an input, such as a button. You also need to set the block to use the correct pin. The example is using GPIO pin 4.

	![input block](images/input.png)

- One way of detecting button pushes is to use a `forever`{:class="blockcontrol"} loop containing an `if else`{:class="blockcontrol"} block. Find the `forever`{:class="blockcontrol"} block in the **Control** menu and drag it into your Scripts area. Then grab the `if else` block and place it into the loop.

	![forever if](images/forever.png)
	![if else block](images/ifelse.png)

- Next, find the `gpio ( ) is high?`{:class="blockmoreblocks"} block from **More Blocks**, and drag it into you Scripts area.

	![high block](images/high.png)

- Set the pin number to the one of the pin which you have wired your button to. This block can now be placed into the `if else`{:class="blockcontrol"} block.

	![high block connected](images/high-connect.png)

- The pin will be `low`{:class="blockmoreblocks"} when the button is pushed, and `high`{:class="blockmoreblocks"} when the button is not pushed, and you can use `say`{:class="blockmoreblocks"} blocks to show this.

	![completed script](images/complete.png)

- Here's a video showing you the whole process.

	<video width="560" height="315" controls>
	<source src="https://s3.eu-west-2.amazonaws.com/learning-resources-production/projects/rpi-scratch-button/c79b0bdd8e3d6cee705ccde31f7d7d64ace5be24/en/images/scratch-pi-gpio-button.webm" type="video/webm">
	Try using Firefox or Chrome if your browser does not have WebM video support.
	</video>
