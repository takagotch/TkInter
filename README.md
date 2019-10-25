### tkinter
---
https://github.com/python/cpython/tree/master/Lib/tkinter

https://wiki.python.org/moin/TkInter

```py
// tkinter/test/test_tkinter/test_loadtk.py

class TkLoadTest(unittest.TestCase):

  @unittest.skipIf('DISPLAY' not in os.environ, 'No $DISPLAY set.')
  def testLoadTk(self):
    tcl = Tcl()
    self.assertRaises(TclError,tcl.winfo_geometry)
    tcl.loadtk()
    self.assertEqual('1x1+0+0', tcl.winfo_geometry())
    tcl.destroy()
  
  def testLoadTkFailure(self):
    old_display = None
    if sys.platform.startswith(('win', 'darwin', 'cygwin')):


```

```
```

```
```


