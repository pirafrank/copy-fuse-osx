
## WARNING: Unmaintained!

### This repo is no longer maintained and kept just for legacy purposes. This because [Barracuda Networks has discontinued Copy](https://techlib.barracuda.com/Copy/EndOfLife).

# Readme for Copy-Fuse

## Usage Prequisites

<table>
    <thead>
	<tr>
	    <td>General Name</td>
		<td>OS X</td>
	</tr>
    </thead>
    <tbody>
	<tr>
	    <td>Python 2</td>
	    <td>python27</td>
	</tr>
	<tr>
	    <td>Fuse</td>
	    <td>osxfuse</td>
	</tr>
	<tr>
	    <td>Python Fuse Bindings</td>
	    <td>py27-fuse</td>
	</tr>
	<tr>
	    <td>Python URLLib3</td>
		<td>urllib3</td>
	</tr>
	<tr>
	    <td>Python Setuptools utility</td>
	    <td>py27-setuptools</td>
	</tr>
    </tbody>
</table>

## Usage How To

Clone the copy-fuse repo

	git clone https://github.com/copy-app/copy-fuse

'cd' to the copy-fuse repo

   	cd copy-fuse

ensure that copyfuse.py is executable

   	sudo chmod +x copyfuse.py

execute copyfuse.py

   	./copyfuse.py user@email.com password /path/to/mount/point

to unmount your Copy account

	fusermount -u /path/to/mount/point

## Troubleshooting

- SyntaxError: invalid token on line 228

  > The mount point given as the third argument to copyfuse.py does not exist, or is not a directory
