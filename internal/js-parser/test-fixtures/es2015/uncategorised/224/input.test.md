# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > uncategorised > 224`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "es2015/uncategorised/224/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "es2015/uncategorised/224/input.js"
		end: Object {
			column: 5
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Expected a semicolon or a line terminator"}]}
			}
			location: Object {
				filename: "es2015/uncategorised/224/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 3
					line: 2
				}
				start: Object {
					column: 4
					line: 2
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "es2015/uncategorised/224/input.js"
				end: Object {
					column: 1
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSReferenceIdentifier {
				name: "x"
				loc: Object {
					filename: "es2015/uncategorised/224/input.js"
					identifierName: "x"
					end: Object {
						column: 1
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
			}
		}
		JSExpressionStatement {
			loc: Object {
				filename: "es2015/uncategorised/224/input.js"
				end: Object {
					column: 3
					line: 2
				}
				start: Object {
					column: 1
					line: 2
				}
			}
			expression: JSReferenceIdentifier {
				name: "is"
				loc: Object {
					filename: "es2015/uncategorised/224/input.js"
					identifierName: "is"
					end: Object {
						column: 3
						line: 2
					}
					start: Object {
						column: 1
						line: 2
					}
				}
			}
		}
		JSExpressionStatement {
			loc: Object {
				filename: "es2015/uncategorised/224/input.js"
				end: Object {
					column: 5
					line: 2
				}
				start: Object {
					column: 4
					line: 2
				}
			}
			expression: JSReferenceIdentifier {
				name: "y"
				loc: Object {
					filename: "es2015/uncategorised/224/input.js"
					identifierName: "y"
					end: Object {
						column: 5
						line: 2
					}
					start: Object {
						column: 4
						line: 2
					}
				}
			}
		}
	]
}
```

### `diagnostics`

```

 es2015/uncategorised/224/input.js:2:4 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Expected a semicolon or a line terminator

    1 │ x·
  > 2 │  is y
      │     ^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```