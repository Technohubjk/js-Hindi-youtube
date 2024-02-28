// Write a function createCounter. It should accept an initial integer init. It should return an object with three functions.

// The three functions are:

// increment() increases the current value by 1 and then returns it.
// decrement() reduces the current value by 1 and then returns it.
// reset() sets the current value to init and then returns it.

/**
 * @param {integer} init
 * @return { increment: Function, decrement: Function, reset: Function }
 */
var createCounter = function(init) {
    let a=init;
    return{
        increment:function(init){
            a++;
            return a;
        }, 
        decrement:function(){
            a--;
            return a;
        },
        reset:function() {
            a=init;
            return a;
        }

        }
    }
let a = createCounter(10)
console.log(a.increment()) // Outputs 11 - Increments the count by 1
console.log(a.decrement()) // Outputs 10 - Decrements the count by 1
console.log(a.reset())         // Resets the count back to 1
/**
 * const counter = createCounter(5)
 * counter.increment(); // 6
 * counter.reset(); // 5
 * counter.decrement(); // 4
 */ 
