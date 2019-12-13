# PCA_matlab

## sample data
| 学生编号 | 语文 | 数学| 物理 | 化学 | 英语 | 历史 |
| --- | --- | --- | --- | --- | --- | --- |
| 1	| 84 | 65 | 61 | 72 | 79 | 81 |
| 2	| 64 | 77 | 77 | 76 | 55 | 70 |
| 3	| 65 | 67 | 63 | 49 | 57 | 67 |
| 4	| 74 | 80 | 69 | 75 | 63 | 74 |
| 5	| 84 | 74 | 70 | 80 | 74 | 82 |

sample =
| 84 | 65 | 61 | 72 | 79 | 81 |
|----|----|----|----|----|----|
| 64 | 77 | 77 | 76 | 55 | 70 |
| 65 | 67 | 63 | 49 | 57 | 67 |
| 74 | 80 | 69 | 75 | 63 | 74 |
| 84 | 74 | 70 | 80 | 74 | 82 |


sampleSize =

     5


dimSize =

     6


meanOfEachDim =
| 74.2000 | 72.6000 | 68.0000 | 70.4000 | 65.6000 | 74.8000 |
|---------|---------|---------|---------|---------|---------|


centeredData =
| 9.8000   | -7.6000 | -7.0000 | 1.6000   | 13.4000  | 6.2000  |
|----------|---------|---------|----------|----------|---------|
| -10.2000 | 4.4000  | 9.0000  | 5.6000   | -10.6000 | -4.8000 |
| -9.2000  | -5.6000 | -5.0000 | -21.4000 | -8.6000  | -7.8000 |
| -0.2000  | 7.4000  | 1.0000  | 4.6000   | -2.6000  | -0.8000 |
| 9.8000   | 1.4000  | 2.0000  | 9.6000   | 8.4000   | 7.2000  |


C3 =
| 95.2000  | -13.9000 | -23.7500 | 62.1500  | 100.3500 | 63.0500 |
|----------|----------|----------|----------|----------|---------|
| -13.9000 | 41.3000  | 32.7500  | 44.9500  | -26.9500 | -5.1000 |
| -23.7500 | 32.7500  | 40.0000  | 42.5000  | -33.0000 | -8.5000 |
| 62.1500  | 44.9500  | 42.5000  | 151.3000 | 53.7000  | 53.8500 |
| 100.3500 | -26.9500 | -33.0000 | 53.7000  | 110.8000 | 65.9000 |
| 63.0500  | -5.1000  | -8.5000  | 53.8500  | 65.9000  | 43.7000 |


EVectors =
| 0.5004  | -0.3882 | -0.3944 | -0.3443 | 0.2028  | 0.5326  |
|---------|---------|---------|---------|---------|---------|
| -0.1327 | 0.3223  | -0.0219 | -0.8160 | -0.4606 | -0.0088 |
| 0.1816  | 0.3080  | -0.7089 | 0.3788  | -0.4733 | -0.0459 |
| 0.0683  | -0.2149 | 0.4523  | 0.2489  | -0.6424 | 0.5196  |
| 0.0307  | 0.7492  | 0.1304  | 0.0965  | 0.3278  | 0.5513  |
| -0.8327 | -0.2075 | -0.3461 | 0.0297  | 0.0515  | 0.3745  |


Evalues =

| -0.0000 | 0      | 0      | 0      | 0        | 0        |
|---------|--------|--------|--------|----------|----------|
| 0       | 0.0000 | 0      | 0      | 0        | 0        |
| 0       | 0      | 2.6035 | 0      | 0        | 0        |
| 0       | 0      | 0      | 9.8930 | 0        | 0        |
| 0       | 0      | 0      | 0      | 163.5103 | 0        |
| 0       | 0      | 0      | 0      | 0        | 306.2932 |

sortedD =
| 306.2932 |
|----------|
| 163.5103 |
| 9.8930   |
| 2.6035   |
| 0.0000   |
| -0.0000  |


orderD =
| 6 |
|---|
| 5 |
| 4 |
| 3 |
| 2 |
| 1 |

sortedEvalues =

| 306.2932 | 0        | 0      | 0      | 0      | 0       |
|----------|----------|--------|--------|--------|---------|
| 0        | 163.5103 | 0      | 0      | 0      | 0       |
| 0        | 0        | 9.8930 | 0      | 0      | 0       |
| 0        | 0        | 0      | 2.6035 | 0      | 0       |
| 0        | 0        | 0      | 0      | 0.0000 | 0       |
| 0        | 0        | 0      | 0      | 0      | -0.0000 |


