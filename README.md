# projectM-bugfixes [!!THESE BUGFIXES ARE NO LONGER NEEDED, AS THE LATEST VERSION OF PROJECTM HAS FIXED IT!!]

Patch for projectM to fix text rendering bugs.

bugfixes-22.02.2015.patch

This package is made from the abs Arch Linux package. It is tested still working september 2016 ;)

(The following commands should only be executed on Arch Linux)

Perform a full system upgrade and install the 'abs' package:

sudo pacman -Syu abs
then run 'abs' as root to create the ABS tree by synchronizing it with the Arch Linux server:

sudo su
then enter your password

abs
when abs is finished you can exit the root prompt by:

exit
create a working folder in your home directory:

mkdir -v ~/abs
now copy the projectM folder from the tree abs created into our abs home folder:

sudo cp -rv /var/abs/community/projectm ~/abs/projectm
cd ~/abs/projectm
now we must give ourselfes user access so we don't have to compile as root:

sudo chown -R <your-user>:<your-user> ../projectm
now enter the folder and download the patch file (if you don't have 'git', simply 'sudo pacman -S git'):

git clone https://github.com/kaarejens/projectM-bugfixes

cp -f projectM-bugfixes/* .
Make the project and install it (this will take some time):

makepkg -scCi
That's it! You should now have the patched version of projectM installed on Arch!
