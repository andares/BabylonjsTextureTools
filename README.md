# Babylon.js Texture Tools with Multi-Level Output

```sh
# Install emsdk
sudo apt install ninja-build cmake
git clone https://github.com/emscripten-core/emsdk.git
cd emsdk
./emsdk install latest
./emsdk activate latest
source ./emsdk_env.sh
# To see the available versions, run ls emsdk_env.*, then run the one that matches your shell.
cd ..

# Setup Texture Tools
git clone git@github.com:andares/BabylonjsTextureTools.git
cd BabylonjsTextureTools
git submodule update --init --recursive
cd native/LTCGenerator
# Now open CMakePresets.json and find the rsh configuration key. Then, update its value to "Linux" or "Windows" based on your operating system.
cmake --preset wasm
cmake --build --preset wasm
pnpm install
pnpm start
# Navigate to http://172.24.47.146:8080/ in your browser to get started.
```
