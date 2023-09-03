#!/usr/bin/python3

import sys


def factors(nums):
    for num in range(2, nums):
        if nums % num == 0:
            return num, nums // num
    return None, None

def main(fn):
    with open(fn, 'r') as file:
        for line in file:
            nums = int(line.strip())
            x, y = factors(nums)
            if x and y:
                print(f"{nums}={x}*{y}")

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: factors <file>")
    else:
        fn = sys.argv[1]
        main(fn)
