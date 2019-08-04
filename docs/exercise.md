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
- ```echo "very long text inside" > verylong.seq```
## Dis play the file "verylong.seq" on the screen using "cat" , "more"  command.
- ```cat verylong.seq```
- ```more verylong.seq```
## Walk upwards and downwards in the file using the "more" program.
- ```more``` khá giống với cát nhưng khác ở chỗ là nó trình bày theo từng trang nên ta có sử dụng phím ```space``` để lướt từng trang một và sử dụng phím enter để di chuyển từng dòng. Không thể sử dụng phím lên xuống 
## Search for the word "Length" using the "more" and the "less" program, compare the   results.
- Để search bằng more ta bấm ```/key_word``` giống vi hay vim để search tương tự less cũng có thể sử dụng ```/``` hoặc ```?``` để search.
- Khi search bằng more nó sẽ chỉ chuyển tới trang mà có từ search đó còn less nó sẽ bôi đậm từ khóa search.
## Access the online help in the "more" program, then exit from the program. 
- Không hiểu rõ câu hỏi.
- Sử dụng lệnh ``` man more```
## Change the permission of your own file "foo.txt" so that anyone may read it. 
- ```chmod 777 foo.txt```
## Change the permission of the file to denies to  your access 
- ```chmod u-rwx foo.txt```
## Change the owner file to root user
- ```sudo chown root foo.txt```
##  Write the command to search hello, how, are, you in a file. 
- ```grep 'hello\|how\|are\|you' /home/duong/test.txt```
## Write command to find a file that have text “where are you”
- ```grep -iRl "where are you" /home/duong/Downloads```
## Write command to search services using name
- ```ps aux | grep -i jenkins```
## Write command to stop/start, kill a services using PID
- Stop ```kill -STOP 321321```
- Restart ```kill -CONT 321321```
- Kill ```kill -9 321321```
## Write the command to get the PID of process named “runme.sh”
- ```pidof runtime.sh```
## Write command to display full log file, 100 last lines of log file
- ```tail -n 100 log_file```
## Write command to search a text from log file
- ```tail -n 100 log_file | grep search_text```
## Using less command to search a text in a file
- Sau khi dùng less để đọc một file sử dụng phím ```/``` hoặc ```?``` để tìm đoạn văn bản trong file đó.
## Write command to set environment variable in unix
- ```export JAVA_HOME=/usr/java/jdk1.5.0_07/bin/java```
## Write command to install a package in unix.
- ```sudo apt-get install default-jdk```
## Write command to create a execute file 
- ```touch run.sh```
## Compare 2 files txt1 and txt2 to show the difference 
- ```diff file1 file2```
## Write command to search a text that ignore the sensitive case. for eg: search science in science.txt.
- ```grep -i science science.txt```
## Search and display 10 lines around the text found 
- ```grep -A 10 -i science science.txt```
## Search and display 10 first lines around the text found 
- ```grep -B 10 -i science science.txt```
##  Search a text in tab <begin> and </begin> 
- ```grep -o '<begin>.*</begin>' science.txt | sed 's/\(<begin>\|<\/begin>\)//g' ```
