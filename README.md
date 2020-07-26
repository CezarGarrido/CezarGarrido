### Hi there 👋
```go
package main

import (
	"play.ground/profile"
)

func main() {
	me := profile.NewBio("Cezar G.B")
	stack := profile.NewStack(
		[]string{"Go"},
		[]string{"Postgres"},
		[]string{"Docker"},
		[]string{"Vue.js"},
	)
	_ = me
	_ = stack
}
-- go.mod --
module play.ground
-- profile/profile.go --
package profile

type Bio struct {
	Name string
}
type Stack struct {
	languages []string
	databases []string
	misc      []string
	ongoing   []string
}
func NewBio(name string) *Bio {
	return &Bio{name}
}
func NewStack(languages, databases, misc, ongoing []string) *Stack {
	return &Stack{languages, databases, misc, ongoing}
}
```
