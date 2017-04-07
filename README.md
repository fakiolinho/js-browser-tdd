# js-browser-tdd

Setup a fast TDD env on browser with mocha and chai.

## Installation

```bash
git clone https://github.com/fakiolinho/js-browser-tdd.git
npm i && npm start
```

## Tested Method

Function to test if a number is prime:

```javascript
function isPrime(x) {
	if (! Number.isInteger(x)) {
	  	return false;
	}
	    
	if (x < 2) {
	  	return false;
	}
	    
	for (let i = 2; i <= Math.sqrt(x); i++) {
	  	if (x % i === 0) {
	    	return false;
	  	}
	}
	    
	return true;
}
```