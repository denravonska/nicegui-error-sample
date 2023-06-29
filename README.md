Small example that triggers an error when trying to invoke nicegui via a module.
Standalone works:
```
$ cd nicegui-error-sample/sample/
$ python __main__.py 

NiceGUI ready to go on http://localhost:8080, and http://127.0.1.1:8080
Opening in existing browser session.
```

Running as module doesn't:
```
$ cd nicegui-error-sample
$ python -m sample

You must call ui.run() to start the server.
If ui.run() is behind a main guard
   if __name__ == "__main__":
remove the guard or replace it with
   if __name__ in {"__main__", "__mp_main__"}:
to allow for multiprocessing.

ERROR:    Application startup failed. Exiting.
```
