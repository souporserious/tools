# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > expression-grouping > migrated_0000`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "esprima/expression-grouping/migrated_0000/input.js"
	hasHoistedVars: false
	integrity: undefined
	interpreter: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "esprima/expression-grouping/migrated_0000/input.js"
		end: Object {
			column: 0
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "esprima/expression-grouping/migrated_0000/input.js"
				end: Object {
					column: 15
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSBinaryExpression {
				operator: "+"
				loc: Object {
					filename: "esprima/expression-grouping/migrated_0000/input.js"
					end: Object {
						column: 15
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				right: JSNumericLiteral {
					value: 3
					format: undefined
					raw: "3"
					loc: Object {
						filename: "esprima/expression-grouping/migrated_0000/input.js"
						end: Object {
							column: 15
							line: 1
						}
						start: Object {
							column: 14
							line: 1
						}
					}
				}
				left: JSBinaryExpression {
					operator: "+"
					loc: Object {
						filename: "esprima/expression-grouping/migrated_0000/input.js"
						end: Object {
							column: 11
							line: 1
						}
						start: Object {
							column: 0
							line: 1
						}
					}
					left: JSNumericLiteral {
						value: 1
						format: undefined
						raw: "1"
						loc: Object {
							filename: "esprima/expression-grouping/migrated_0000/input.js"
							end: Object {
								column: 2
								line: 1
							}
							start: Object {
								column: 1
								line: 1
							}
						}
					}
					right: JSNumericLiteral {
						value: 2
						format: undefined
						raw: "2"
						loc: Object {
							filename: "esprima/expression-grouping/migrated_0000/input.js"
							end: Object {
								column: 8
								line: 1
							}
							start: Object {
								column: 7
								line: 1
							}
						}
					}
				}
			}
		}
	]
}
```

### `diagnostics`

```
✔ No known problems!

```
