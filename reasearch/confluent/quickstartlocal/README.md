# Quick Start Local

1. Download and Install
```
https://packages.confluent.io/archive/7.1/confluent-7.1.1.zip
unzip confluent-7.1.1.zip
# Install the Confluent Hub client. 
# MacOS
brew tap confluentinc/homebrew-confluent-hub-client
brew install --cask confluent-hub-client
confluent-hub
# Issue
# The operation couldn’t be completed. Unable to locate a Java Runtime.
# Please visit http://www.java.com for information on installing Java.
# Solution
brew tap adoptopenjdk/openjdk
brew search adoptopenjdk
brew install adoptopenjdk11


# Linux
wget http://client.hub.confluent.io/confluent-hub-client-latest.tar.gz
tar -xvf confluent-hub-client-latest.tar.gz
export PATH=/path/to/confluent-hub-client-latest/bin
confluent-hub


# install kafka-connect-datagen
./confluent-7.1.1/bin/confluent-hub install --no-prompt confluentinc/kafka-connect-datagen:0.1.0`

# Start Confluent Platform using the Confluent CLI. 
export PATH=<path-to-confluent>/bin:$PATH
confluent start
# Error: unknown command "start" for "confluent"

```
