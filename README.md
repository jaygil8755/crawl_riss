# crawl_riss
- RISS 학술연구정보서비스에서 논문을 자동으로 수집하는 라이브러리입니다.  
- 키워드를 입력하면 학술논문과 학위논문을 엑셀 파일과 CSV 파일로 자동 저장합니다.  
- 검색 결과가 1,000개가 넘으면 최대 1,000개만 수집하고, 키워드 뒤에 수집할 숫자를 지정할 수 있습니다.
- riss.kr 사이트가 바뀌면 코드가 작동안될 수도 있습니다.^^ 안되면 제 이메일(jaygil87555@gmail.com)으로 연락주세요.
- This package provides functionalities to crawl academic papers from RISS using two different methods (HS and HW).

## Installation

You can install this package via pip:

```bash
pip install crawl_riss
from crawl_riss import crawl_hs, crawl_hw```

# 학술 논문 수집
`crawl_hs.crawl_papers_hs("생성형 AI")`

# 실행 결과:
# 전체 검색된 논문 수: 1079개
# 수집할 논문 수: 1000개
# CSV 파일이 /content/생성형_AI_학술논문/생성형_AI_학술논문.csv에 저장되었습니다.
# Excel 파일이 /content/생성형_AI_학술논문/생성형_AI_학술논문.xlsx에 저장되었습니다.

# 학위 논문 수집
`crawl_hw.crawl_papers_hw("생성형 AI")`
# 실행 결과:
# 전체 검색된 논문 수: 374개
# 수집할 논문 수: 374개
# CSV 파일이 /content/생성형_AI_학위논문/생성형_AI_학위논문.csv에 저장되었습니다.
# Excel 파일이 /content/생성형_AI_학위논문/생성형_AI_학위논문.xlsx에 저장되었습니다.

# 학술 논문 수집 - 수집할 수 지정
`crawl_hw.crawl_papers_hw("딥러닝", 11)`
# 전체 검색된 논문 수: 8304개
# 수집할 논문 수: 11개
# CSV 파일이 /content/딥러닝_학위논문/딥러닝_학위논문.csv에 저장되었습니다.
# Excel 파일이 /content/딥러닝_학위논문/딥러닝_학위논문.xlsx에 저장되었습니다.


