## Example sbt project that compiles using Dotty

### Requirements

Until artifacts are published, you'll need to compile Dotty and its compiler
bridge yourself:
```shell
git clone https://github.com/lampepfl/dotty.git
cd dotty
sbt publishLocal
cd ..

git clone https://github.com/smarter/dotty-bridge.git
cd dotty-bridge
sbt publishLocal
cd ..
```

### Usage

This is a normal sbt project, you can compile code with `sbt compile` and run it
with `sbt run`. See
https://github.com/smarter/dotty-bridge#implementation-status for what works and
what doesn't.

If compiling this example project fails, you probably have a global sbt plugin
that does not work with dotty, try to disable all plugins in `~/.sbt/0.13/plugins`.

### Discuss

Feel free to come chat with us on the
[Dotty gitter](http://gitter.im/lampepfl/dotty)!
