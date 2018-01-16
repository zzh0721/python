# 求素数
def is_prime(x):
    if x < 2:
        return False
    else:
        for n in range(2, x-1):
            if x % n == 0:
                return False
        return True
        
        
# 转置文本
def reverse(text):
  word = ""
  l = len(text) - 1
  while l > 0:
    word = word + text[l]
    l -= 1


# 去掉元音字母
def anti_vowel(text):
  c = ""
  for i in text:
    for j in "aeiouAEIOU":
      if i == j:
        i = ""
    c += i
  return c
  
  
# 制定字符替换为*
# 不懂
def censor(text, word):
    words = text.split()
    result = ''
    stars = '*' * len(word)
    count = 0
    for i in words:
        if i == word:
            words[count] = stars
        count += 1
    result =' '.join(words)

    return result



# -*- coding:utf-8 -*-  
  
""" 
功能：python跳出循环 
"""  
# 方法2：for...else...用法，用于跳出指定循环层  
  
for i in range(5):  
    for j in range(5):  
        for k in range(5):  
            if i == j == k == 3:  
                break  
            else:      
                print i, '----', j, '----', k  
        else:        # else1  
            continue  
        break        # break1  
    else:            # else2  
        continue  
    break            # break2  

方法3解释：
（1）break能跳出某一重循环（该重循环的本次及剩余次数都不再执行），但并不能跳出该重循环的其他外重循环。

例如，最内第3重循环break之后，程序返回第2重循环继续执行第2重的下一次，然后第3重循环将再次执行。

（2）continue是跳过某一重循环的某一次，但该重循环的剩余次数会继续执行。

（3）for...else：其中else块中的语句将在for循环完整执行过之后才会被执行，如果for循环被break，则else块将不会被执行。

（4）方法3中，当第3重循环满足i == j == k ==3时，第3重循环被break，则并列的else1将跳过，执行break1，导致第2重循环

被终止，则else2被跳过，执行break2，导致第1重循环被终止。

最终实现跳出整个循环。
