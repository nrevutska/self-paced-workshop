Write code to import packages:

```
import (
    "fmt"
    "net/http"
)
```

write code to handling requests:

```
func hello(w http.ResponseWriter, req *http.Request) {
   fmt.Fprintf(w, "hello\n")
}
```

now, write `main` function:

```
http.HandleFunc("/hello", hello)

http.ListenAndServe(":80", nil)
```
