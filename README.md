# python41
permutation recursion
def permute(s,bucket=''):
    if not s:
        print(bucket)
        return
    for i in range(len(s)):
        ns=s[:i]+s[i+1:]
        permute(ns,bucket+s[i])
text=input("Enter a name/word:")
print("Possibilities of combinations......")
permute(text)
