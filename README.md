# SudokuMaker

SudokuMaker which can make sudoku 4x4, 9x9, 16x16, …, 100x100.

## Installation

```python
pip install sudoku_maker
```

## Usage

```python
import sudoku_maker

sudoku_maker.make(args)
```

args is a block number (generally => 9)

args is only permited in (4, 9, 16, 25, 36, 49, 64, 81, 100)

e.g. sudoku_maker.make(4) #=> [[3, 1, 2, 4], [4, 3, 1, 2], [1, 2, 4, 3], [2, 4, 3, 1]]

means

```
-----------------
| 3 | 1 | 2 | 4 |
-----------------
| 4 | 3 | 1 | 2 |
-----------------
| 1 | 2 | 4 | 3 |
-----------------
| 2 | 4 | 3 | 1 |
-----------------
```

## Demo

```python
>>> import sudoku_maker

>>> sudoku_maker.make(9)
[[6, 4, 9, 2, 3, 8, 1, 7, 5], [4, 7, 6, 8, 9, 3, 5, 1, 2], [7, 1, 4, 3, 6, 9, 2, 5, 8], [5, 2, 1, 6, 7, 4, 3, 8, 9], [1, 5, 7, 9, 4, 6, 8, 2, 3], [2, 8, 5, 4, 1, 7, 9, 3, 6], [8, 3, 2, 7, 5, 1, 6, 9, 4], [9, 6, 3, 5, 8, 2, 7, 4, 1], [3, 9, 8, 1, 2, 5, 4, 6, 7]]

>>> sudoku_maker.make(25)
[[12, 11, 15, 16, 22, 25, 21, 5, 10, 2, 4, 20, 23, 9, 1, 19, 8, 17, 6, 13, 3, 24, 18, 7, 14], [19, 22, 16, 12, 6, 24, 18, 21, 2, 25, 9, 1, 20, 10, 5, 13, 17, 4, 8, 23, 15, 3, 7, 14, 11], [6, 16, 11, 22, 12, 18, 25, 2, 5, 21, 20, 9, 4, 1, 10, 8, 13, 23, 19, 17, 14, 7, 24, 3, 15], [22, 15, 14, 11, 16, 21, 2, 10, 1, 5, 23, 4, 17, 20, 9, 6, 19, 13, 12, 8, 7, 18, 25, 24, 3], [8, 12, 22, 6, 19, 7, 24, 25, 21, 18, 1, 10, 9, 5, 2, 17, 23, 20, 13, 4, 11, 14, 3, 15, 16], [4, 13, 8, 17, 23, 11, 15, 3, 7, 14, 21, 25, 2, 18, 24, 9, 1, 5, 20, 10, 6, 22, 16, 12, 19], [23, 8, 19, 13, 17, 15, 14, 7, 24, 3, 2, 21, 5, 25, 18, 20, 9, 10, 4, 1, 12, 16, 11, 22, 6], [17, 19, 6, 8, 13, 14, 3, 24, 18, 7, 5, 2, 10, 21, 25, 4, 20, 1, 23, 9, 22, 11, 15, 16, 12], [20, 17, 13, 23, 4, 16, 11, 14, 3, 15, 25, 18, 21, 24, 7, 1, 10, 2, 9, 5, 19, 12, 22, 6, 8], [13, 6, 12, 19, 8, 3, 7, 18, 25, 24, 10, 5, 1, 2, 21, 23, 4, 9, 17, 20, 16, 15, 14, 11, 22], [3, 18, 25, 24, 7, 9, 20, 23, 17, 4, 6, 19, 12, 8, 13, 15, 11, 22, 14, 16, 2, 10, 1, 5, 21], [14, 24, 18, 7, 3, 1, 9, 4, 23, 20, 19, 8, 6, 13, 17, 11, 16, 12, 15, 22, 21, 5, 10, 2, 25], [16, 14, 3, 15, 11, 2, 5, 1, 9, 10, 17, 23, 13, 4, 20, 12, 6, 8, 22, 19, 24, 25, 21, 18, 7], [15, 7, 24, 3, 14, 10, 1, 20, 4, 9, 8, 13, 19, 17, 23, 16, 22, 6, 11, 12, 25, 2, 5, 21, 18], [11, 3, 7, 14, 15, 5, 10, 9, 20, 1, 13, 17, 8, 23, 4, 22, 12, 19, 16, 6, 18, 21, 2, 25, 24], [2, 1, 9, 10, 5, 8, 19, 12, 22, 6, 14, 15, 3, 11, 16, 25, 18, 7, 21, 24, 4, 17, 13, 23, 20], [5, 9, 20, 1, 10, 19, 6, 22, 16, 12, 3, 14, 7, 15, 11, 21, 25, 24, 2, 18, 23, 13, 8, 17, 4], [10, 20, 4, 9, 1, 6, 12, 16, 11, 22, 7, 3, 24, 14, 15, 2, 21, 18, 5, 25, 17, 8, 19, 13, 23], [1, 4, 23, 20, 9, 12, 22, 11, 15, 16, 24, 7, 18, 3, 14, 5, 2, 25, 10, 21, 13, 19, 6, 8, 17], [9, 23, 17, 4, 20, 22, 16, 15, 14, 11, 18, 24, 25, 7, 3, 10, 5, 21, 1, 2, 8, 6, 12, 19, 13], [18, 2, 5, 21, 25, 23, 17, 8, 19, 13, 16, 22, 11, 12, 6, 7, 3, 15, 24, 14, 1, 20, 4, 9, 10], [25, 5, 10, 2, 21, 17, 13, 19, 6, 8, 11, 16, 15, 22, 12, 24, 7, 14, 18, 3, 9, 4, 23, 20, 1], [21, 10, 1, 5, 2, 13, 8, 6, 12, 19, 15, 11, 14, 16, 22, 18, 24, 3, 25, 7, 20, 23, 17, 4, 9], [7, 25, 21, 18, 24, 20, 4, 17, 13, 23, 12, 6, 22, 19, 8, 14, 15, 16, 3, 11, 5, 1, 9, 10, 2], [24, 21, 2, 25, 18, 4, 23, 13, 8, 17, 22, 12, 16, 6, 19, 3, 14, 11, 7, 15, 10, 9, 20, 1, 5]]

```

## Contributing

1. Fork it ( https://github.com/hooor/sudoku_maker_python/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
