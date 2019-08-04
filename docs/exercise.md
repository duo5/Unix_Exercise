# Unix exercise


## Create folder "unix" and folder "data" into "foo"
- ```mkdir foo```
- ```mkdir foo/unix```
- ```mkdir foo/data```
## Create file "foo.txt" using at least 3  difference command.
- ```echo "content" > foo.txt```
- ```cat > foo.txt```
- ```touch foo.txt```
- ```vim foo.txt```
## Copy the file "foo.txt" into "foo.txt.copy".
- ```cat foo.txt > foo.txt.copy```
## Rename the file "foo.txt.copy" to "foo2".
- ```mv foo.txt.copy foo2```
## Move the file "foo2" into the "data" subdirectory.
- ```mv foo2 ./data```
## Create a new subdirectory called "new" in the unix directory.
- ```mkdir unix/new```
## Move the file "foo2" in the "data" directory into the "new" directory.
- ```mv data/foo2 unix/new```
## Move the file "foo2" in the "new" directory back into the "unix" directory and change the name to "foo.old".
- ```mv unix/new/foo2 unix```
- ```mv unix/foo2 unix/foo.old```
## Delete the file "foo.old".
- 
