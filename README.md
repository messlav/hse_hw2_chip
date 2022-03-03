# hse_hw2_chip

Link to colab https://colab.research.google.com/drive/1AZk_gHZ4z72G-jK_QN-V5yyJ_14xNlGl?usp=sharing

Я выбрал клеточную линия - A549, гистоновую клетка - H3K27me3

 ## FastQC outputs
 
 **Analize for ChIP-seq ENCFF000AKV**
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.50.31.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.50.42.png)
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.50.53.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.52.36.png)
 
**Then I tried to trim it, but without that it was ok**

**Analize for ChIP-seq trimmed ENCFF000AKV**
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.51.17.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.51.23.png)
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.51.28.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.51.40.png)
 
 **Analize for ChIP-seq ENCFF000AKW**
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.52.43.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.52.49.png)
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.52.54.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.02.png)
 
 **And again I tried to trim it, although that was ok**
 
  **Analize for ChIP-seq trimmed ENCFF000AKW**
  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.07.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.12.png)
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.18.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.26.png)
 
 And after this all, control file without trimming - ENCFF000AHJ
   ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.32.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.36.png)
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.42.png)  ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2015.53.49.png)
 
 ##Table with statistic for all 3 samples**
 ![alt text](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2017.26.42.png)
 
 **Почему процент выравниваний получился именно таким?**
 Процент выравнивания получился достаточно низким, т.к. выравнивание происходило всего на одну хромосому, которая состовляет лишь малую часть генома.
 
 ## Venn diagram
 
**For ENCFF000AKW sample**
Number of sections from the file ENCFF000AKW that intersect with the file ENCFF130IOE             |  Number of sections from the file ENCFF130IOE that intersect with the file ENCFF000AKW
:-------------------------:|:-------------------------:
![](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2017.41.03.png)  |  ![](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2017.41.15.png)


** For ENCFF000AKV sample**
Number of sections from the file ENCFF000AKV that intersect with the file ENCFF130IOE              |  Number of sections from the file ENCFF130IOE that intersect with the file ENCFF000AKV
:-------------------------:|:-------------------------:
![](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2017.41.28.png)  |  ![](https://github.com/messlav/hse_hw2_chip/blob/main/imgs/Снимок%20экрана%202022-03-03%20в%2017.41.42.png)

**Проанализируйте полученные результаты. Как можно объяснить различия в количестве пересечений?**

Так как изначально у нас было выравнивание лишь на одну хромосому, поэтому и количество пиков весьма небольшое. Из-за этого и пересекающихся участков тоже немного. Пересечения же не совпадают из-за того что мы по-разному их определяем: вначале одно на другое, а затем наоборот.

 
