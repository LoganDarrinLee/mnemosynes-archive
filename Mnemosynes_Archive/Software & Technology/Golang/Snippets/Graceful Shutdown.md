[Source](https://dev.to/mokiat/proper-http-shutdown-in-go-3fji)

This will finish serving all current/ongoing server requests before shutting down.

```go
import (
"os"
"os/signal"
"syscall"
)

go func() {

// Create new channel
sigChan := make(chan os.Signal, 1)

// Configure sigChan to recieve specific os specific signals
signal.Notify(sigChan, syscall.SIGINT, syscall.SIGTERM)

// Block until a signal is recieved
<-sigChan

// Hanlde server errors on close. 
if err := server.Close(); err != nil {
	log.Fatalf("HTTP close error: %v", err)
}

}()
```

More 