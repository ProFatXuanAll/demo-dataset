# Chinese Poetry Dataset

Source: https://github.com/Werneror/Poetry

Pre-processed version of [chinese poetry dataset](https://github.com/Werneror/Poetry).
Pre-processing includes:

- NFKC normalization (using [Python's `unicodedata`](https://docs.python.org/3/library/unicodedata.html))
- Convert simplified chinese to traditional chinese (using [`opencc`](https://github.com/BYVoid/OpenCC))

All files are compressed as zip files to reduce storage size.

## Statistics

收錄了從先秦到現代的共計85萬餘首古詩詞。

| 朝代           | 詩詞數  | 作者數  |
|---------------|--------|--------|
| 宋            | 287114 |   9446 |
| 明            | 236957 |   4439 |
| 清            |  90089 |   8872 |
| 唐            |  49195 |   2736 |
| 元            |  37375 |   1209 |
| 近現代        |  28419 |    790 |
| 當代          |  28219 |    177 |
| 明末清初       |  17700 |    176 |
| 元末明初       |  15736 |     79 |
| 清末民國初     |  15367 |     99 |
| 清末近現代初   |  12464 |     48 |
| 宋末元初      |  12058 |     41 |
| 南北朝        |   4586 |    434 |
| 近現代末當代初 |   3426 |     23 |
| 魏晉          |   3020 |    251 |
| 金末元初      |   3019 |     17 |
| 金            |   2741 |    253 |
| 民國末當代初   |   1948 |      9 |
| 隋            |   1170 |     84 |
| 唐末宋初      |   1118 |     44 |
| 先秦          |    570 |      8 |
| 隋末唐初      |    472 |     40 |
| 漢            |    363 |     83 |
| 宋末金初      |    234 |      9 |
| 遼            |     22 |      7 |
| 秦            |      2 |      2 |
| 魏晉末南北朝初  |      1 |      1 |
| 總和          | 853385 |  29377 |

## Format

古詩詞數據按朝代存儲於多個 csv 文件中，有"題目"、"朝代"、"作者"和"內容"共四個字段
古詩詞中有一些生僻字，這些生僻字屬於 utf8mb4 字符，在許多設備中無法顯示，故而使用"?"來替代。

## License

MIT License.
