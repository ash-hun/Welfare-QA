<img width="848" alt="image" src="https://github.com/ash-hun/Welfare-QA/assets/32566767/f6c6a955-9e83-45f2-9446-1c641f53a430">

# Dataset Card for Welfare-QA

## Description

대한민국 보건복지부에서 발간하였으며 2023년 5월 11일에 [복지로](https://www.bokjiro.go.kr/ssis-tbu/index.do)에 등록된 안내책자를 바탕으로 만들어졌습니다.
총 413페이지의 비정형 PDF에 담긴 약 460여개의 복지제도에 대한 Question-Answering-Documents 데이터셋입니다.
원본은 다음 링크에서 확인해보실 수 있습니다. [👉 '2023 나에게 힘이되는 복지서비스 PDF 책자'](https://www.bokjiro.go.kr/ssis-tbu/twatxa/wlfarePr/selectWlfareSubMain.do?dmMnuParam=column27)

## Project Repo

- Github Repo : [Ask-for-Welfare](https://github.com/ssisOneTeam/Ask-for-Welfare)

## How to Uses

```python
>>> from datasets import load_dataset
>>> dataset = load_dataset("Ash-Hun/Welfare-QA", split='train')
>>> dataset
Dataset({
    features: ['Question', 'Answer', 'Documents'],
    num_rows: 9547
})
```

```python
>>> dataset[0]
{'Question': 'LPG 사용 가정의 고무호스를 교체하려면 어떤 지원을 받을 수 있나요?',
 'Answer': 'LPG용기 사용가구 시설개선 사업을 통해 LPG 고무호스를 금속배관으로 교체하는 데 필요한 지원을 받으실 수 있습니다.',
 'Documents': 'LPG용기 사용가구 시설개선'}
```
