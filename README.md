# Scripts

sudo apt install zram-tools
echo -e "ALGO=zstd\nPERCENT=100" | sudo tee -a /etc/default/zramswap
sudo service zramswap reload

apt install openssh-server screen python3 git default-jdk android-tools-adb bc bison \
build-essential curl flex g++-multilib gcc-multilib gnupg gperf imagemagick lib32ncurses-dev \
lib32readline-dev lib32z1-dev  liblz4-tool libncurses5-dev libsdl1.2-dev libssl-dev \
libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc yasm zip zlib1g-dev \
libtinfo5 libncurses5

wget https://www.python.org/ftp/python/2.7.18/Python-2.7.18.tgz
sudo tar xzf Python-2.7.18.tgz
cd Python-2.7.18
sudo ./configure --enable-optimizations
sudo make altinstall
cd 
sudo ln -sfn '/usr/local/bin/python2.7' '/usr/bin/python2'
