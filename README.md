# Korean-Embedding-Model-Performance-Benchmark-for-Retriever
Korean Sentence Embedding Model Performance Benchmark for RAG System

## Ⅰ. 개요
#### 1. 실험목표
  > 한국어 임베딩 모델과 하이퍼파라미터 조정에 따른 Retriever 성능비교
#### 2. 실험배경

  **1. 한국어, 특히 복지 도메인에 기반한 Embedding Model의 필요성**
  
  **2. 이전 진행 사항**
  
    2-1. 이전에 사용한 Base Korean Embedding Model: KoSimCSE-RoBERTa-multitask
        - 한국어 Embedding Model 중 AVG Score가 가장 높은 Model 사용
    
    2-2. Tokenizer Vocab 추가 및 Embedding Model Domain Adaptation 진행
        - Retriever 결과의 미흡함 확인
        - 더 나은 성과를 위해 추가적인 실험과 비교 분석 필요
        
  **3. 연구 목적**
  
    - 실험을 통한 Korean Embedding Model 선정과 하이퍼 파리미터 조정함으로써 개선된 성능 도출

#### 3. 실험환경
    pip install -r requirement.txt
       
## Ⅱ. 가정
  위 배경에 의거하여 한국어 문장 임베딩 모델과 그에따른 하이퍼파라미터를 조정함으로써 관련된 문서가 잘 도출되는 성능에 직결될 것이라 생각하였다. 즉, Korean Sentence Embedding Model선정과 해당모델에 대한 Hyper Parameter 조합에 따라 가장 Retriever 결과가 가장 잘 나오는 조합과 모델을 선정한다. 즉, 아래와 같은 2가지 방법을 바탕으로 성능비교를 진행하고자 한다.
     

## Ⅲ. 방법

  **1. 고성능의 Retriever 결과도출을 위한 다양한 한국어 문장 임베딩 모델들에 대한 성능비교 (HitRate)**
  
    1-1. 다양한 한국어 문장 임베딩 모델 리스트업
      - 모델 선정이유/근거
      - 평가지표 선정이유/근거
    
    1-2. Retriever 성능평가 진행
      - 성능평가 방식 선정
      - 성능평가 진행

    1-3. 기존 모델(=KoSimCSE-RoBERTa-multitask)과의 Performance Benchmarking 진행
      
  **2. 가장 높은 성능을 가지는 모델에 대하여 하이퍼파라미터 조정 진행**
  
    2-1. 하이퍼파라미터 선정
    
    2-2. 하이퍼파라미터 튜닝후 성능평가 진행
      - 성능평가 방식 선정 (전수조사, GridsearchCV, etc… )
      - 성능평가 진행  
      
    2-3. 하이퍼파라미터 튜닝 전/후 Performance Benchmarking 진행

## Ⅳ. 실험결과 (※ 전/후 결과비교가 중요)
  1. Embedding Model 비교/선정  
  2. Retreiver 성능측정  
    1. Embedding Model 교체 전/후 Retriever 성능비교  
    2. BM25, Re-Rank, Filtering 적용 전/후 Retriever 성능비교  
  3. 최종 실험결과 도출  

## Ⅴ. 컨트리뷰터

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/PangPangGod">
        <img src="https://github.com/PangPangGod.png" width="100px;" alt="송준호"/><br />
        <sub><b>송준호</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/ash-hun">
        <img src="https://github.com/ash-hun.png" width="100px;" alt="최재훈"/><br />
        <sub><b>최재훈</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/MoonHeesun">
        <img src="https://github.com/MoonHeesun.png" width="100px;" alt="문희선"/><br />
        <sub><b>문희선</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Noveled">
        <img src="https://github.com/Noveled.png" width="100px;" alt="김민식"/><br />
        <sub><b>김민식</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/myeongjun1007">
        <img src="https://github.com/myeongjun1007.png" width="100px;" alt="현명준"/><br />
        <sub><b>현명준</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/kha-jaejun">
        <img src="https://github.com/kha-jaejun.png" width="100px;" alt="가재준"/><br />
        <sub><b>가재준</b></sub>
      </a>
    </td>
  </tr>
</table>

### Ⅵ. 참고자료
  1. 참조한 자료 목록
