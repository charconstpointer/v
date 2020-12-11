# v 
# 🦋 Fluent validator


```
const foo:string = "foo bar baz";
const v = new Validator();
const result = v
  .addStep<string>(s => s.length > 5, "length should be greater than 5")
  .addStep<string>(s => s.includes("foo"), "should contain 'foo'")
  .validate(foo);
      
const isValid = result.ok;
result.errors.map(console.log);
```
