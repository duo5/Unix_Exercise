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
- ```rm -f unix/foo.old```
## Remove the "new" subdirectory.
- ```rm -r unix/new```
## Create file "verylong.seq"   with some text insideCreate file "verylong.seq"   with some text inside
- ```echo "Some text inside" > verylong.seq```
## Dis play the file "verylong.seq" on the screen using "cat" , "more"  command.
- ```cat verylong.seq```
- ```more verylong.seq```
## Walk upwards and downwards in the file using the "more" program.
- ```more``` khá giống với cát nhưng khác ở chỗ là nó trình bày theo từng trang nên ta có sử dụng phím ```space``` để lướt từng trang một và sử dụng phím mũi tên lên xuống để di chuyển.
## Search for the word "Length" using the "more" and the "less" program, compare the   results.
- Để search bằng more ta bấm ```/key_word``` giống vi hay vim để search tương tự less cũng có thể sử dụng ```/``` hoặc ```?``` để search
