# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `core > uncategorised > 502`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "core/uncategorised/502/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "core/uncategorised/502/input.js"
		end: Object {
			column: 49
			line: 1
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
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Legacy octal literals are not allowed in strict mode"}]}
			}
			location: Object {
				filename: "core/uncategorised/502/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 39
					line: 1
				}
				start: Object {
					column: 39
					line: 1
				}
			}
		}
	]
	body: Array [
		JSFunctionDeclaration {
			id: JSBindingIdentifier {
				name: "hello"
				loc: Object {
					filename: "core/uncategorised/502/input.js"
					identifierName: "hello"
					end: Object {
						column: 14
						line: 1
					}
					start: Object {
						column: 9
						line: 1
					}
				}
			}
			loc: Object {
				filename: "core/uncategorised/502/input.js"
				end: Object {
					column: 49
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			head: JSFunctionHead {
				async: false
				generator: false
				hasHoistedVars: false
				params: Array []
				rest: undefined
				returnType: undefined
				thisType: undefined
				typeParameters: undefined
				loc: Object {
					filename: "core/uncategorised/502/input.js"
					end: Object {
						column: 16
						line: 1
					}
					start: Object {
						column: 14
						line: 1
					}
				}
			}
			body: JSBlockStatement {
				loc: Object {
					filename: "core/uncategorised/502/input.js"
					end: Object {
						column: 49
						line: 1
					}
					start: Object {
						column: 17
						line: 1
					}
				}
				directives: Array [
					JSDirective {
						value: "use strict"
						loc: Object {
							filename: "core/uncategorised/502/input.js"
							end: Object {
								column: 32
								line: 1
							}
							start: Object {
								column: 19
								line: 1
							}
						}
					}
				]
				body: Array [
					JSExpressionStatement {
						loc: Object {
							filename: "core/uncategorised/502/input.js"
							end: Object {
								column: 47
								line: 1
							}
							start: Object {
								column: 33
								line: 1
							}
						}
						expression: JSObjectExpression {
							loc: Object {
								filename: "core/uncategorised/502/input.js"
								end: Object {
									column: 45
									line: 1
								}
								start: Object {
									column: 34
									line: 1
								}
							}
							properties: Array [
								JSObjectProperty {
									key: JSStaticPropertyKey {
										value: JSNumericLiteral {
											value: 17
											format: "octal"
											loc: Object {
												filename: "core/uncategorised/502/input.js"
												end: Object {
													column: 39
													line: 1
												}
												start: Object {
													column: 36
													line: 1
												}
											}
										}
										loc: Object {
											filename: "core/uncategorised/502/input.js"
											end: Object {
												column: 39
												line: 1
											}
											start: Object {
												column: 36
												line: 1
											}
										}
									}
									value: JSNumericLiteral {
										value: 42
										format: undefined
										loc: Object {
											filename: "core/uncategorised/502/input.js"
											end: Object {
												column: 43
												line: 1
											}
											start: Object {
												column: 41
												line: 1
											}
										}
									}
									loc: Object {
										filename: "core/uncategorised/502/input.js"
										end: Object {
											column: 43
											line: 1
										}
										start: Object {
											column: 36
											line: 1
										}
									}
								}
							]
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 core/uncategorised/502/input.js:1:39 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Legacy octal literals are not allowed in strict mode

    function hello() { 'use strict'; ({ 021: 42 }); }
                                           ^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```