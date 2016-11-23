# env
Package env provides a convenient way to initialize variables from the environment.

# Usage

```
// If the environment variable `abc` is empty, the default value `15` is returned.
result := env.Int("abc", 15)

println(result==15) // print `true`

// Set the environment variable
os.Setenv("abc", "25")

// Read from the environment variable
env.Parse()

println(result==25) // print `true`
```