sortedEvectors =
| 0.5326  | 0.2028  | -0.3443 | -0.3944 | -0.3882 | 0.5004  |
|---------|---------|---------|---------|---------|---------|
| -0.0088 | -0.4606 | -0.8160 | -0.0219 | 0.3223  | -0.1327 |
| -0.0459 | -0.4733 | 0.3788  | -0.7089 | 0.3080  | 0.1816  |
| 0.5196  | -0.6424 | 0.2489  | 0.4523  | -0.2149 | 0.0683  |
| 0.5513  | 0.3278  | 0.0965  | 0.1304  | 0.7492  | 0.0307  |
| 0.3745  | 0.0515  | 0.0297  | -0.3461 | -0.2075 | -0.8327 |


sumOfEvalues =

  482.3000


percentage =

    0.6351


percentage =

    0.9741


percentage =

    0.9946


percentage =

    1.0000


percentage =

    1.0000


percentage =

     1


k =

     2


filteredEvalues =
| 306.2932 | 0        |
|----------|----------|
| 0        | 163.5103 |


filteredEvectors =

| 0.5326  | 0.2028  |
|---------|---------|
| -0.0088 | -0.4606 |
| -0.0459 | -0.4733 |
| 0.5196  | -0.6424 |
| 0.5513  | 0.3278  |
| 0.3745  | 0.0515  |


rowFeatureVectors =

| 0.5326 | -0.0088 | -0.0459 | 0.5196  | 0.5513 | 0.3745 |
|--------|---------|---------|---------|--------|--------|
| 0.2028 | -0.4606 | -0.4733 | -0.6424 | 0.3278 | 0.0515 |


rowDataAdjust =
| 9.8000  | -10.2000 | -9.2000  | -0.2000 | 9.8000 |
|---------|----------|----------|---------|--------|
| -7.6000 | 4.4000   | -5.6000  | 7.4000  | 1.4000 |
| -7.0000 | 9.0000   | -5.0000  | 1.0000  | 2.0000 |
| 1.6000  | 5.6000   | -21.4000 | 4.6000  | 9.6000 |
| 13.4000 | -10.6000 | -8.6000  | -2.6000 | 8.4000 |
| 6.2000  | -4.8000  | -7.8000  | -0.8000 | 7.2000 |


FinalData =
| 16.1486 | -10.6168 | -23.4021 | 0.4397  | 17.4306 | 0.3745 |
|---------|----------|----------|---------|---------|--------|
| 12.4840 | -15.6732 | 13.6071  | -7.7705 | -2.6474 | 0.0515 |


reconstructData =
| 85.3331 | 66.7085 | 61.3497 | 70.7706 | 78.5947 | 81.4892 |
|---------|---------|---------|---------|---------|---------|
| 65.3667 | 79.9120 | 75.9056 | 74.9522 | 54.6098 | 70.0181 |
| 64.4944 | 66.5377 | 62.6350 | 49.5003 | 57.1578 | 66.7372 |
| 72.8584 | 76.1752 | 71.6575 | 75.6201 | 63.2956 | 74.5648 |
| 82.9474 | 73.6666 | 68.4523 | 81.1568 | 74.3422 | 81.1907 |


sample =
| 84 | 65 | 61 | 72 | 79 | 81 |
|----|----|----|----|----|----|
| 64 | 77 | 77 | 76 | 55 | 70 |
| 65 | 67 | 63 | 49 | 57 | 67 |
| 74 | 80 | 69 | 75 | 63 | 74 |
| 84 | 74 | 70 | 80 | 74 | 82 |


diff =

| -1.3331 | -1.7085 | -0.3497 | 1.2294  | 0.4053  | -0.4892 |
|---------|---------|---------|---------|---------|---------|
| -1.3667 | -2.9120 | 1.0944  | 1.0478  | 0.3902  | -0.0181 |
| 0.5056  | 0.4623  | 0.3650  | -0.5003 | -0.1578 | 0.2628  |
| 1.1416  | 3.8248  | -2.6575 | -0.6201 | -0.2956 | -0.5648 |
| 1.0526  | 0.3334  | 1.5477  | -1.1568 | -0.3422 | 0.8093  |
