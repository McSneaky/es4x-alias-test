Installed GraalVM from and followed this: https://www.graalvm.org/docs/getting-started/

Added all required variables to path

`which node` returns with /home/mcsneaky/GraalVM/bin

Installed es4x-pm like shown in here: https://github.com/reactiverse/es4x#usage

Tried to run index.js but alias does not work, throws error:

```
ModuleError: Module "stream" was not found
        at <js> Require.resolve(file:/home/mcsneaky/Projects/McSneaky/es4x-alias-test/node_modules/.lib/es4x-0.10.0.jar!/io/reactiverse/es4x/jvm-npm.js:165:5324-5402)
        at <js> Require(file:/home/mcsneaky/Projects/McSneaky/es4x-alias-test/node_modules/.lib/es4x-0.10.0.jar!/io/reactiverse/es4x/jvm-npm.js:132:4365-4391)
        at <js> this.require(file:/home/mcsneaky/Projects/McSneaky/es4x-alias-test/node_modules/.lib/es4x-0.10.0.jar!/io/reactiverse/es4x/jvm-npm.js:46:1459-1475)
        at <js> :anonymous(/home/mcsneaky/Projects/McSneaky/es4x-alias-test/index.js:1:77-93)
        at <js> _load(file:/home/mcsneaky/Projects/McSneaky/es4x-alias-test/node_modules/.lib/es4x-0.10.0.jar!/io/reactiverse/es4x/jvm-npm.js:97:3264-3345)
        at <js> runMain(file:/home/mcsneaky/Projects/McSneaky/es4x-alias-test/node_modules/.lib/es4x-0.10.0.jar!/io/reactiverse/es4x/jvm-npm.js:110:3648-3692)
        at org.graalvm.sdk/org.graalvm.polyglot.Value.invokeMember(Value.java:459)
        at io.reactiverse.es4x.impl.JSVerticleFactory$1.start(JSVerticleFactory.java:81)
        at io.vertx.core.Verticle.start(Verticle.java:66)
        at io.vertx.core.impl.DeploymentManager.lambda$doDeploy$9(DeploymentManager.java:556)
        at io.vertx.core.impl.ContextImpl.executeTask(ContextImpl.java:369)
        at io.vertx.core.impl.EventLoopContext.lambda$executeAsync$0(EventLoopContext.java:38)
        at io.netty.util.concurrent.AbstractEventExecutor.safeExecute(AbstractEventExecutor.java:163)
        at io.netty.util.concurrent.SingleThreadEventExecutor.runAllTasks(SingleThreadEventExecutor.java:510)
        at io.netty.channel.nio.NioEventLoop.run(NioEventLoop.java:518)
        at io.netty.util.concurrent.SingleThreadEventExecutor$6.run(SingleThreadEventExecutor.java:1044)
        at io.netty.util.internal.ThreadExecutorMap$2.run(ThreadExecutorMap.java:74)
        at io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
        at java.base/java.lang.Thread.run(Thread.java:834)
```