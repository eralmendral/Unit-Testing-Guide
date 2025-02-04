### Using Jasmine Framework
> Behavior Driven JavaScript
> Karma Test Runner
> Jasmine is a JavaScript testing framework, and Karma is a test runner that executes Jasmine tests. They are often used together to perform unit tests in Angular. 

### Syntax
- describe
- it 


### Example
```JavaScript
  describe('Calculate', () => {
    it('should add two numbers', () => {
    
	pending();

  }) 

 })
 
```


### Jasmine Spy
 - Simulate a function
 - Create a mock function instead of creating instance of the service.


### Example
```JavaScript
  it('should add two numbers', () => {
 	const logger = jasmine.spyOn('', ['log'])
	const calculator = new CalculatorService(logger)
	const result = calculator.add(1,2);
	
	expect(result).toBe(3);
	expect(logger.log).toHaveBeenCallTimes(1)

 })
```

### Structuring Angular Unit Tests
 - Test Setup
 - beforeEach

### Using Dependency Injection
 - Dependency Injection - design pattern widely used by Angular Framework. Means some components or service might depends from other services.
- TestBed - provide fake implementations of some of the internal services.

``
