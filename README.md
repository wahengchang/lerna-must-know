# lerna-must-know


## init
 
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
