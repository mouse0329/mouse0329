# TypeScript 型リスト

## 1. 基本型
| 型名         | 説明                                         | 使用例                         |
|--------------|---------------------------------------------|--------------------------------|
| `string`     | 文字列を表す                                 | `let name: string = "Hello";` |
| `number`     | 数値を表す（整数、小数含む）                 | `let age: number = 25;`       |
| `boolean`    | 真偽値を表す                                 | `let isDone: boolean = true;` |
| `null`       | 明示的に「値がない」状態                     | `let empty: null = null;`     |
| `undefined`  | 未定義の値                                  | `let notDefined: undefined;`  |
| `bigint`     | 任意の大きな整数値を表す（`ES2020`以降）      | `let big: bigint = 100n;`     |
| `symbol`     | 一意の値を生成する                           | `let sym: symbol = Symbol();` |

## 2. 配列
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `Array`      | 配列型を表す                                 | `let nums: number[] = [1, 2, 3];`  |
| `Tuple`      | 要素数と型が固定された配列                   | `let tuple: [string, number] = ["apple", 5];` |

## 3. オブジェクト
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `object`     | オブジェクト全般を表す（詳細な型付けなし）    | `let obj: object = { key: "value" };` |
| 型リテラル    | オブジェクトの詳細な型定義                  | `let person: { name: string; age: number } = { name: "Taro", age: 30 };` |

## 4. 特殊型
| 型名         | 説明                                       | 使用例                              |
|--------------|-------------------------------------------|-------------------------------------|
| `any`        | どんな値でも許容（非推奨）                 | `let data: any = "Hello";`         |
| `unknown`    | 値の型が不明だが、型チェックが必要         | `let input: unknown;`             |
| `never`      | 決して値を返さない（例外を投げる関数など） | `function error(): never { throw new Error("Error!"); }` |
| `void`       | 値を返さない関数の戻り値                  | `function log(): void { console.log("Hello"); }` |

## 5. ユニオン型・交差型
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `Union`      | 複数の型を許容（`|`を使用）                  | `let id: string | number;`        |
| `Intersection`| 複数の型を結合（`&`を使用）               | `type FullName = { first: string } & { last: string };` |

## 6. 型エイリアス
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `Type Alias` | カスタム型を定義する                      | `type ID = string | number;`      |

## 7. 列挙型
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `enum`       | 列挙型を定義                                 | `enum Color { Red, Green, Blue }`  |

## 8. 関数型
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `Function`   | 関数の型を定義する                        | `let add: (a: number, b: number) => number;` |

## 9. ジェネリクス
| 型名         | 説明                                         | 使用例                              |
|--------------|---------------------------------------------|-------------------------------------|
| `Generics`   | 型を柔軟にするためのテンプレート           | `function identity<T>(arg: T): T { return arg; }` |

<!---
mouse0329/mouse0329 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
