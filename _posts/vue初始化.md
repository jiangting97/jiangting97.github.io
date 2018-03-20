init.js

主要负责初始化：
 initLifecycle(vm)

    initEvents(vm)
    initRender(vm)
    callHook(vm, 'beforeCreate')
    initInjections(vm) // resolve injections before data/props
    initState(vm)
    initProvide(vm) // resolve provide after data/props
    callHook(vm, 'created')


initInjections:初始化数据

observer
dep：用来存放观察