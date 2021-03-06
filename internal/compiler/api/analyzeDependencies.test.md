# `analyzeDependencies.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/compiler/api/analyzeDependencies.test.ts --update-snapshots` to update.

## `correctly identifies a file with cjs exports as cjs`

```javascript
Object {
	dependencies: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	exports: Array [
		local {
			kind: "value"
			name: "foo"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 19
					line: 1
				}
				start: Object {
					column: 14
					line: 1
				}
			}
		}
	]
	diagnostics: Array [
		Object {
			tags: undefined
			origins: Array [Object {category: "analyzeDependencies"}]
			location: Object {
				filename: "unknown"
				integrity: undefined
				language: "js"
				marker: undefined
				sourceTypeJS: "module"
				end: Object {
					column: 19
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			description: Object {
				category: "analyzeDependencies/cjsExportInES"
				message: RAW_MARKUP {value: "You cannot use CommonJS exports in an ES module"}
				advice: Array [
					action {
						command: "check"
						extra: undefined
						hidden: true
						shortcut: "s"
						args: Array ["unknown"]
						commandFlags: Object {decisions: Array ["suppress-analyzeDependencies/cjsExportInES-unknown-1"]}
						instruction: RAW_MARKUP {value: "To suppress this error run"}
						noun: RAW_MARKUP {value: "Add suppression comment"}
					}
					action {
						args: Array []
						command: "check"
						extra: true
						hidden: true
						shortcut: undefined
						commandFlags: Object {decisions: Array ["global-suppress-analyzeDependencies/cjsExportInES"]}
						instruction: RAW_MARKUP {value: "To add suppression comments for ALL files with this category run"}
						noun: RAW_MARKUP {value: "Add suppression comments for ALL files with this category"}
					}
				]
			}
		}
	]
}
```

## `correctly identifies a file with es exports as es`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		foo: Object {
			filename: "unknown"
			identifierName: "foo"
			end: Object {
				column: 16
				line: 1
			}
			start: Object {
				column: 13
				line: 1
			}
		}
	}
	exports: Array [
		local {
			kind: "value"
			name: "foo"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "foo"
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 13
					line: 1
				}
			}
		}
	]
}
```

## `correctly identifies a file with es imports as es`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "bar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 12
					line: 1
				}
				start: Object {
					column: 7
					line: 1
				}
			}
		}
	]
}
```

## `correctly identifies a file with no imports or exports as unknown`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
}
```

## `defines topLevelLocalBindings`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		bar: Object {
			filename: "unknown"
			identifierName: "bar"
			end: Object {
				column: 11
				line: 1
			}
			start: Object {
				column: 8
				line: 1
			}
		}
		foo: Object {
			filename: "unknown"
			identifierName: "foo"
			end: Object {
				column: 9
				line: 2
			}
			start: Object {
				column: 6
				line: 2
			}
		}
	}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			optional: false
			source: "foo"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 23
					line: 1
				}
				start: Object {
					column: 18
					line: 1
				}
			}
			names: Array [
				value {
					name: "bar"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 11
							line: 1
						}
						start: Object {
							column: 8
							line: 1
						}
					}
				}
			]
		}
	]
}
```

## `disallow mix of es and cjs exports`

```javascript
Object {
	dependencies: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "cjs"
	topLevelLocalBindings: Object {
		foo: Object {
			filename: "unknown"
			identifierName: "foo"
			end: Object {
				column: 16
				line: 1
			}
			start: Object {
				column: 13
				line: 1
			}
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse"}]
			location: Object {
				filename: "unknown"
				integrity: undefined
				language: "js"
				sourceText: undefined
				end: Object {
					column: 25
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			description: Object {
				category: "parse"
				categoryValue: "js"
				message: RAW_MARKUP {value: "<emphasis>import</emphasis> and <emphasis>export</emphasis> can only appear in a module"}
				advice: Array [
					log {
						category: "info"
						text: RAW_MARKUP {value: "Change the extension to <emphasis>.mjs</emphasis> to turn this file into a module"}
					}
					log {
						category: "info"
						text: Array [
							RAW_MARKUP {value: "Add <emphasis>\"type\": \"module\"</emphasis> to your <filelink emphasis target=\""}
							"package.json"
							RAW_MARKUP {value: "\" />"}
						]
					}
				]
			}
		}
	]
	exports: Array [
		local {
			kind: "value"
			name: "foo"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "foo"
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 13
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "bar"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 19
					line: 2
				}
				start: Object {
					column: 14
					line: 2
				}
			}
		}
		local {
			kind: "value"
			name: "default"
			loc: undefined
			valueType: "other"
		}
	]
}
```

