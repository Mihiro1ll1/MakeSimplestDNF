# MakeSimplestDNF
**[Python3]** Optimization DNF with Quine-McCluskey algorithm implementation

## Input
Logical function written in DNF (Disjunctive Normal Form)   
Example: **[[1],[-1,-2,3],[-1,3]]**  
  It means **A+A'B'C+A'C** (' means NOT).  
  Each number represents a corresponding logical variable.  
  Minus signifies the negation of its logical variable.  

## Output
The simplest form after conversion
Example: **[[1],[3]]**   
  This result is the output to the above example of Input.  
  In this case, **A+C** is the answer.

## Requirement
Nothing special

## Usage
First, place **QM.py** in the same directory as the file in which 
you want to use this function (let's say **driver.py**).  
Or, you can make **QM.py** be your own module.  
In **driver.py**,
- import QM.py `import QM`
- call QM function `ans = QM.QM(dnf)`
- then, `ans` is the simplest DNF 

## Confirmed Environment
OS: macOS Sierra 10.12.5  
Python: 3.6.3
