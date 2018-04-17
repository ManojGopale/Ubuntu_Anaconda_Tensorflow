Bootstrap: docker
From: ubuntu:latest

%post
	mkdir /extra
	mkdir /xdisk
	mkdir /rsgrps
	apt-get install wget
	wget https://repo.continuum.io/archive/Anaconda3-5.1.0-Linux-x86_64.sh
	apt-get install bzip2
	bash Anaconda3-5.1.0-Linux-x86_64.sh -f -b -p $HOME/anaconda
	export PATH="$HOME/anaconda/bin:$PATH"
	conda update conda
	pip install --upgrade tensorflow
	pip install keras
