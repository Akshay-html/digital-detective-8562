# Mission 05 - Numbers and data

## 1. Task / objective

AI-assisted draft: practise decimal/binary/hexadecimal conversion, verify examples using Python, build a converter, and explain text encoding. Review every calculation and explain the code yourself before submitting.

## 2. Work completed

### Hand conversion answers

| Question | Working | Answer |
|---|---|---|
| Decimal 13 to binary | 13 ÷ 2 remainders (bottom-up): 1, 1, 0, 1 | `1101₂` |
| Decimal 25 to binary | 25 ÷ 2 remainders (bottom-up): 1, 1, 0, 0, 1 | `11001₂` |
| `1010₂` to decimal | 1×8 + 0×4 + 1×2 + 0×1 | `10₁₀` |
| `1101₂` to decimal | 1×8 + 1×4 + 0×2 + 1×1 | `13₁₀` |
| `A₁₆` to decimal | A represents 10 | `10₁₀` |
| `1F₁₆` to decimal | 1×16 + 15 | `31₁₀` |
| `1111₂` to hexadecimal | 8 + 4 + 2 + 1 = 15 | `F₁₆` |

### Python checks

`bin(13)` returns `0b1101`; `int('1010', 2)` returns `10`; `hex(31)` returns `0x1f`. The converter uses `input()` to read text, `int()` to parse decimal input, `bin()` to convert to binary, and `hex()` to convert to hexadecimal. `[2:]` removes the `0b`/`0x` prefix; `.upper()` displays hexadecimal letters in uppercase.

### Converter runs

| Decimal input | Binary | Hexadecimal |
|---:|---:|---:|
| 10 | `1010` | `A` |
| 13 | `1101` | `D` |
| 25 | `11001` | `19` |

### Text encoding

ASCII decimal code for uppercase `A`: 65. For lowercase `a`: 97. An encoding standard maps characters to numbers/bytes so devices store and exchange text consistently. Example outside basic ASCII: `अ`.

## 3. Commands / tools used

`python3 number_converter.py`; built-in Python functions `input`, `int`, `bin`, and `hex`.

## 4. My understanding

Reference note: binary is base 2 and hexadecimal is base 16. Binary digits are grouped in fours to map to a hexadecimal digit; `1111₂` is decimal 15, which is `F₁₆`. Encoding gives software a shared mapping from characters to numeric values. Rewrite this in your own words.

## 5. Difficulties faced

No error occurred during the three converter runs. Python 3.9.6 was already available.

## 6. How I resolved them

Not applicable. The examples were checked using Python's built-in conversions.

## 7. Evidence / files

`number_converter.py`; this README records manual conversions and three observed runs.

## 8. Commit details

Commit message: `Build number converter and practise data representation`.
