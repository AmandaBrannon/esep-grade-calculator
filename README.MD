# ESEP Grade Calculator

This library is a simple utility that is written in Go and can help users to calculate their grades. It contains fields for three categories:

Assignments - 50% weight
Exams - 35% weight
Essays - 15% weight

The grading scale is a follows, with a C being passing:
A >=90
B >=80
C >=70
D >= 60
F <60

## How to use:
1. Create a new instance of the calculator class with "YourNameHerecalc = NewGradeCalculator()"
2. Add your (already weighted) grades with "YourNameHerecalc.AddGrade("Name of Thing", IntegerGrade, TypeName)" where IntegerGrade is the Grade you got as an integer, and TypeName being one of three valid words of "Assignment", "Exam", or "Essay".
3. Continue adding all of your grades until complete
4. Get your final score with "final_score := YourNameHerecalc.GetFinalGrade()"
5. Print out your final score with print(final_score)


## Package Requirements
Runtime requirements:
Golang 1.24+

## To get on the local machine
Fork this repository or the original repository to your machine, then make sure all packages are downloaded. Run the unit tests through the terminal.

## Run unit tests:
```
cd grade_calculator/
go test ./...
```

## Run unit tests with code coverage:
```
cd grade_calculator/
go test -coverprofile=coverage.txt ./...
```