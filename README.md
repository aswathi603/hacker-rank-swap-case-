# hacker-rank-swap-case-

You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.

    Www.HackerRank.com → wWW.hACKERrANK.COM
    Pythonist 2 → pYTHONIST 2

Input format:

    A single line containing a string S.

Constraints:

    0 < len(S) <= 1000

Output format:

    Print the modified string S.

Sample input 0:

    HackerRank.com presents "Pythonist 2".

Sample output 0:

    hACKERrANK.COM PRESENTS "pYTHONIST 2".

SOLUTION 1

def swap_case(s):

      swap =''
      for char in s:
        if char.upper()!=char:
            swap+=char.upper()
        elif char.lower()!= char:
            swap+=char.lower()
        else:
            swap+=char
    return swap

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)


SOLUTION 2

def swap_case(s):

    return s.swapcase()
    

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
