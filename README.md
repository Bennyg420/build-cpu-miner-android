# build-cpu-miner-android

pkg update && pkg upgrade -y
pkg install git automake autoconf pkg-config libcurl libjansson libssl libgmp zlib clang make -y



git clone https://github.com/JayDDee/cpuminer-opt.git


cd cpuminer-opt


./build.sh


or

./autogen.sh
CFLAGS="-O3 -march=native" ./configure --with-curl
make -j $(nproc)

Run Miner:

./cpuminer -a <ALGO> -o <POOL_URL> -u <USERNAME> -p <PASSWORD>
