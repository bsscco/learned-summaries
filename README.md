# codecademy-learn-ruby
Learn Ruby course is one of Codecademy courses. summarized this course's content.


- 데이터 타입
    - number, boolean, string

- 변수
    - my_num = 25

- 수학 연산자
    - +, -, *, **, /, %

- 출력
    - print
    - puts # add new line

- 객체
    - 모든 것이 객체

- 주석
    - # comment
    - =begin
        - comment

    - =end

- 네이밍 컨벤션
    - 변수 snake_case

- 입력
    - gets
    - gets.chomp

- 문자열 interpolation
    - "I took #{monkey} to the zoo"
    - ''로 감싸는 건 인식 못함.

- 메소드!
    - name = 'bsscco'.capitalize # name = 'bsscco'
    - name = 'bsscco'.capitalize! # name = 'Bsscco'

- 메소드?
    - boolean 반환

- 문자열 메소드
    - capitalize
    - upcase
    - downcase
    - chomp
    - gsub

- 흐름 제어 : 분기
    - if문
        - if n &gt; 0
            - puts  'positive' # 들여쓰기 안 해도 잘 돌아감.

        - elsif n &lt; 0
            - puts  'negative'

        - else
            - puts 'zero'

        - end

    - unless문
        - unless n &gt; 0
            - puts 'zero or negative'

        - end

    - if, unless문은 식(expression)이라서 값이 될 수 있다.
    - case문
        - case lang
            - when 'ko'
                - puts 'ko'

            - when 'en'
                - puts 'en'

            - else
                - puts 'error'

        - end

- 흐름 제어 : 반복
    - while문
        - i = 0
        - while i &lt; 10
            - print i
            - i += 1

        - end

    - until문
        - i = 0
        - until i &gt;= 10
            - puts i
            - i += 1

        - end

    - for문
        - for i in 1...10
            - puts i

        - end

    - loop 메소드
        - loop { print 'hh' }
        - loop do 
            - print 'hh' 

        - end
        - do 키워드는 curly braces {}를 대체한다.
        - break if
        - next if

- 범위
    - 1...5 # 1,2,3,4
    - 1..5 # 1,2,3,4,5

- 배열
    - arr = [1,2,3,4,5]
    - arr.each do |x| 
        - puts x

    - end
    - arr.each {|x| puts x }
    - arr.push 1
    - arr &lt;&lt; 1

- 반복 정리
    - while, until
    - for, loop, times
    - 10.times do 
        - puts 'hh' 

    - end
    - 'A'.upto 'Z' do |c| puts c end
    - 10.downto 1 do |n| puts n end

- 해시
    - hash = Hash.new
    - hash = {}
    - hash = {1 =&gt; 1, '2' =&gt; 2} # =&gt;을 해시로켓이라 부름.
    - hash['n1'] = 1
    - hash.each do |k, v| puts "#{k}, #{v}" end
    - hash = Hash.new('no value')
    - puts hash['no key'] # 'no value'
    - hash.delete 'key'
    - 루비1.9부터 심볼을 해시키로 사용할 땐 :sym =&gt; 1 형태에서 sym: 1 형태로 써도 된다.
    - filtered = hash.select do |v, k| k &gt; 3 end
    - hash.each_key do
    - hash.each_value do

- 메소드
    - def func
        - puts 'f'

    - end
    - def func(greeting, *friends) 
        - friends.each do |friend|
            - puts greeting + ' ' + friend

        - end

    - end
    - def add(a, b)
        - a + b

    - end
    - 블록은 이름없는 메소드다.
        - 1.times { puts 'As am I' }

    - def func(d = false) # 디폴트 파라메터

- 결합 비교 연산자
    - title1 &lt;=&gt; title2

- nil
    - nil은 false와 다르다.

- 심볼
    - 심볼은 string과 다르다.
    - "s".object_id == "s".object_id # false
    - :s == :s # true
    - 심볼을 해시 키로 쓰는 이유
        - 메모리 절약
        - 접근 속도가 빠르다.

- 형변환
    - 5.to_s
    - '1'.to_i
    - 's'.to_sym
    - 's'.intern
    - :sym.to_s

- 단순한 if, unless
    - puts "it's true" if true
    - puts "it's false" unless false

- 삼항 연산자
    - true ? 'TRUE' : 'FALSE'

- 조건 할당 연산자
    - puts nil || 'str' # 'str'
        - v = nil 
        - v ||= 'str' # 'str

    - puts nil && 'str' # ''
        - v = nil 
        - v &&= 'str' # nil

- 메소드 존재 확인
    - 4.respond_to? :next # true

- 연결 연산자
    - arr.push 1 # arr &lt;&lt; 1
    - 'a' &lt;&lt; 'b' # 'ab'

- 자료형 확인
    - 1.is_a? Integer
