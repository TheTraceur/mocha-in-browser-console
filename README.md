[![npm version](https://badge.fury.io/js/mocha-in-browser-console.svg)](https://www.npmjs.com/package/mocha-in-browser-console)

[![GitHub version](https://badge.fury.io/gh/TheTraceur%2Fmocha-in-browser-console.svg)](https://github.com/TheTraceur/mocha-in-browser-console)

© by [**traceur**](https://www.npmjs.com/~traceur)

## Installation

```bash
npm install mocha-in-browser-console
```

## Usage

```html
<script src="node_modules/mocha-in-browser-console/mocha-in-browser-console.min.js"></script>
```

```js
var test = function(){
	
	var mocha = new Mocha(); // initial setup - before writing tests
	
	describe("my test suite",function(){
		
		describe("my test",function(){
			
			it("succeeds",function(){
				
				assert(true);
				
			});
			
			it("fails",function(){
				
				assert(false);
				
			});
			
		});
		
	});
	
	mocha.run();

};

test(); // can test at any time 
```

![alt tag](http://cdn.pspu.pl/mocha/mocha_test_4.png)