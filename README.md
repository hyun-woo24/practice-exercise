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


## 클래스 활용

class Student:
    
    def __init__(self, kor, eng, math):
        self.kor = kor
        self.eng = eng
        self.math = math
        
    def average(self):
        #학생의 평균점수 계산
        return (self.kor+self.eng+self.math)/3
        
#사용자로부터 학생 수를 받음           
num=int(input('학생 수 입력 (N): '))

#입력한 학생 수만큼 반복
for i in range(1,num+1):
    #사용자로부터 받은 국어, 영어, 수학 점수를 각 변수에 저장
    kor = int(input(f'{i}번째 학생의 국어 성적 입력: '))
    eng = int(input(f'{i}번째 학생의 영어 성적 입력: '))
    math = int(input(f'{i}번째 학생의 수학 성적 입력: '))
    
    studentScore = Student(kor, eng, math)
    
    #학생의 평균점수 출력
    print(f'{i}번째 학생의 평균 점수: {studentScore.average()}')
    
    
    
