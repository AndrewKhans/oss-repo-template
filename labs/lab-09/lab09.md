# Example 0

When first attempting to run this example, I got an issue related to permissions being denied. After running the example with `sudo`, all worked fine. The issue is likely due to the way that I installed docker.

### Whalesay Output
![image](https://i.gyazo.com/56bc86f9cbd95d3c94d38faa4b0417aa.png)

# Example 1

Downloading and running an Ubuntu virtualization took just seconds in this example. Since it was so quick to create, I'm certainly going to make use of docker in the future whenever I'm working on a project and I need to download packages that I don't intend to keep around.

### Cowsay Output

![image](https://i.gyazo.com/d342e1bc364e8869ef5cacc31d5126b1.png)

# Example 2

Setting up communication between containers is very simple. This feature of docker is certainly useful for projects that have both a client and a server.

### Rocketchat
![image](https://i.gyazo.com/246a5a63495657340717f1889d94be5e.png)

### Docker ps
![image](https://i.gyazo.com/981102dc810aba3ab74dfc319b557495.png)


# Example 3

Seeing a docker container communicate with the outside operating system is very cool. I can see this being useful for projects written in a container that have a front-end GUI that users will want to see and interact with.

### Flask Server Output
![image](https://i.gyazo.com/75eb4771454f9dc7028aade38d906352.png)


# Example 4

Docker-compose allows docker projects to use other docker images. This example used a .yml file to speed up the process of running a project with multiple docker images, automating the step of running the database.

### Posting a Few Messages
![image](https://i.gyazo.com/a021d367c3508e6252572a3a75f0d903.png)

### Modifying a Message
![image](https://i.gyazo.com/6f31570940c417f47d329fcc480a7d8e.png)

### Deleting a Message
![image](https://i.gyazo.com/8a85eecdaa019bcd754d8ab572e0ab24.png)
