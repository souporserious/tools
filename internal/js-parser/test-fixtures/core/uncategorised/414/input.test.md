# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `core > uncategorised > 414`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: true
	directives: Array []
	filename: "core/uncategorised/414/input.js"
	hasHoistedVars: false
	integrity: undefined
	interpreter: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "core/uncategorised/414/input.js"
		end: Object {
			column: 6
			line: 1
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse"}]
			description: Object {
				advice: Array []
				category: "parse"
				categoryValue: "js"
				message: Array [
					RAW_MARKUP {value: "Unknown start to an "}
					"throw argument"
				]
			}
			location: Object {
				filename: "core/uncategorised/414/input.js"
				integrity: undefined
				language: "js"
				sourceText: undefined
				end: Object {
					column: 5
					line: 1
				}
				start: Object {
					column: 5
					line: 1
				}
			}
		}
	]
	body: Array [
		JSThrowStatement {
			loc: Object {
				filename: "core/uncategorised/414/input.js"
				end: Object {
					column: 6
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			argument: JSReferenceIdentifier {
				name: "INVALID_PLACEHOLDER"
				loc: Object {
					filename: "core/uncategorised/414/input.js"
					end: Object {
						column: 6
						line: 1
					}
					start: Object {
						column: 5
						line: 1
					}
				}
			}
		}
	]
}
```

### `diagnostics`

```

 core/uncategorised/414/input.js:1:5 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Unknown start to an throw argument

    throw;
         ^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
