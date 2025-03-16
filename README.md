# list-xmr

sudo apt update && sudo apt upgrade -y

sudo apt install -y git build-essential cmake libuv1-dev libssl-dev libhwloc-dev

git clone https://github.com/xmrig/xmrig.git
cd xmrig

mkdir build && cd build

# optional
cmake -DWITH_HWLOC=OFF ..
-------------------------------------------

cmake ..
make

# Option 1: Command-Line (Quick Fix)
# Run XMRig with 4 threads at 80% usage using --threads=4 and --cpu-max-threads-hint=80:

./xmrig -o rx.unmineable.com:3333 -a rx -k --threads=4 --cpu-max-threads-hint=80 -u XMR:46AEHQwkApgAJ6HpGoYsKFELrSytXbn5nhsMkUFwxNm9UnHWBiAoiPJRS8MnHSGXv3aw1FD3pRMU1AmUKFrKST2iV2wm56H.tauhidxv

# To limit XMRig to 3 threads while using your current mining command, simply add the --threads=3 flag like this:

./xmrig -o rx.unmineable.com:3333 -a rx -k --threads=3 -u XMR:46AEHQwkApgAJ6HpGoYsKFELrSytXbn5nhsMkUFwxNm9UnHWBiAoiPJRS8MnHSGXv3aw1FD3pRMU1AmUKFrKST2iV2wm56H.tauhidxv

# normal 

./xmrig -o rx.unmineable.com:3333 -a rx -k -u XMR:46AEHQwkApgAJ6HpGoYsKFELrSytXbn5nhsMkUFwxNm9UnHWBiAoiPJRS8MnHSGXv3aw1FD3pRMU1AmUKFrKST2iV2wm56H.tauhidxv
