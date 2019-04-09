# Third Part Homework
Resource: [Janke Learning Variables & Hoisting](https://github.com/janke-learning/variables-and-hoisting/blob/master/README.md)

## Swaps
* challenges
    1. [the first](https://goo.gl/k9jdZy)
    solution : [pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%22b%22,%20b%20%3D%20%22a%22%3B%0Alet%20_%20%3D%20'%20'%3B%0A%0A_%20%3D%20b%3B%0Ab%20%3D%20a%3B%0Aa%20%3D%20_%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)


    The fix:

    ```js
    let a = "b", b = "a";
    let _ = ' ';
    _ = b;
    b = a;
    a = _;
    ```
    1. [the second](https://goo.gl/KvayUU)
    solution :[pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%22c%22,%20b%20%3D%20%22a%22,%20c%20%3D%20%22b%22%3B%0Alet%20_%20%3D%20'%20'%3B%0A%0A//%20can%20be%20done%20in%204%20lines%0A_%20%3D%20c%3B%0Ac%20%3D%20a%3B%0Aa%20%3D%20b%3B%0Ab%20%3D%20_%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    The fix:

    ```js
    let a = "c", b = "a", c = "b";
    let _ = ' ';

    _ = c;
    c = a;
    a = b;
    b = _;
    ```


    1. [the third](https://goo.gl/WXXtV7)
    solution : [pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%22d%22,%20b%20%3D%20%22a%22,%20c%20%3D%20%22b%22,%20d%20%3D%20%22c%22%3B%0Alet%20_%20%3D%20'%20'%3B%0A%0A//%20can%20be%20done%20in%205%20lines%0A_%20%3D%20a%3B%0Aa%20%3D%20b%3B%0Ab%20%3D%20c%3B%0Ac%20%3D%20d%3B%0Ad%20%3D%20_%3B&curInstr=7&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    The fix:
    ```js
    let a = "d", b = "a", c = "b", d = "c";
    let _ = ' ';
    _ = a;
    a = b;
    b = c;
    c = d;
    d = _;
    ```

    1. [the fourth](https://goo.gl/nTA1DG)
    solution : [pytut]
    The fix
    1. [the fifth](https://goo.gl/gDaKNi)
    solution : [pytut]
    The fix

## Sentences
To reassign variables so that at each step of execution the variables spell out the next word in a sentence.
1. Without extra holder variables:
* challenges:
    1. [the toad reads me](https://goo.gl/imKwgj)

      solution :

    1. [eating meat every meal](https://goo.gl/cwZijk)

      solution :
    1. [many men may melt my mind](https://goo.gl/16C62t)

      solution :
    1. [if fir trees ever fall](https://goo.gl/8y5Lh2)

      solution :
2. With extra holder variables:
* challenges:
    1. [the toad reads me](https://goo.gl/4eqhLb)
    solution :
    1. [eating meat every meal](https://goo.gl/F9Njwp)
    solution :
    1. [many men may melt my mind](http://www.pythontutor.com/javascript.html#code=//%20many%20men%20may%20melt%20my%20mind%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20'%3B%0Alet%20x,%20y%3B%0A//%20--%20you%20write%20this%20--%0A%0A//%20many%0A%0A//%20men%0A%0A//%20may%0A%0A//%20melt%0A%0A//%20my%0A%0A//%20mind&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
    solution :
    1. [if fir trees ever fall](https://goo.gl/BCC6pz)
    solution :
