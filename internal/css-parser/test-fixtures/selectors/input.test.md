# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/css-parser/index.test.ts --update-snapshots` to update.

## `selectors`

```javascript
CSSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	filename: "selectors/input.css"
	integrity: undefined
	loc: Object {
		filename: "selectors/input.css"
		end: Object {
			column: 1
			line: 11
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	body: Array [
		CSSRule {
			loc: Object {
				filename: "selectors/input.css"
				end: Object {
					column: 1
					line: 3
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			block: CSSBlock {
				value: Array []
				startingTokenValue: "{"
				loc: Object {
					filename: "selectors/input.css"
					end: Object {
						column: 1
						line: 3
					}
					start: Object {
						column: 37
						line: 1
					}
				}
			}
			prelude: Array [
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 3
							line: 1
						}
						start: Object {
							column: 0
							line: 1
						}
					}
					patterns: Array [
						CSSTypeSelector {
							value: "div"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 3
									line: 1
								}
								start: Object {
									column: 0
									line: 1
								}
							}
						}
					]
				}
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 14
							line: 1
						}
						start: Object {
							column: 3
							line: 1
						}
					}
					patterns: Array [
						CSSTypeSelector {
							value: "div"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 8
									line: 1
								}
								start: Object {
									column: 5
									line: 1
								}
							}
						}
						CSSCombinator {
							combinator: "nextSibiling"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 11
									line: 1
								}
								start: Object {
									column: 9
									line: 1
								}
							}
						}
						CSSIdSelector {
							value: "id"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 14
									line: 1
								}
								start: Object {
									column: 11
									line: 1
								}
							}
						}
					]
				}
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 25
							line: 1
						}
						start: Object {
							column: 14
							line: 1
						}
					}
					patterns: Array [
						CSSTypeSelector {
							value: "div"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 19
									line: 1
								}
								start: Object {
									column: 16
									line: 1
								}
							}
						}
						CSSCombinator {
							combinator: "subsequentSibiling"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 22
									line: 1
								}
								start: Object {
									column: 20
									line: 1
								}
							}
						}
						CSSIdSelector {
							value: "id"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 25
									line: 1
								}
								start: Object {
									column: 22
									line: 1
								}
							}
						}
					]
				}
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 37
							line: 1
						}
						start: Object {
							column: 25
							line: 1
						}
					}
					patterns: Array [
						CSSTypeSelector {
							value: "div"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 30
									line: 1
								}
								start: Object {
									column: 27
									line: 1
								}
							}
						}
						CSSCombinator {
							combinator: "child"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 33
									line: 1
								}
								start: Object {
									column: 31
									line: 1
								}
							}
						}
						CSSIdSelector {
							value: "id"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 36
									line: 1
								}
								start: Object {
									column: 33
									line: 1
								}
							}
						}
					]
				}
			]
		}
		CSSRule {
			loc: Object {
				filename: "selectors/input.css"
				end: Object {
					column: 1
					line: 7
				}
				start: Object {
					column: 0
					line: 5
				}
			}
			block: CSSBlock {
				value: Array []
				startingTokenValue: "{"
				loc: Object {
					filename: "selectors/input.css"
					end: Object {
						column: 1
						line: 7
					}
					start: Object {
						column: 22
						line: 5
					}
				}
			}
			prelude: Array [
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 22
							line: 5
						}
						start: Object {
							column: 0
							line: 5
						}
					}
					patterns: Array [
						CSSClassSelector {
							value: "escapedclassname"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 21
									line: 5
								}
								start: Object {
									column: 0
									line: 5
								}
							}
						}
					]
				}
			]
		}
		CSSRule {
			loc: Object {
				filename: "selectors/input.css"
				end: Object {
					column: 1
					line: 11
				}
				start: Object {
					column: 0
					line: 9
				}
			}
			block: CSSBlock {
				value: Array []
				startingTokenValue: "{"
				loc: Object {
					filename: "selectors/input.css"
					end: Object {
						column: 1
						line: 11
					}
					start: Object {
						column: 11
						line: 9
					}
				}
			}
			prelude: Array [
				CSSSelector {
					loc: Object {
						filename: "selectors/input.css"
						end: Object {
							column: 11
							line: 9
						}
						start: Object {
							column: 0
							line: 9
						}
					}
					patterns: Array [
						CSSClassSelector {
							value: "class"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 6
									line: 9
								}
								start: Object {
									column: 0
									line: 9
								}
							}
						}
						CSSCombinator {
							combinator: "nextSibiling"
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 9
									line: 9
								}
								start: Object {
									column: 7
									line: 9
								}
							}
						}
						CSSUniversalSelector {
							loc: Object {
								filename: "selectors/input.css"
								end: Object {
									column: 10
									line: 9
								}
								start: Object {
									column: 9
									line: 9
								}
							}
						}
					]
				}
			]
		}
	]
}
```
