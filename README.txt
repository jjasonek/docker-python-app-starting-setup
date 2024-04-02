PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup> docker run --help
...

-i, --interactive                      Keep STDIN open even if not attached

...

-t, --tty                              Allocate a pseudo-TTY


To run this interactive Python app, we combine flags -i and -t.
Running then looks like this:

PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup> docker run -it 34d52ade3c6165a202
Please enter the min number: 5
Please enter the max number: 6
6
PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup>


and re-run can look like this:

PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup> docker start -a crazy_driscoll
Please enter the min number:
PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup> docker start -a -i crazy_driscoll
Please enter the min number: 5
Please enter the max number: 15
13
PS C:\Training\Docker\python-app-starting-setup\python-app-starting-setup>
