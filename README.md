# evm2llvm
Small evm -> llvm translator using evmjit

# Building

  Checkout evmjit submodule (and dependencies) and make.
  ```
  git submodule update --init --recursive
  make
  ```
  
  update 
  g++ -g lift.cc -I./evmjit/libevmjit -I./evmjit/include -I./evmjit/evmc/include -I ./evmjit/deps/include/  ./evmjit/build/libevmjit/libevmjit-standalone-thin.a -ldl -lpthread

