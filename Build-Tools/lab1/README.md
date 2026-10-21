# Lab 1: Building and Packaging a Java Application with Maven

This lab walks through building, testing, packaging, and running a simple Java Calculator application using **Maven**.

## Objectives

- Install Java and Maven
- Clone the application source code
- Run unit tests
- Build the application and generate the artifact
- Run the application and verify it works

## Steps

### 1. Install Java and Maven

```bash
sudo apt update
sudo apt install -y openjdk-17-jdk maven git
```

Verify the installation:

```bash
java -version
mvn -version
```

### 2. Clone the Source Code

```bash
git clone https://github.com/Ibrahim-Adel15/CalculatorMavenApp.git
cd CalculatorMavenApp
```

### 3. Run Unit Tests

```bash
mvn test
```


### 4. Build the Application

```bash
mvn clean package
```

This compiles the code, runs the tests, and generates the artifact at:

```
target/calculator.jar
```

Verify that the artifact exists:

```bash
ls -l target/calculator.jar
```

### 5. Run the Application

```bash
java -jar target/calculator.jar
```

