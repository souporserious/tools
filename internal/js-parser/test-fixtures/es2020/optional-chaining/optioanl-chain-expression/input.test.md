# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2020 > optional-chaining > optioanl-chain-expression`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
	hasHoistedVars: false
	integrity: undefined
	interpreter: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
		end: Object {
			column: 8
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
				filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
				end: Object {
					column: 8
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSOptionalCallExpression {
				arguments: Array []
				loc: Object {
					filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
					end: Object {
						column: 8
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				callee: JSMemberExpression {
					loc: Object {
						filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
						end: Object {
							column: 6
							line: 1
						}
						start: Object {
							column: 0
							line: 1
						}
					}
					property: JSStaticMemberProperty {
						value: JSIdentifier {
							name: "c"
							loc: Object {
								filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
								identifierName: "c"
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
						optional: true
						loc: Object {
							filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
							identifierName: "c"
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
					object: JSMemberExpression {
						loc: Object {
							filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
							end: Object {
								column: 3
								line: 1
							}
							start: Object {
								column: 0
								line: 1
							}
						}
						object: JSReferenceIdentifier {
							name: "a"
							loc: Object {
								filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
								identifierName: "a"
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
						property: JSStaticMemberProperty {
							value: JSIdentifier {
								name: "b"
								loc: Object {
									filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
									identifierName: "b"
									end: Object {
										column: 3
										line: 1
									}
									start: Object {
										column: 2
										line: 1
									}
								}
							}
							loc: Object {
								filename: "es2020/optional-chaining/optioanl-chain-expression/input.js"
								identifierName: "b"
								end: Object {
									column: 3
									line: 1
								}
								start: Object {
									column: 2
									line: 1
								}
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
