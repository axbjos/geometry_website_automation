# Geometry Calculator Web App

Source code and automation for and example (and very simple) Python Flask Web App

## To Simply Run the Application:

1. Clone this repo to any computer capable of running Python 3.

    ```git clone https://github.com/axbjos/geometry_web_complete.git```

2. Install the Python 3 "Virtual Environment" module (best to run this in a venv, Ubuntu example provided.  Other OS will be different.).

    ```sudo apt install python3.8-venv```

3. cd into the application directory.

    ```cd geometry_web_complete```

4. Create a Virtual Environment.

    ```python3 -m venv venv```

5. On Ubuntu, activate the Virtual Environment using.

    ```source venv/bin/activate```

6. Install the dependencies.  

    ```pip3 install -r requirements.txt```

7. Run the Application (run on port 5000).   

    ```python3 Geometry.py```

If you want to run the Python Unit tests, use the Pyunit module.  python3 -m unittest <testfile.py>

## To Build/Run the Application as a Docker Container:

1. Clone this repo to a server running Docker Engine

    ```git clone https://github.com/axbjos/geometry_web_complete.git```

2. cd into the *geometry_web_complete* directory

    ```cd geometry_web_complete```

3. Run Docker Build to build the container

    ```docker build --pull --rm -f "Dockerfile" -t geometrywebdocker:latest "."```

4. Run the container

    ```docker run --rm -d  -p 5000:5000/tcp geometrywebdocker:latest```

## Infrastructure Automation Examples

Use the following Infrastructure Automation Examples for inspiration on how to build your own Infrastructure.


### Vagrant

- Must have Vagrant and a suitable hypervisor.  Use Virtualbox, VMare Fusion, VMware Workstation.  

- Download the desired Vagrant File, put it in a directory, and rename it "Vagrantfile"   Then simply *vagrant up*

- All examples use the ubuntu/focal64 (aka Ubunt 20.04 Vagrant compatible template "box")

- *M1 macOS examples coming soon*  Will need to use VMware Fusion

**Vagrantfiles:**

VagranfileFlaskApp - Vagrant automation to build an Ubuntu Server and automate all steps to install dependencies and run the Flask Application.  At the end, the Flask app is up and running on port 5000.  

VagrantffileDockerFlaskApp - Vagrant automation that builds an Ubuntu Server, automates all steps to install Docker Engine.  The automates building the Flask Application Container and running.  At the end, the Flask App is running on port 5000 as a container.

VagrantfileDockerOnly - Vagrant automation to build an Ubuntu Server running the Docker Engine - that's it.  Log in and build and run any container.

### Terraform

The Terraform directory contains two different .tf files.

- axnetlabs.tf --> only has usefulness in the Axnet VMware Homelab of Joe Axberg.  This file will create a standard Ubuntu 20.04 server in that environment. By default an Ubuntu 20.04 with 1GB RAM, 1 CPU, and 20GB HDD will be created.

- senglab.tf --> only has usefulness in the Dunwoody Software Engineering VMware Lab.  This file will create a standard Ubuntu 20.04 server in that environment. By default an Ubuntu 20.04 with 1GB RAM, 1 CPU, and 20GB HDD will be created.

- awslab.tf --> coming soon, will work with AWS 







