# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > statement-block > migrated_0000`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "esprima/statement-block/migrated_0000/input.js"
	hasHoistedVars: false
	integrity: undefined
	interpreter: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "esprima/statement-block/migrated_0000/input.js"
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
		JSBlockStatement {
			directives: Array []
			loc: Object {
				filename: "esprima/statement-block/migrated_0000/input.js"
				end: Object {
					column: 7
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			body: Array [
				JSExpressionStatement {
					loc: Object {
						filename: "esprima/statement-block/migrated_0000/input.js"
						end: Object {
							column: 5
							line: 1
						}
						start: Object {
							column: 2
							line: 1
						}
					}
					expression: JSReferenceIdentifier {
						name: "foo"
						loc: Object {
							filename: "esprima/statement-block/migrated_0000/input.js"
							identifierName: "foo"
							end: Object {
								column: 5
								line: 1
							}
							start: Object {
								column: 2
								line: 1
							}
						}
					}
				}
			]
		}
	]
}
```

### `diagnostics`

```
✔ No known problems!

```
