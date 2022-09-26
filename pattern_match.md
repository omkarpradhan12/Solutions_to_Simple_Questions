# Match a pattern without regex
# solutions
# Python

## given string - can use input() for user test cases
given_string = "aabbabaab" 

## pattern to be found - can use input for user test cases
pattern = "ab" 

## counter initialized with 0
counter = 0

for i in range(len(given_string)-len(pattern)+1):
    dummy = ""
    for j in range(len(pattern)):
        dummy+=given_string[i+j]
    if dummy==pattern:
        counter+=1
print(pattern, " found ", counter, "time(s)")
