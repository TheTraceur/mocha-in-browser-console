
© by [**traceur**](https://www.npmjs.com/~traceur)

## Installation

```bash
npm install mocha-in-browser-console
```

## Usage

```html
<script src="./mocha-in-browser-console.min.js"></script>
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