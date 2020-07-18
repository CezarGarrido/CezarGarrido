### Hi there 👋

```go
package profile

type Bio struct {
  Name string
}

type Stack struct {
    languages   []string
    databases   []string
    misc        []string
    ongoing     []string
}
func NewBio(name string)*Bio {
     return &Bio{name}
}
func NewStack(languages,databases,mis,ongoing []string)*Stack {
     return &Stack{languages, databases, misc, ongoing}
}
```
