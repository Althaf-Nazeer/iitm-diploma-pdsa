#Write a function del char(s,c) that takes strings s and c as input, where c has length 1 (i.e., a single character), and returns the string obtained by deleting all occurrences of c in s. If c has length other than 1, the function should return s



def del_char(s, c):
    if len(c) != 1:
        return s

    result = ""
    for char in s:
        if char != c:
            result += char

    return result

s = input()
c = input()
print(del_char(s,c))
