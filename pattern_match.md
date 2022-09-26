# Match a pattern without regex
<hr>

## Inputs
### given string - can use input() for user test cases
### pattern to be found - can use input for user test cases

## Outputs
### Number of times pattern was found

# solutions

# Python

given_string = input()
pattern = input()
counter = 0
for i in range(len(given_string)-len(pattern)+1):
    dummy = ""
    for j in range(len(pattern)):
        dummy+=given_string[i+j]
    if dummy==pattern:
        counter+=1
print(pattern, " found ", counter, "time(s)")
