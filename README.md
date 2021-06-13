# PlotJuggler MQTT plugin

This repository contains a streaming plugin for
[PlotJuggler](https://github.com/facontidavide/PlotJuggler) that
uses MQTT as transport layer.

The protocols which are recognized are JSON, CBOR, MessagePack and BSON.

## Build

To build this plugin, PlotJuggler must be installed in your system.

For instance, in Linux, you should perform a full compilation and installation:

```
git clone https://github.com/facontidavide/PlotJuggler.git
cd PlotJuggler
mkdir build; cd build
cmake ..
make
sudo make install
```

The compile this plugin:
```
git clone --recurse-submodules https://github.com/PlotJuggler/plotjuggler-mqtt.git
cd plotjuggler-mqtt
mkdir build; cd build
cmake ..
make
sudo make install
```

## Plugin installation

If PlotJuggler can't find this plugin, check the folder where the file
`libDataStreamMQTT.so` is located and add it manually in:

    App -> Preferences... -> Plugins