## `discovers async import('foo')`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		yes: Object {
			filename: "unknown"
			identifierName: "yes"
			end: Object {
				column: 12
				line: 3
			}
			start: Object {
				column: 9
				line: 3
			}
		}
	}
	dependencies: Array [
		es {
			kind: "value"
			all: true
			async: true
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "./foo"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 14
					line: 1
				}
				start: Object {
					column: 7
					line: 1
				}
			}
		}
		es {
			kind: "value"
			all: true
			async: true
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "./bar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 16
					line: 4
				}
				start: Object {
					column: 9
					line: 4
				}
			}
		}
	]
}
```

## `discovers commonjs exports`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "cjs"
	topLevelLocalBindings: Object {}
	exports: Array [
		local {
			kind: "value"
			name: "yes"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 27
					line: 1
				}
				start: Object {
					column: 14
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "default"
			loc: undefined
			valueType: "other"
		}
	]
}
```

## `discovers commonjs module.exports`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "cjs"
	topLevelLocalBindings: Object {}
	exports: Array [
		local {
			kind: "value"
			name: "default"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 30
					line: 1
				}
				start: Object {
					column: 17
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "default"
			loc: undefined
			valueType: "other"
		}
	]
}
```

## `discovers export declarations`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		Bar: Object {
			filename: "unknown"
			identifierName: "Bar"
			end: Object {
				column: 16
				line: 3
			}
			start: Object {
				column: 13
				line: 3
			}
		}
		foo: Object {
			filename: "unknown"
			identifierName: "foo"
			end: Object {
				column: 19
				line: 2
			}
			start: Object {
				column: 16
				line: 2
			}
		}
		yes: Object {
			filename: "unknown"
			identifierName: "yes"
			end: Object {
				column: 16
				line: 1
			}
			start: Object {
				column: 13
				line: 1
			}
		}
	}
	exports: Array [
		local {
			kind: "value"
			name: "yes"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "yes"
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 13
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "foo"
			valueType: "function"
			loc: Object {
				filename: "unknown"
				identifierName: "foo"
				end: Object {
					column: 19
					line: 2
				}
				start: Object {
					column: 16
					line: 2
				}
			}
		}
		local {
			kind: "value"
			name: "Bar"
			valueType: "class"
			loc: Object {
				filename: "unknown"
				identifierName: "Bar"
				end: Object {
					column: 16
					line: 3
				}
				start: Object {
					column: 13
					line: 3
				}
			}
		}
	]
}
```

## `discovers export default`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	exports: Array [
		local {
			kind: "value"
			name: "default"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 20
					line: 1
				}
				start: Object {
					column: 15
					line: 1
				}
			}
		}
	]
}
```

## `discovers export from`

```javascript
Object {
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	exports: Array [
		external {
			kind: "value"
			exported: "foo"
			imported: "foo"
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 11
					line: 1
				}
				start: Object {
					column: 8
					line: 1
				}
			}
		}
		external {
			kind: "value"
			exported: "bar"
			imported: "bar"
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 13
					line: 1
				}
			}
		}
		external {
			kind: "value"
			exported: "no"
			imported: "default"
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 31
					line: 1
				}
				start: Object {
					column: 18
					line: 1
				}
			}
		}
		external {
			kind: "value"
			exported: "noo"
			imported: "boo"
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 43
					line: 1
				}
				start: Object {
					column: 33
					line: 1
				}
			}
		}
	]
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: true
			imported: false
			optional: false
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 58
					line: 1
				}
				start: Object {
					column: 50
					line: 1
				}
			}
			names: Array [
				value {
					name: "foo"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 11
							line: 1
						}
						start: Object {
							column: 8
							line: 1
						}
					}
				}
				value {
					name: "bar"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 16
							line: 1
						}
						start: Object {
							column: 13
							line: 1
						}
					}
				}
				value {
					name: "default"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 31
							line: 1
						}
						start: Object {
							column: 18
							line: 1
						}
					}
				}
				value {
					name: "boo"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 43
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
```

## `discovers export star`

```javascript
Object {
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	exports: Array [
		externalAll {
			kind: "value"
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 23
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
		}
	]
	dependencies: Array [
		es {
			kind: "value"
			all: true
			async: false
			exported: true
			imported: false
			names: Array []
			optional: false
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 22
					line: 1
				}
				start: Object {
					column: 14
					line: 1
				}
			}
		}
	]
}
```

## `discovers import default`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		bar: Object {
			filename: "unknown"
			identifierName: "bar"
			end: Object {
				column: 10
				line: 1
			}
			start: Object {
				column: 7
				line: 1
			}
		}
	}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			optional: false
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 24
					line: 1
				}
				start: Object {
					column: 16
					line: 1
				}
			}
			names: Array [
				value {
					name: "default"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 10
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
	]
}
```

