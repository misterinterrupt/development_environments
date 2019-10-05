# update package manager
`sudo apt update`

# install build stuff that lots of things use like e.g. gnu make
`sudo apt-get install build-essential`


# install atom from snap store
# install vs code from snap store

#install docker-repositories
`sudo apt-get install apt-transport-https ca-certificates curl software-properties-common`

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

`sudo apt-key fingerprint 0EBFCD88`#(check that the fingerprint matches)

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"`

`sudo apt-get update`

#install docker-ce
`sudo apt-get install docker-ce docker-ce-cli containerd.io`

#make docker cli usable without sudo every time (hacker may kill you for that tho)
`sudo groupadd docker
sudo usermod -a -G docker $USER`


#install docker-compose
`sudo apt-get install docker-compose`


#install n to $HOME/n (defaults to this)
`curl -L https://git.io/n-install | bash`
`. /home/interrupt/.bashrc`

#install npm
`curl -O -L https://npmjs.org/install.sh | bash`
