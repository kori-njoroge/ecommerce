The Project was developed on windows Computer, the following the guides are for a windows computer

**1. Cloning the Project from Github**
> Open command  prompt and enter the command below.
``` git clone https://github.com/siraj3838/weShop-Client.git```
*Reason*: This command fetches all the files from the remote repository and sets up the necessary configuration to allow us to work with the repository locally.

 **2.Open the project in Vs code or the Editor of choice**
 > Create a 'Dockerfile" in the parent directory of the project.
 ![Project structure](image.png)
 > Copy the contents of the docker file I have submited and paste in the docker file.
 > Right click on the Project folder and select open in Intergrated Terminal
 ![open in Inetergrated Terminal](image-1.png)

**3. Working With Docker**
> a. Building the Docker Image - In Terminal Enter the following command
```docker build -t my-vite-app . ```
You should get an output in your terminal as the screenshot attached.
![Building Docker Image](image-2.png)

> b. Run the Docker Container
 - the port used to access the application in localhost is ```5173```
 > Run the following command in Terminal after the fisrt one.
 ```docker run -p 5173:5173 my-vite-app```
You should get an output in your terminal as the screenshot attached
![Run the docker container](image-3.png)


**4. Access the application after running the container**
> Open your browser, on a new tab paste the URL below and click 'Enter'
```http://localhost:5173```
You should get a page as shown belo.
![Project Home Pagee](image-4.png)