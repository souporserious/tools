# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2017 > async-functions > 30`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "es2017/async-functions/30/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "es2017/async-functions/30/input.js"
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
		JSVariableDeclarationStatement {
			loc: Object {
				filename: "es2017/async-functions/30/input.js"
				end: Object {
					column: 40
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			declaration: JSVariableDeclaration {
				kind: "const"
				loc: Object {
					filename: "es2017/async-functions/30/input.js"
					end: Object {
						column: 40
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				declarations: Array [
					JSVariableDeclarator {
						id: JSBindingIdentifier {
							name: "foo"
							loc: Object {
								filename: "es2017/async-functions/30/input.js"
								identifierName: "foo"
								end: Object {
									column: 9
									line: 1
								}
								start: Object {
									column: 6
									line: 1
								}
							}
						}
						loc: Object {
							filename: "es2017/async-functions/30/input.js"
							end: Object {
								column: 39
								line: 1
							}
							start: Object {
								column: 6
								line: 1
							}
						}
						init: JSFunctionExpression {
							id: undefined
							loc: Object {
								filename: "es2017/async-functions/30/input.js"
								end: Object {
									column: 39
									line: 1
								}
								start: Object {
									column: 12
									line: 1
								}
							}
							body: JSBlockStatement {
								body: Array []
								directives: Array []
								loc: Object {
									filename: "es2017/async-functions/30/input.js"
									end: Object {
										column: 39
										line: 1
									}
									start: Object {
										column: 37
										line: 1
									}
								}
							}
							head: JSFunctionHead {
								async: false
								generator: false
								hasHoistedVars: false
								rest: undefined
								returnType: undefined
								thisType: undefined
								typeParameters: undefined
								loc: Object {
									filename: "es2017/async-functions/30/input.js"
									end: Object {
										column: 36
										line: 1
									}
									start: Object {
										column: 20
										line: 1
									}
								}
								params: Array [
									JSBindingObjectPattern {
										rest: undefined
										loc: Object {
											filename: "es2017/async-functions/30/input.js"
											end: Object {
												column: 35
												line: 1
											}
											start: Object {
												column: 21
												line: 1
											}
										}
										meta: JSPatternMeta {
											optional: undefined
											typeAnnotation: undefined
											loc: Object {
												filename: "es2017/async-functions/30/input.js"
												end: Object {
													column: 35
													line: 1
												}
												start: Object {
													column: 21
													line: 1
												}
											}
										}
										properties: Array [
											JSBindingObjectPatternProperty {
												key: JSStaticPropertyKey {
													value: JSIdentifier {
														name: "async"
														loc: Object {
															filename: "es2017/async-functions/30/input.js"
															identifierName: "async"
															end: Object {
																column: 28
																line: 1
															}
															start: Object {
																column: 23
																line: 1
															}
														}
													}
													loc: Object {
														filename: "es2017/async-functions/30/input.js"
														end: Object {
															column: 28
															line: 1
														}
														start: Object {
															column: 23
															line: 1
														}
													}
												}
												value: JSBindingIdentifier {
													name: "bar"
													loc: Object {
														filename: "es2017/async-functions/30/input.js"
														identifierName: "bar"
														end: Object {
															column: 33
															line: 1
														}
														start: Object {
															column: 30
															line: 1
														}
													}
												}
												loc: Object {
													filename: "es2017/async-functions/30/input.js"
													end: Object {
														column: 33
														line: 1
													}
													start: Object {
														column: 23
														line: 1
													}
												}
											}
										]
									}
								]
							}
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
✔ No known problems!

```