# Lab 01 – Event Model Trace

## Console Trace

The console output appeared in this order:

1. `A-sync`
2. `E-sync`
3. `B-click`
4. `D-microtask`
5. `C-timeout`

## Observation

The synchronous statements `A-sync` and `E-sync` execute first when the page loads. After clicking the button, the click event handler executes and prints `B-click`. The Promise callback runs next because Promise callbacks are microtasks. The `setTimeout()` callback runs after the microtask because it is a macrotask.

## Conclusion

The trace shows that JavaScript executes synchronous code first, followed by microtasks such as `Promise.then()`, and then macrotasks such as `setTimeout()`.
