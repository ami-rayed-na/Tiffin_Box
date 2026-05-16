#basic #linux 

Sorry, I don’t have an introduction for this topic in mind right now. I’ll update it when I come up with one. For now, let’s dive into the topic.

### cat 

`cat` is the short form of *concatenate*, meaning to combine pieces together(not the domestic one you have in your home). `cat` command can be used in various ways. But the most popular one is to read a file.
To read a file just use the file name, e.g:
```
user@ubuntu:~$ cat flag.txt
```

Also we can create a file using `cat` command. Just a redirect, denoted with the ">" symbol, and a name for the file we want to create. e.g:
```
user@ubuntu:~$ cat > flag.txt
```

When you press <span class="lal">ENTER</span>, linux will go into interactive mode & wait for you to start entering contents. This can be puzzling because the prompt disappear, just simply type your content it will go into the file 