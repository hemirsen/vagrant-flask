# Vagrant is an open-source tool that helps us to automate the creation and management of Virtual Machines. In a nutshell, we can specify the configuration of a virtual machine in a simple configuration file, and Vagrant creates the same Virtual machine using just one simple command. It provides command-line interfaces to automate such tasks.

-------------

**1.** Vagrant will automatically build and run images based on local Dockerfile. This is useful for iterating on an application locally that is built
into an image later.

**2.** When the repository is committed, a new image will be pushed to docker hub (this is what `.github/workflows/push-to-hub.yml` does)

**3.** After committing we need to run bash.sh script.

-------------
 #USAGE
 
**1.** Clone the repository.

**2.** Create your github repository and add your dockerhub username, access token as secret.

**3.** You must change dockerhub username and repository name in `.github/workflows/push-to-hub.yml` and `./Vagrantfile`.

**4.** Run `vagrant up` command and its ready to use.
