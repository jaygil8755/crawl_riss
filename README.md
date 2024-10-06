# crawl_riss
riss 학술연구정보서비스에서 논문을 자동으로 수집하는 코드입니다.   
키워드를 입력하면 학술논문과 학위논문을 엑셀파일과 csv파일로 자동 저장합니다.  
This package provides functionalities to crawl academic papers from RISS using two different methods (HS and HW).

## Installation

You can install this package via pip:

```bash
pip install crawl_riss

from crawl_riss import crawl_hs, crawl_hw
crawl_hs.crawl_papers_hs("생성형 AI")

전체 검색된 논문 수: 1079개
수집할 논문 수: 1000개
CSV 파일이 /content/생성형_AI_학술논문/생성형_AI_학술논문.csv에 저장되었습니다.
Excel 파일이 /content/생성형_AI_학술논문/생성형_AI_학술논문.xlsx에 저장되었습니다.

crawl_hw.crawl_papers_hw("생성형 AI")
전체 검색된 논문 수: 374개
수집할 논문 수: 374개
CSV 파일이 /content/생성형_AI_학위논문/생성형_AI_학위논문.csv에 저장되었습니다.
Excel 파일이 /content/생성형_AI_학위논문/생성형_AI_학위논문.xlsx에 저장되었습니다.
