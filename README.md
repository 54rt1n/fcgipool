fcgipool
=============

fork of the go internal library to create statically sized, pre-allocated fcgi pools

Go fcgi only requires the Serve method be invoked:
func Serve(l net.Listener, handler http.Handler) error

The interface has changed very little, with the Serve method changing to:
func Serve(l net.Listener, handler http.Handler, poolSize int) error

