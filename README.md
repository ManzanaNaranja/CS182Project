# CS182 Project Option 1

## Setup

1) Download JQF

```git
git clone https://github.com/rohanpadhye/JQF.git
``` 
2) Download Maven [Here](https://maven.apache.org/install.html)

3) Run setup script in the JQF directory
```
./setup.sh
```

## Fuzzing with JQF

1. Run /setup.sh in the JQF directory to build JQF
2. Compile the program under test 
```
javac -cp .:$(./scripts/classpath.sh) SimpleTest.java
```
3. Run JQF Random for 10 iterations

```
/bin/jqf-random SimpleTest testSimpleTest 10
```
