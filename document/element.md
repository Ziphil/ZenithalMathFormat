## 要素

### 括弧類 (`p`, `b`, ･･･)

#### 構文
```
\p<(内容)><(内容)> ･･･ <(内容)>
```

2 つ以上の引数が渡された場合は、それぞれがコンマで区切られる。

#### 変種
| 名称 | 括弧 |
|:----:|:----:|
| `p` | ( ～ ) |
| `b` | [ ～ ] |
| `c` | { ～ } |
| `v` | \| ～ \| |
| `vv` | ‖ ～ ‖ |
| `f` | ⌊ ～ ⌋ |
| `g` | ⌈ ～ ⌉ |
| `a` | ⟨ ～ ⟩ |
| `aa` | ⟪ ～ ⟫ |

### 上付きと下付き (`sp`, `sb`, `spsb`)

#### 構文
```
\sp<(ベース)><(上付き)>
\sb<(ベース)><(下付き)>
\spsb<(ベース)><(上付き)><(下付き)>
```

#### 例
```
\sp<x><2> + 1
\sb<A><ij>
```

### 分数 (`frac`, `dfrac`)

#### 構文
```
\frac<(分子)><(分母)>
\dfrac<(分子)><(分母)>
```

`dfrac` は常にディスプレイスタイルになる。

### 根号 (`sqrt`)

#### 構文
```
\sqrt<(内容)>
\sqrt<(内容)><(指数)>
```

指数は省略可能。

### 積分記号 (`int`, `oint`, ･･･)

#### 構文
``` 
\int>
\int<(下限)><(上限)>
```

下限と上限は省略可能。

#### 変種
| 名称 | 記号 |
|:----:|:----:|
| `int` | ∫ |
| `oint` | ∮ |

### 関数類 (`sin`, `cos`, ･･･)

#### 構文
```
\sin>
```

#### 変種
たくさんある。

### 記号類

#### 構文
```
\pm>
```

#### 変種
たくさんある。

## その他の拡張

### ギリシャ文字

#### 構文
```
`a
```

通常の ZenML のエスケープ構文のように、`` ` `` に続けてラテン文字を置くと、対応するギリシャ文字に変換される。

#### 例
```
\sin> (`u + `f) = \sin> `u \cos> `f + \cos `u \sin `f
```