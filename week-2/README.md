# Week 2

|  | your Emoji | your comments | coach emoji | coach comments |
| --- | --- | --- | --- | --- |
| :seedling: __[fcc: finish js basics](./fcc-basic-js-pt-2.md) | :white_check_mark: :question: | What is the function of Radix in [105.parseInt Function](https://github.com/prgrmfl/javascript-1-homework/blob/master/week-2/fcc-basic-js-pt-2.md#105-use-the-parseint-function-with-a-radix-) | :green_heart: | [radix](https://en.wikipedia.org/wiki/Radix), a math thing. not central to JS |
| :dash: __[janke: tracing conditionals](./js-tracing-conditionals.md) | | | | |
| :seedling: __[javascript.info: loops](./jsinfo-loops.md) | :white_check_mark: | | :green_heart: | |
| :dash: __[janke: loop refactors](./jl-loop-refactors.md) | | | | |
| :seedling: __[fcc: data structures](./fcc-data-structures.md) | :white_check_mark: but :question: | Why is this being true in [this exercise](http://pythontutor.com/live.html#code=let%20users%20%3D%20%7B%0A%20%20Alan%3A%20%7B%0A%20%20%20%20age%3A%2027,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Jeff%3A%20%7B%0A%20%20%20%20age%3A%2032,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Sarah%3A%20%7B%0A%20%20%20%20age%3A%2048,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Ryan%3A%20%7B%0A%20%20%20%20age%3A%2019,%0A%20%20%20%20online%3A%20true%0A%20%20%7D%0A%7D%3B%0A%0Afunction%20isEveryoneHere%28obj%29%20%7B%0A%20%20if%28obj.hasOwnProperty%28'Alan',%20'Kamil',%20'Jeff',%20'Sarah',%20'Ryan'%29%29%20%7B%0A%20%20%20%20return%20true%3B%0A%20%20%7D%0A%20%20return%20false%3B%20%20%0A%7D%0A%0Aconsole.log%28isEveryoneHere%28users%29%29%3B%20//true&cumulative=false&curInstr=6&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false) about "17. Check if an Object has a Property", although in 'if' statement  there is one property 'Kamil' which doesn't belong to the object [=](http://pythontutor.com/live.html#code=let%20users%20%3D%20%7B%0A%20%20Alan%3A%20%7B%0A%20%20%20%20age%3A%2027,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Jeff%3A%20%7B%0A%20%20%20%20age%3A%2032,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Sarah%3A%20%7B%0A%20%20%20%20age%3A%2048,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Ryan%3A%20%7B%0A%20%20%20%20age%3A%2019,%0A%20%20%20%20online%3A%20true%0A%20%20%7D%0A%7D%3B%0A%0Afunction%20isEveryoneHere%28obj%29%20%7B%0A%20%20const%20arr%20%3D%20%5B%5D%3B%0A%20%20const%20names%20%3D%20%5B'Alan',%20'Kamil',%20'Jeff',%20'Sarah',%20'Ryan'%5D%3B%0A%20%20for%20%28let%20item%20of%20names%29%20%7B%0A%20%20%20%20arr.push%28obj.hasOwnProperty%28item%29%29%0A%20%20%7D%0A%20%20return%20arr%3B%0A%7D%0A%0Aconsole.log%28isEveryoneHere%28users%29%29%3B%20//true&cumulative=false&curInstr=20&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false) | :green_heart: | [the solution from in class](http://pythontutor.com/live.html#code=let%20users%20%3D%20%7B%0A%20%20Alan%3A%20%7B%0A%20%20%20%20age%3A%2027,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Jeff%3A%20%7B%0A%20%20%20%20age%3A%2032,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Sarah%3A%20%7B%0A%20%20%20%20age%3A%2048,%0A%20%20%20%20online%3A%20true%0A%20%20%7D,%0A%20%20Ryan%3A%20%7B%0A%20%20%20%20age%3A%2019,%0A%20%20%20%20online%3A%20true%0A%20%20%7D%0A%7D%3B%0A%0Afunction%20isEveryoneHere%28obj%29%20%7B%0A%20%20const%20arr%20%3D%20%5B%5D%3B%0A%20%20const%20names%20%3D%20%5B'Alan',%20'Kamil',%20'Jeff',%20'Sarah',%20'Ryan'%5D%3B%0A%20%20for%20%28let%20item%20of%20names%29%20%7B%0A%20%20%20%20arr.push%28obj.hasOwnProperty%28item%29%29%0A%20%20%7D%0A%20%20return%20arr%3B%0A%7D%0A%0Aconsole.log%28isEveryoneHere%28users%29%29%3B%20//true&cumulative=false&curInstr=20&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false) |
| :seedling: __[janke: errors const](./jl-errors-const.md) | :white_check_mark: | | :white_check_mark: | |
| :seedling: __[janke: errors arrays](./jl-errors-arrays.md) | :white_check_mark:  | | :white_check_mark: | |
| :seedling: __[janke: errors objects](./jl-errors-objects.md) | :white_check_mark:  | | :white_check_mark: | |
| :seedling: __[javascript.info: objects](./jsinfo-objects.md) | :white_check_mark:  | | :white_check_mark: | |
| :dash: __[janke: reference types](./jl-reference-types.md) | | | | |
| :fire: __[janke: ref-type arguments](./jl-functions-ref-type-args.md) | | | | |
| :dash: __[janke: sentences w/o temps](./jl-variables-sentences-1.md) | | | | |
| :fire: __[janke: sentences w/ temps](./jl-variables-sentences-2.md) | | | | |



---


## submission instructions

| emoji | who uses it | meaning |
| --- | --- | --- |
|  :wavy_dash: | student | started, in progress  | 
| :question: | student | need help (after asking your fellow students!) | 
| :white_check_mark: | student | you think it's done, check please! | 
| :white_check_mark: | coaches | homework is checked and OK |
| :warning: | coaches | homework has a few issues, see comments and keep in touch on a new issue |
| :shipit: | coaches | there's an answer to your question, in the comments and/or an issue  | 
| :star2: | coaches | you did something awesome |

---

## priority guide

* :seedling: : must finish
* :dash: : start it
* :fire: : challenge

___
___
### <a href="https://hackyourfuture.be" target="_blank"><img src="https://pbs.twimg.com/profile_images/984474625009741824/Bs_qKx6-_400x400.jpg" width="100" height="100"></img></a>
