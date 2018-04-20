Bootstrap: docker
From: ubuntu:latest

%post
	apt-get update
	apt-get install wget -y
	apt-get install bzip2 -y
	apt-get install vim -y

	wget https://repo.continuum.io/archive/Anaconda3-5.1.0-Linux-x86_64.sh
	bash Anaconda3-5.1.0-Linux-x86_64.sh -f -b -p $HOME/anaconda
	export PATH="$HOME/anaconda/bin:$PATH"

	conda update conda -y
	pip install --upgrade tensorflow
	pip install keras
	conda update conda -y
