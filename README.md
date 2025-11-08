# build-cpu-miner-android

pkg install git build-essential automake autoconf pkg-config libcurl openssl libssl-dev libjansson libjansson-dev libgmp libgmp-dev zlib zlib-dev -y


git clone https://github.com/JayDDee/cpuminer-opt.git


cd cpuminer-opt


./build.sh


or

./autogen.sh
CFLAGS="-O3 -march=native" ./configure --with-curl
make -j $(nproc)

Run Miner:

./cpuminer -a <ALGO> -o <POOL_URL> -u <USERNAME> -p <PASSWORD>
