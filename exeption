
#!/usr/bin/python3
# Author: Tatyana Polyakova

# person is class that has string representation as name, age and so on

person = {}

properties = [
    ("name", str),
    ("last name", str),
    ("age", int),
    ("height", float),
    ("weight", float),
]

# this use test with exception handling where string represent binary

for property, p_type in properties:
    valid_value = None

    while valid_value is None:
        try:
            value = input("Please enter your %s: " % property)
            valid_value = p_type(value)
        except ValueError as ve:
            print(ve)

    person[property] = valid_value


binary = []
def strBin(s_str):
        for s in s_str:
            if s == ' ':
                binary.append('00100000')
            else:
                binary.append(bin(ord(s)))
s_str = input("String: ")
strBin(s_str)

b_str = '\n'.join(str(b_str) for b_str in binary) # print as type str
# replace '\n' to '' to output in one line without spaces, ' ' if with spaces

print(b_str.replace('b',''))