## `discovers import specifiers`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		bar: Object {
			filename: "unknown"
			identifierName: "bar"
			end: Object {
				column: 11
				line: 1
			}
			start: Object {
				column: 8
				line: 1
			}
		}
		foo: Object {
			filename: "unknown"
			identifierName: "foo"
			end: Object {
				column: 16
				line: 1
			}
			start: Object {
				column: 13
				line: 1
			}
		}
		lol: Object {
			filename: "unknown"
			identifierName: "lol"
			end: Object {
				column: 32
				line: 1
			}
			start: Object {
				column: 29
				line: 1
			}
		}
		to: Object {
			filename: "unknown"
			identifierName: "to"
			end: Object {
				column: 42
				line: 1
			}
			start: Object {
				column: 40
				line: 1
			}
		}
	}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			optional: false
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 57
					line: 1
				}
				start: Object {
					column: 49
					line: 1
				}
			}
			names: Array [
				value {
					name: "bar"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 11
							line: 1
						}
						start: Object {
							column: 8
							line: 1
						}
					}
				}
				value {
					name: "foo"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 16
							line: 1
						}
						start: Object {
							column: 13
							line: 1
						}
					}
				}
				value {
					name: "default"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 32
							line: 1
						}
						start: Object {
							column: 18
							line: 1
						}
					}
				}
				value {
					name: "ya"
					loc: Object {
						filename: "unknown"
						end: Object {
							column: 42
							line: 1
						}
						start: Object {
							column: 34
							line: 1
						}
					}
				}
			]
		}
	]
}
```

## `discovers import star`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "foobar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 29
					line: 1
				}
				start: Object {
					column: 21
					line: 1
				}
			}
		}
	]
}
```

## `discovers local export specifiers`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	exports: Array [
		local {
			kind: "value"
			name: "foo"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "foo"
				end: Object {
					column: 11
					line: 1
				}
				start: Object {
					column: 8
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "bar"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "bar"
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 13
					line: 1
				}
			}
		}
		local {
			kind: "value"
			name: "no"
			valueType: "other"
			loc: Object {
				filename: "unknown"
				identifierName: "yes"
				end: Object {
					column: 21
					line: 1
				}
				start: Object {
					column: 18
					line: 1
				}
			}
		}
	]
}
```

## `discovers require('module') call`

```javascript
Object {
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {
		yeah: Object {
			filename: "unknown"
			identifierName: "yeah"
			end: Object {
				column: 13
				line: 3
			}
			start: Object {
				column: 9
				line: 3
			}
		}
	}
	dependencies: Array [
		es {
			kind: "value"
			all: false
			async: false
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "foo"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 26
					line: 1
				}
				start: Object {
					column: 21
					line: 1
				}
			}
		}
		cjs {
			kind: "value"
			all: true
			async: false
			exported: false
			imported: true
			names: Array []
			optional: false
			source: "bar"
			loc: Object {
				filename: "unknown"
				end: Object {
					column: 16
					line: 4
				}
				start: Object {
					column: 2
					line: 4
				}
			}
		}
	]
}
```

## `discovers top level await`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	exports: Array []
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
	firstTopAwaitLocation: Object {
		filename: "unknown"
		end: Object {
			column: 14
			line: 1
		}
		start: Object {
			column: 0
			line: 1
		}
	}
}
```

## `ignores require() call if shadowed`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "cjs"
	exports: Array [
		local {
			kind: "value"
			name: "default"
			loc: undefined
			valueType: "other"
		}
	]
	topLevelLocalBindings: Object {
		yes: Object {
			filename: "unknown"
			identifierName: "yes"
			end: Object {
				column: 12
				line: 6
			}
			start: Object {
				column: 9
				line: 6
			}
		}
	}
}
```

## `ignores require(dynamic) call`

```javascript
Object {
	dependencies: Array []
	diagnostics: Array []
	exports: Array []
	firstTopAwaitLocation: undefined
	importFirstUsage: Array []
	moduleType: "es"
	topLevelLocalBindings: Object {}
}
```
