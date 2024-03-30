# practice-exercise
연습문제


# 코드 추가

a = int(input('a: '))
b = int(input('b: '))
X = int(input('Max: '))

def problem(num1, num2, num3):
    for i in range(0, num3+1):
        print(f'{num1}x{num1}x{i} + {num2} = {num1*num1*i+num2}')
        
         
problem(a,b,X)
