# MongoDB

1. For Windows/Mac/Linux:

- Visit [MongoDB Download Center](https://www.mongodb.com/try/download/community) and download the appropriate version for your operating system.
- Follow the installation guide for your OS.

2. For Linux (Ubuntu): Run the following commands in your terminal to install MongoDB:
```
    # Import the public GPG key:
    wget -qO - https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -
    
    # Create the MongoDB source list file:
    echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list
    
    # Update the system's package list:
    sudo apt-get update
    
    # Install MongoDB:
    sudo apt-get install -y mongodb-org
    
    # Start MongoDB:
    sudo systemctl start mongod
    sudo systemctl enable mongod
```
