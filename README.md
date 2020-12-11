# v 


```
const foo:string = "foo bar baz";
const v = new Validator();
const errors = v
  .addStep<string>(s => s.length > 5, "length should be greater than 5")
  .addStep<string>(s => s.includes("foo"), "should contain 'foo'")
  .validate(request);
      
const isValid = v.ok;
errors.map(console.log);
```
