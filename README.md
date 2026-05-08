# 발주량 산정 시스템

가구/목제 상품의 최적 발주량을 자동으로 계산하는 Streamlit 웹앱입니다.

## 기능

- 수요예측 파일 + CPP 리스트 업로드
- 3개월치 발주량 자동 계산 (CPP 단위 반올림 적용)
- 발주량 결과 Excel 다운로드 (통합/월별/공급처별/발주서 시트)
- 공급처별 발주서 조회
- 긴급/발주필요/여유 상태 자동 분류

## 필요 파일

| 파일 | 필수 시트/컬럼 |
|------|--------------|
| 수요예측.xlsx | `품목별상세` 시트 |
| grd_list.xls | 단품코드, 단품컬러, 적재단위(CPP) |

## 로컬 실행

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Streamlit Cloud 배포

1. 이 저장소를 GitHub에 업로드
2. [share.streamlit.io](https://share.streamlit.io) 접속
3. GitHub 저장소 연결 → `app.py` 선택 → Deploy
