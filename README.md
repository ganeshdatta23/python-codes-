# README: 100 Important Python Codes for Interviews

# 1. Swap two variables without using a third variable
x, y = 5, 10
y, x = x, y

# 2. Reverse a string
def reverse_string(s):
    return s[::-1]

# 3. Check if a string is palindrome
def is_palindrome(s):
    return s == s[::-1]

# 4. Find factorial using recursion
def factorial(n):
    return 1 if n == 0 else n * factorial(n - 1)

# 5. Fibonacci series using recursion
def fibonacci(n):
    return n if n <= 1 else fibonacci(n-1) + fibonacci(n-2)

# 6. Check if a number is prime
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

# 7. Find GCD of two numbers
def gcd(a, b):
    return a if b == 0 else gcd(b, a % b)

# 8. Find LCM of two numbers
def lcm(a, b):
    return (a * b) // gcd(a, b)

# 9. Check if a year is leap year
def is_leap_year(year):
    return (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0)

# 10. Reverse a number
def reverse_number(n):
    return int(str(n)[::-1])

# 11. Find largest element in a list
def find_max(lst):
    return max(lst)

# 12. Find smallest element in a list
def find_min(lst):
    return min(lst)

# 13. Sum of digits of a number
def sum_of_digits(n):
    return sum(int(digit) for digit in str(n))

# 14. Find duplicate elements in a list
def find_duplicates(lst):
    return list(set([x for x in lst if lst.count(x) > 1]))

# 15. Count occurrences of elements in a list
def count_occurrences(lst):
    from collections import Counter
    return Counter(lst)

# 16. Merge two sorted lists
def merge_sorted_lists(lst1, lst2):
    return sorted(lst1 + lst2)

# 17. Find second largest element in a list
def second_largest(lst):
    return sorted(set(lst))[-2]

# 18. Remove duplicates from a list
def remove_duplicates(lst):
    return list(set(lst))

# 19. Check if two strings are anagrams
def are_anagrams(s1, s2):
    return sorted(s1) == sorted(s2)

# 20. Find common elements in two lists
def common_elements(lst1, lst2):
    return list(set(lst1) & set(lst2))

