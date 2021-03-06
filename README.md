# Codefresh Terminal

Provides easy access to Docker container's insides. Follow these steps and you will know what inside your container :)

# Step 1: create terminal service and build it

Click Add Service button and use this link https://github.com/containers101/cf-terminal as repo URL. Click build button in the end. It will create terminal image for you. 

<p align="center">
  <img src="./images/step 1.gif">
</p>

# Step 2: add terminal in your composition

If you don't have composition yet please follow this link https://g.codefresh.io/compositions/new/services and create a new one. If you already have composition just use this composition. In our example we created a new composition for this service https://github.com/containers101/who-m-i (we called it my-service) and used https://github.com/containers101/cf-terminal/blob/master/docker-compose.yml for configuration. As you can see we shared app folder from my-service with terminal.

<p align="center">
  <img src="./images/step 2.gif">
</p>

Don't forget to launch your composition in the end.

# Step 3: get access to terminal

So all is done. Now we can get access to terminal and check what exactly is placed inside app folder. Open this link https://g.codefresh.io/environments/ and click Open App link.

<p align="center">
  <img src="./images/step 3.gif">
</p>

Username and password can be defined by environment variables: USERNAME/PASSWORD.
If not defined, login to terminal using: user/pass.

## About Containers 101

[Containers 101](https://www.meetup.com/Containers-101-meetup/) is online/offline meetup group based in Mountain View that provides guides and helps developers work with Containers. Created by [Codefresh](https://codefresh.io/) which provides environments for every commit, Docker CI and CD, and an embedded registry. 

[Join Containers 101](https://www.meetup.com/Containers-101-meetup/)
Learn more about [Codefresh](https://codefresh.io/)

