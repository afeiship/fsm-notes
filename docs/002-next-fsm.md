# next-fsm


## plan
```js
var fsm = new nx.Fsm({
  state: false,
  transitions:[
    { name: 'on', from: false, to: true },
    { name: 'off', from: false, to: true }
  ],
  onTransition: function(inEvent){
    const { value } = inEvent.target;
    console.log('current state:', value);
    // this.setState({ value: currentState })
  }
});


fsm.on();
fsm.off();
fsm.transition('on');
```


## resources
- https://www.cnblogs.com/p2227/p/javascript-finite-state-machine-application.html
- http://gh.p2227.com/demo/fsm/
