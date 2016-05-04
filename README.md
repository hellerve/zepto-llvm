# llvm-zepto

This is a silly compiler that transforms a tiny subset of zepto
into LLVM IR and compiles it into machine code.

## Usage

For an example, look no further than into the `examples` directory.

```bash
zepto main.zp examples/add.zp add
./add
echo $? # should print 3
```

We just added 1 and 2 natively! Yay!

## Caveats

This compiler is far from zepto compliant. Specifically, it compiles a subset
of zepto that only works with integers, has no closures, lambdas or the like
and has only functions as top-level definitions. Oh yeah, also it requires a
main function.

What I want to say is: it's not useful.

<hr/>

Have fun!
