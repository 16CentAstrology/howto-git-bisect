# How to use ´git bisect´

Find the change that introduced a bug in your code.

## How does it work?


| Step 1   | Step 2   | Step 3   | Step 4   | Step 5   | Step 6   | Step 7   |
|----------|----------|----------|----------|----------|----------|----------|
| `4a4e` :bomb: |     |          |          |          |          |          |
| `cfaf`   |          |          |          |          |          |          |
| `e6f1`   |          |          |          |          |          |          |
| `77ca`   |          |          |          |          |          |          |
| `9e15`   |          |          |          |          |          |          |
| `f99c`   |          |          |          |          |          |          |
| `1642`   |          |          |          |          |          |          |
| `4ba6`   |          |          |          |          |          |          |
| `7e56`   |          |          |          |          |          |          |
| `397b`   |          |          |          |          |          |          |
| `7eb5`   |          |          |          |          |          |          |
| `4203`   |          |          |          |          |          |          |
| `09af`   |          |          |          |          |          |          |
| `6d3b`   |          |          |          |          |          |          |
| `0219`   |          |          |          |          |          |          |
| `34a1` ? | `34a1` :bomb: | `34a1` :bomb: |          |          |          |          |
| `1054`   | `1054`   | `1054`   |          |          |          |          |
| `bcab`   | `bcab`   | `bcab`   |          |          |          |          |
| `4ae6`   | `4ae6`   | `4ae6` ? | `4ae6` :bomb: |          |          |          |
| `7d75`   | `7d75`   | `7d75`   | `7d75`   |          |          |          |
| `e079`   | `e079`   | `e079`   | `e079` ? | `e079` :bomb: | `e079` :bomb: | `e079` :bomb: |
| `8013`   | `8013`   | `8013`   | `8013`   | `8013` ? | `801e` :smiley_cat: |          |
| `7487`   | `7487` ? | `7487` :smiley_cat: | `7487` :smiley_cat: | `7487` :smiley_cat: |         |          |
| `f3b2`   | `f3b2`   |          |          |          |          |          |
| `b12a`   | `b12a`   |          |          |          |          |          |
| `301f`   | `301f`   |          |          |          |          |          |
| `5151`   | `5151`   |          |          |          |          |          |
| `2dac`   | `2dac`   |          |          |          |          |          |
| `1ed8`   | `1ed8`   |          |          |          |          |          |
| `f8a4` :smiley_cat: | `f8a4` :smiley_cat: |          |          |          |          |          |
| `...`    |          |          |          |          |          |          |  
