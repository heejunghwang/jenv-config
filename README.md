# Jenv Config

To manage java versions locally, you can use jenv config(It is similar to nvm in node.js). This is repo for simple jenv command shell.

## Prerequisite

1. Install Java(s)
```
brew tap AdoptOpenJDK/openjdk
brew install adoptopenjdk11
```

2. Install Jenv
```
brew install jenv
```


2. Set config
2-1. Check Java versions
```
jenv versions
```

2-2. Add Java to jenv

You can add the Java versions you want to install.

```sh
jenv add /Library/Java/JavaVirtualMachines/<target version>/Contents/Home
```

This is example command to add Java version.

```sh
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home

jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-12.jdk/Contents/Home

jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home
```

3. Chang java version
You can use the simple shell to change java versions.

```
./java11-local.sh
```