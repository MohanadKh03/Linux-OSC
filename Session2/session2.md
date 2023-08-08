## Step1
### First unzip the directory
![Step1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/653ae39c-7307-4c21-832a-239ee9b2c9fa)

--- 
## Step2
### Discover what is inside the folder .. It seems there is a hidden file ? 
![Step2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/0697a9cf-5463-4048-9732-8e19086d9ddf)

---
## Step3
### Indeed there is a hidden file archived , So let's extract what's inside and see what is inside 
![Step3](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/7df013b1-a9ae-405e-bb20-0f706302492f)
![Step3 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/2b44ffe7-1085-430e-957d-14ff551a8b18)

---
## Step4
### After knowing the stuff extracted ``(using -v)`` it turns out these are hidden directory , Let's dive deep inside the hidden directory
![Step4](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/61101f25-8837-4805-8ac0-1e02bbd685db)
### Another README file , Let's have a look at it 
![Step4 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/a1a51840-52c2-417b-bac0-c31e44c5637b)
### So it seems we need to decompress the other directory/file which is ``level-2`` BUT this is without an extension , We need to give it an extension to decompress it as written above

---
## Step5
### Rename the ``level-2`` to ``level-2.gz`` and then we can decompress it using ``gunzip`` and see what kind of file is it
![Step5](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/74b17e3e-c109-426e-8397-5c178c096605)
### So after decompressing it seems that this is an archive ``tar`` , Let's extract it
![Step5 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/6c4dc45c-12a4-416b-98e5-e35c6b65b493)
### Because -v is used , All the stuff inside the ``level-2`` directory is shown , There are A LOT of files/directories inside I couldnt get all of them in the Screenshot though
### BUT anyways let's go to that directory and see what's inside 

---
## Step6
### That's A LOT of files/directories .. For some reason they all seem to be empty ? 
![Step6](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/f8065700-e215-4ab3-bd99-ff0d504055d4)
### Maybe there is a directory/file that is not empty and that is the one we should get into ? How do we do this ? using ``find`` instead of just randomly choosing files and check whether they are empty or not
![Step6 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/954c26d1-ede5-46fd-91f5-d523e658c76c)
### And indeed there is one non-empty directory and one non-empty file inside that directory !

---
## Step7
### Let's go to that file and see what can we do with it
![Step7](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/d50536bf-b1a1-4cde-a541-a16471c891ea)
### So it seems that this is another gzip compressed file/directory ! As before , We need to rename its extension in order to be able to unzip the file/directory
![Step7 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/aaa8f7b8-0741-44d1-999f-4421c0dfa3d9)
### After renaming and decompressing , It seems that this is an archive ``tar`` .. Now we extract what's inside it
![Step7 2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/7074ed13-df43-4cd0-a414-327995ffa77c)
### Yet again , there are so many files this time .. There is probably a file that is not empty so let's find it and see how this will end up
![Step7 3](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/22c3b8fe-e2c5-41e0-bd9d-d71a13ce74cb)
![Step7 4](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/07674349-c863-4939-895f-90cdfa0c57ac)
### Some non empty files/directories again , Let's check each one of them 
![Step7 5](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/f633d0aa-446b-4963-aac3-f2b9da70027c)
### So we have to get the link for some file to get its size , Let's do this using the ``ls -l``
![Step7 6](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/6e87dd79-7f84-4f52-8640-ec4225583b89)
### There it is , the link to that other file/directory .. Let's go check it out !
![Step7 7](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/d61a970b-6186-4181-a383-79815366c594)
### The file's size that we are looking for is 239 KB , Let's search for a file that has this exact size or anything greater than 2KB , Most if not all of the files are empty anyway 
![Step7 8](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/8008c3c2-1ada-46a3-8808-04c4cf602a5e)
### Let's go to that directory 

---
## Step8
### Inside this directory are a lot of files , Let's do the same thing as before and look for non-empty files
![Step8](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/48870e78-a579-43da-88a0-f3653fc74575)
### There it is the only non-empty file , What is inside this ? 
![Step8 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/f1159de1-1b62-4c8e-8d81-0c058f25499a)
#### ``The end of the many finds/decompressions and extractions ! ``


 


