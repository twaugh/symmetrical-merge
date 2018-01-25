History of the `foo` function:
```
$ git log -L:foo:xyzzy.c
commit 5e131bd43320245429eb291dc2873a84c1aeac5f
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:42:56 2017 +0100

    update foo again

diff --git a/xyzzy.c b/xyzzy.c
--- a/xyzzy.c
+++ b/xyzzy.c
@@ -3,6 +3,6 @@
 int foo(int x)
 {
-  x += 25;
+  x += 30;
   return x;
 }
 

commit 26268ab266262fa25438deeb8f662f14a0d48186
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:38:30 2017 +0100

    merge together


commit d3ec071b0b424d202208185d49e1da44798a9cd3
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:36:16 2017 +0100

    modify foo

diff --git a/foo.c b/foo.c
--- a/foo.c
+++ b/foo.c
@@ -3,5 +3,5 @@
 int foo(int x)
 {
-  x += 20;
+  x += 25;
   return x;
 }

commit 5f71c28c94ea6af8de370f62b0e3c1ec289cb0ae
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:35:51 2017 +0100

    initial commit

diff --git a/foo.c b/foo.c
--- /dev/null
+++ b/foo.c
@@ -0,0 +3,5 @@
+int foo(int x)
+{
+  x += 20;
+  return x;
+}
```

History of the `bar` function:
```
$ git log -L:bar:xyzzy.c
commit 8e46eb47057f4fedf3ac19c7228f3bb09145e15d (HEAD -> master, origin/master, origin/HEAD)
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:43:07 2017 +0100

    update bar again

diff --git a/xyzzy.c b/xyzzy.c
--- a/xyzzy.c
+++ b/xyzzy.c
@@ -9,4 +9,4 @@
 int bar(int x)
 {
-  return logn(x, 10);
+  return floor(logn(x, 10));
 }

commit b0d6fad373e9ea1e72a320fd445ad9e26b61d956
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:36:26 2017 +0100

    modify bar

diff --git a/bar.c b/bar.c
--- a/bar.c
+++ b/bar.c
@@ -3,4 +3,4 @@
 int bar(int x)
 {
-  return log(x);
+  return logn(x, 10);
 }

commit 5f71c28c94ea6af8de370f62b0e3c1ec289cb0ae
Author: Tim Waugh <twaugh@redhat.com>
Date:   Wed May 10 16:35:51 2017 +0100

    initial commit

diff --git a/bar.c b/bar.c
--- /dev/null
+++ b/bar.c
@@ -0,0 +3,4 @@
+int bar(int x)
+{
+  return log(x);
+}
```
