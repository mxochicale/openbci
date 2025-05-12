# build gtec driver

## building driver
```
make clean
make gtec_amplifier
```

## Dependencies
```
sudo apt update
sudo apt install protobuf-compiler
protoc
# https://www.geeksforgeeks.org/how-to-install-protobuf-on-ubuntu/

# git clone git@github.com:findepi/multiplexer.git
# and add multplexer depencencies

```


## issues
```
                 from ../base/AmplifierServer.cpp:7:
../base/azlib/preproc/common.h:59:4: error: #error "Hey, Google, define GOOGLE_ATTRIBUTE_ALWAYS_INLINE!"
   59 | #  error "Hey, Google, define GOOGLE_ATTRIBUTE_ALWAYS_INLINE!"
      |    ^~~~~
In file included from ../base/azlib/logging.h:35,
                 from ../base/azlib/timer.h:36,
                 from ../base/multiplexer/BasicClient.h:32,
                 from ../base/multiplexer/Client.h:29,
                 from ../base/multiplexer/backend/BaseMultiplexerServer.h:35,
                 from ../base/AmplifierServer.h:11,
                 from ../base/AmplifierServer.cpp:7:
../base/azlib/signals.h:29:10: fatal error: boost/signals.hpp: No such file or directory
   29 | #include <boost/signals.hpp>
      |          ^~~~~~~~~~~~~~~~~~~
compilation terminated.
make: *** [../base/Makefile.common:72: ../build/AmplifierServer.o] Error 1

```
