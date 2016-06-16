# m2p
Maven .classpath generator for multi-maven project

### How to use

* Checkout and build

```
git clone https://github.com/Shvid/m2p
cd m2p
mvn clean install
```

* Setup PATH (on MacBook)

```
pwd
cd ~
nano .project
export PATH=$PATH:{from pwd}/target/m2p/bin
```

* Go to your multi-module maven project
```
cd my-maven-project
```

* Build your maven project to generate sources
```
mvn clean install
```

* Generate eclipse classpaths for sub-module projects
```
mvn eclipse:eclipse
```

* Join classpath entries from sub modules
```
m2p
```

* .classpath will be generated by using '.classpath' files from sub-modules
* Enjoy

### .m2pignore

Add file with name .m2pignore for each folder in multi-module maven project that you want to ignore


