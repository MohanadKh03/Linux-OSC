## Step1:
### 1.1,1.2
![Step1 1,1 2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/372afe2c-84ef-4fd8-bba3-a5799b29da3f)

### 1.3
![Step1 3](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/b1e5acb4-fe9a-4017-ab5c-84bacafe579e)

### 1.4
### The user "osc" is not sudo as shown
![Step1 4 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/74da4fa6-8575-4752-a5dd-59cace9acafb)
### So we will give "osc" privilege by adding "osc" to the sudoers file ... Quoting from the fedora documentation "https://docs.fedoraproject.org/en-US/quick-docs/adding_user_to_sudoers_file/"
> On Fedora, it is the wheel group the user has to be added to, as this group has full admin privileges.
### Now we add the user "osc" to the wheel group
![Step1 4 2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/43fce28c-2b37-49d2-a17b-0254b0742aee)

### 1.5
![Step1 5](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/87193732-fafa-42ae-8906-4cb2b0a10ee9)

--- 

## Step2:
### 2.1
![Step2 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/91dcc04e-13db-462d-a312-ecad8e508c44)
### 2.2
![Step2 2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/255dff2f-3790-4405-97ad-32802a091c71)

--- 
## Step3:
![Step3](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/3630921c-f0e9-4e82-834d-3e777f7d68cd)

---
## Step4:
### 4.1
![Step4 1](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/2d8742b4-1003-4dd3-a348-5f0e8b743086)
### Then we open vim using ``vi`` command
![Step4 2](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/7ad188f0-9e9a-421a-9f1d-9b9911359668)
### Though it seems that it is not being killed normally ?
![Step4 3](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/201c3a3c-0a34-4730-a167-25619c00f162)
### Let's try forcefully killing it using Sigkill (or just add "-9" that is its code number)
![Step4 4](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/c0ce99a0-0baf-464c-9379-ccc09339f7a3)

---
## Step5:
### NOTE: I am using ``Fedora`` so , dnf is probably the best option to use here
![Step5](https://github.com/MohanadKh03/Linux-OSC/assets/67065678/dce5413f-d66a-49f0-9c42-0b3750305903)





