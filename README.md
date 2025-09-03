class Solution:
    def ispower(self, n):
        if n <= 0:
            return False
        if n == 1:
            return True
        if n % 2 != 0:
            return False
        return self.ispower(n // 2)

b = int(input("Enter the value of b: "))
a = Solution()
print(a.ispower(b))
