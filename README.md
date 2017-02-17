
© by [**traceur**](https://www.npmjs.com/~traceur)

## Installation

```bash
npm install -g mocha-in-browser-console
```

## Usage

```html
<script src="https://cdn.rawgit.com/TheTraceur/mocha-in-browser-console/master/mocha-in-browser-console.min.js"></script>
```

```js
var test = function(){
	
	var mocha = new Mocha();
	
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