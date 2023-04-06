# hse_hw3_chromhmm

Сидорова Татьяна, Группа 2

PC-3 отсутствует в таблице, поэтому была выбрана клеточная линия HUVEC.

[Ccылка на Колаб](https://colab.research.google.com/drive/16GbxuCDYd4vhIfXNgENQOk7901rMPsbY#scrollTo=8KwrEmUd95zC)

## Гистоновые метки

|Гистоновая метка  |     Файл    |
|:----------------:|:-----------:|
|H2az|wgEncodeBroadHistone/wgEncodeBroadHistoneHuvecH2azAlnRep1.bam|
|H3k27ac|wgEncodeBroadHistoneHuvecH3k27acStdAlnRep2.bam|
|H3k27me3|wgEncodeBroadHistoneHuvecH3k27me3StdAlnRep2.bam|
|H3K4me1|wgEncodeBroadHistoneHuvecH3k4me1StdAlnRep2.bam|
|H3K4me2|wgEncodeBroadHistoneHuvecH3k4me2StdAlnRep1.bam|
|H3K4me3|wgEncodeBroadHistoneHuvecH3k4me3StdAlnRep1.bam|
|H3K79me2|wgEncodeBroadHistoneHuvecH3k79me2AlnRep1.bam|
|H3K9ac|wgEncodeBroadHistoneHuvecH3k9acStdAlnRep1.bam|
|H3K9me1|wgEncodeBroadHistoneHuvecH3k9me1StdAlnRep1.bam|
|H4K20me1|wgEncodeBroadHistoneHuvecH4k20me1StdAlnRep1.bam|

## cellmarkfiletable.txt

|Клеточная линия|Гистоноввая метка|Файл с гистоновой меткой|Файл контроля|
|:--------------:|:--------------:|:--------------:|:--------------:|
|HUVEC|H2az|H2az.bam |Control.bam|
|HUVEC|H3k27ac|H3k27ac.bam|Control.bam|
|HUVEC|H3k27me3|H3k27me3.bam|Control.bam|
|HUVEC|H3K4me1|H3K4me1.bam|Control.bam|
|HUVEC|H3K4me2|H3K4me2.bam|Control.bam|
|HUVEC|H3K4me3|H3K4me3.bam|Control.bam|
|HUVEC|H3K79me2|H3K79me2.bam|Control.bam|
|HUVEC|H3K9ac|H3K9ac.bam|Control.bam|
|HUVEC|H3K9me1|H3K9me1.bam|Control.bam|
|HUVEC|H4K20me1|H4K20me1.bam|Control.bam|

## ChromHMM

|Emission|Overlap|Transition|
|:-------:|:-----:|:-------:|
|![image](https://user-images.githubusercontent.com/114301236/230487721-ea343a2c-cefe-4b71-ac62-fde2b5518334.png)|![image](https://user-images.githubusercontent.com/114301236/230487539-f3273970-ad42-4c8b-850a-f4bad598cdc3.png)|![image](https://user-images.githubusercontent.com/114301236/230487651-de82d799-3b06-465a-8b78-a2591c6a8612.png)|

|RefSeqTSS|RefSeqTES|
|:-------:|:-------:|
|![image](https://user-images.githubusercontent.com/114301236/230488064-dca7607b-ccdd-41c5-ae91-62b7fa02db99.png)|![image](https://user-images.githubusercontent.com/114301236/230488111-42aae66f-0451-473c-9f66-2a6d3a6473ba.png)|

## Эпигенетические типы

|Название|Описание|UCSC browser|
|:-------:|:-------:|:-------:|
|Weak Promoter|Метка H2AZ; расположен в CpG-островках, TSS, экзонах|![image](https://user-images.githubusercontent.com/114301236/230495981-71a1e5f0-dad5-4f17-930c-b425e8e98d83.png)|
|Inactive Promoter| Выраженв H2AZ, H3K4me2. Мало выражен в TSS и TES, в экзонах|![image](https://user-images.githubusercontent.com/114301236/230496462-c43f06df-7601-4cd0-a1e9-2b91505beb4d.png)|
|Heterochromatin|Выражен в ядерной ламине. В метках не выражен|![image](https://user-images.githubusercontent.com/114301236/230497014-980b08ee-aa2f-499f-92d3-a79072385bbe.png)|
|Polycomb-repressed|Выражен в ядерной ламине|![image](https://user-images.githubusercontent.com/114301236/230497222-f41bd23e-2eeb-4ac5-be26-e66f81a3effe.png)|
|Weak Enhancer (5)|Метка - H3K4me1. Проявляется в ядерной ламине и TES|![image](https://user-images.githubusercontent.com/114301236/230499354-1ce8a868-3e8f-4d60-bf37-acd88f1a16c9.png)|
|Weak Enhancer (6)|Метки: H3K4me1 и HeK79me2|![image](https://user-images.githubusercontent.com/114301236/230499163-d30bb01d-eb2e-4fd1-9b4c-8eaad0eaa1bd.png)|
|Active Promoter|Метки: H2AZ, H3K4me3, H3K4me1, H3K4me2, H3K79me2, H3K9ac, H3K27ac. Расположен в CpG-островках, TSS, TES экзонах |![image](https://user-images.githubusercontent.com/114301236/230499605-d0b663bd-02d1-4219-bf53-96b503331827.png)|
|Strong Enhancer|Метки: H2AZ, H3K27ac, H3K4me1, H3K4me2, H3K9ac. Расположен в ядерной ламине и TES|![image](https://user-images.githubusercontent.com/114301236/230499994-9dca68f6-07ad-4ed5-8dfd-7a40ea048f93.png)|
|Txn elongation|Меток нет. Располагается в генах, экзонах, TES|![image](https://user-images.githubusercontent.com/114301236/230500283-c9424ae3-9f23-4e67-8498-6fb3e7e9ef5f.png)|
|Weak Txn|Метка - H3K79me2. Расположен в генах.|![image](https://user-images.githubusercontent.com/114301236/230500457-6b4305f4-3409-412d-b514-f25dc36c2608.png)|

