# Experiment 11 – JavaScript Testing Using Selenium

## 1. Check Software Installations

```powershell
java -version
mvn -version
```

## 2. Open the Project

1. Download the ZIP file from the GitHub repository.
2. Extract the ZIP file.
3. Open the extracted project folder in VS Code.
4. Open Terminal → New Terminal.

Make sure you are inside the folder containing `pom.xml`.

## 3. Check Project Files

```powershell
dir
```

Check that the following files are available:

- pom.xml
- program.html
- src

## 4. Execute Selenium Tests

Open the terminal in the project folder containing `pom.xml`.

```powershell
mvn clean test
```

Wait for Maven to compile the project and execute the Selenium test case.

## 5. Expected Application Output

The JavaScript application should open in Google Chrome.

Expected behaviour:

- Initially, the displayed value is 0.
- Selenium clicks the increment button.
- The displayed value changes to 1.

## 6. Expected Test Results

```text
Tests run: 1
Failures: 0
Errors: 0
Skipped: 0

BUILD SUCCESS
```

## 7. View Test Reports

```powershell
Get-Content .\target\surefire-reports\*.txt
```

## Important Notes

1. Java 21 and Maven must be installed.
2. Google Chrome must be installed.
3. Selenium dependencies are managed through pom.xml.
4. Internet access may be required to download Maven dependencies and browser drivers.
5. Open the terminal inside the project folder containing pom.xml.
6. Execute `mvn clean test` to run the Selenium test case.
7. No Docker or Kubernetes is required for this experiment.
