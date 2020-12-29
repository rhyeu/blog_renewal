---
title: Today I Learn - python tip
author: 류성균
date: '2020-12-29'
slug: today-i-learn-python-tip
categories:
  - Today I learn
tags:
  - python
  - os
keywords:
  - tech
---

<!--more-->

```{r}
library(reticulate)
```

# 폴더 내에 있는 여러 파일 한꺼번에 읽기

- reference : https://stackoverflow.com/questions/20906474/import-multiple-csv-files-into-pandas-and-concatenate-into-one-dataframe
```
 path = r'/gdrive/My Drive/Dacon/Sunpower/data/test' # use your path
 all_files = glob.glob(path + "/*.csv")

 li = []

 for filename in all_files:
     df = pd.read_csv(filename, index_col=None, header=0)
     li.append(df)

test = pd.concat(li, axis=0, ignore_index=True)
```

# google sheet로 데이터 쓰기
```
!pip install --upgrade gspread

# Import Drive API and authenticate.
from google.colab import drive
 
# Mount your Drive to the Colab VM.
drive.mount('/gdrive', force_remount=True)
 
# Write the DataFrame to CSV file.
 with open('/gdrive/My Drive/Dacon/Sunpower/sub_1228_baseline.csv', 'w') as f:
   sub.to_csv(f)
```