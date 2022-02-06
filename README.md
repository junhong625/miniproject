# 강수량과 교통사고의 연관성

## 개요

> '**날씨가 좋은 날**'과 '**좋지 않은 날**' 중 어떤 날에 교통사고가 더 많이 일어날까요?   
> 본 프로젝트는 이러한 사소한 궁금증으로부터 시작하여   
> '**과연 비, 눈이 내리는 날에 교통사고가 더 많이 일어날까?**'라는 주제를 선정하여 시작했습니다.

## 데이터 수집

> 교통사고 : [[TAAS(교통사고분석시스템)](http://taas.koroad.or.kr/sta/acs/exs/typical.do?menuId=WEB_KMP_OVT_UAS_PDS#)]에서 데이터 수집   
> 강수량 : [[기상청 기상자료개방포털](https://data.kma.go.kr/climate/RankState/selectRankStatisticsDivisionList.do?pgmNo=179)]에서 데이터 수집


<p align="left">
<img src="https://user-images.githubusercontent.com/83000975/151673753-a66fb1a9-53d2-4fe7-8123-d4231bbbf76f.png" weight=120 height=40>
</p>

#### - TAAS(교통사고분석시스템)
```
데이터 일자 : 2016-01-01 ~ 2020-12-31   
파일명 : 2016.xls ~ 2020.xls   
용량 : 150KB   
사용 columns : [날짜, 사고건수, 사망자수, 부상자수]
```

<p align="left">
<img src="https://user-images.githubusercontent.com/83000975/151673800-c6ce0b2f-4c04-4092-aac2-a006dab3c508.png" weight=120 height=40>
</p>

#### - 기상청 기상자료개방포털
```
데이터 일자 : 2016-01-01 ~ 2020-12-31   
파일명 : 강수량.csv   
용량 : 50KB   
사용 columns : [일시, 강수량(mm)]
```

## 사용 툴&기술
```
툴 : Jupyter Notebook
기술 : Csv, Pandas, Matplotlib, Numpy, Platform
```

## 결과
- **<강수량에 따른 평균 교통사고 수> 그래프**
<p align="left">
<img src="https://user-images.githubusercontent.com/83000975/151675386-9968d6ae-822b-41d6-bc4e-7fe1dbf74a94.jpg" weight=700 height=700>
</p>

- **<평균 사망자 수> 확대 그래프**
<p align="left">
<img src="https://user-images.githubusercontent.com/83000975/151675399-b629d444-40c7-4841-9e16-649769c2a874.png" weight=700 height=700>
</p>

> 예상했던 대로 비, 눈이 오는 날이 맑은 날보다 교통사고가 더 많이 발생했다는 것을 확인할 수 있었습니다.   
> 하지만 예상외로 평균 사망자 수에서 강수량이 가장 많은 날에 평균 사망자 수가 제일 적은 것으로 나타났습니다.   
> 아마도 비나 눈이 많이 오는 날에는 평소보다 더욱 안전운전을 하거나 대중교통을 이용하는 사람들이 많기 때문으로 보입니다.

## 결론
생각지도 못했던 결과를 발견할 수 있었고 유의미한 결과물을 얻어낸 좋은 시도였던 것 같습니다.   
그리고 그래프가 보여주듯이 **비가 오거나 눈이 오는 날에는 평소보다 사고 일어날 확률이 더 높으니 꼭 안전운전 하십시오!**
