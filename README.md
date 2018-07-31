# lerna-must-know

[`lerna`](https://github.com/lerna/lerna) is a tool that allows you to maintain multiple `npm` packages within one repository.

There's a couple of benefits to this kind of approach, the paradigm is called a `monorepo`, and more can be read about it from the [source of `babel`, and `react`](https://github.com/babel/babel/blob/master/doc/design/monorepo.md).

## Init
 
```
$ lerna init
```

## Add
Add a dependency to matched packages

```
$ lerna add module-1 --scope=module-2

// lerna add @bigear/microphone-recorder --scope=@bigear/bigear
```

## bootstrap
this links all modules in a monorepo together. This way, you can immediately test whether a change will break code that relies on a module.
 
```
$ lerna bootstrap
```

## Publish
```
// $ lerna publish --force-publish=*
```

publishing to org npm, needed to make it public on the first publish
```
$ npm publish --access=public
```


## Reference
 - [https://macwright.org/2016/07/08/lerna-npm-organizations-new-wave-modularity.html](https://macwright.org/2016/07/08/lerna-npm-organizations-new-wave-modularity.html)
 - [https://github.com/lerna/lerna](https://github.com/lerna/lerna)
 - [Sample- turf](https://github.com/Turfjs/turf)
 - [Sample-bigear](https://github.com/wahengchang/bigear)
