# EOS Manually Build for macOS
- When you could not build eos with 'eos_build.sh'. ex) error occurred!
  - DO Manually Build
  <pre><code>
  mkdir -p ~/eos/build && cd ~/eos/build
  </code></pre>
  - Use this cmake command
  <pre><code>
  cmake -DBINARYEN_BIN=~/bnaryen/bin -DWASM_ROOT=/usr/local/wasm -DOPENSSL_ROOT_DIR=/usr/local/opt/openssl -DPONSSL_LIBRARIES=/usr/local/opt/opebssk/lib -DBUILD_MONGO_DB_PLUGIN=true ..
  </code></pre>
  - Then make command
  <pre><code>
  make -j$( nproc )
  </code></pre>
