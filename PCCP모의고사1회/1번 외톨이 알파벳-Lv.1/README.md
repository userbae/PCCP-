## 1번 외톨이 알파벳
[문제 링크](https://school.programmers.co.kr/learn/courses/15008/lessons/121683)


<details>
  <summary>
    힌트
  </summary> 
  
</details>

<details>
  <summary>
    정답
  </summary> 
    
  
    function solution(input_string) {
      let answer = new Set();
      const set = new Set();
      const str = input_string.replace(/([a-z])\1{1,}/g,"$1");
  
      for (const s of str){
          if (set.has(s)) answer.add(s);
          else set.add(s);
      }
  
      return answer.size ? Array.from(answer).sort().join("") : "N";
    }
   

<details>
  <summary>
    해석
  </summary> 
  
</details>
</details>
