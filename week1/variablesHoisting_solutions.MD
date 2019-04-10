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
    solution : [pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%22z%22,%20b%20%3D%20%22y%22,%20c%20%3D%20%22x%22,%20d%20%3D%20%22w%22%3B%0Alet%20_%20%3D%20'%20'%3B%0A%0A//%20can%20be%20done%20in%206%20lines%0A//wxyz%0A_%20%3D%20a%3B%20//z%0Aa%20%3D%20d%3B%20//w%0Ad%20%3D%20_%3B%20//z%0A_%20%3D%20b%3B%20//y%0Ab%20%3D%20c%3B%20//x%0Ac%20%3D%20_%3B%20//y%0A%0A&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)


    The fix
    ```js
    let a = "z", b = "y", c = "x", d = "w";
    let _ = ' ';
    //wxyz
    _ = a; //z
    a = d; //w
    d = _; //z
    _ = b; //y
    b = c; //x
    c = _; //y
    ```
    1. [the fifth](https://goo.gl/gDaKNi)

    solution : [pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%22z%22,%20b%20%3D%20%22y%22,%20c%20%3D%20%22x%22,%20d%20%3D%20%22w%22,%20e%20%3D%20%22v%22%3B%0Alet%20_%20%3D%20'%20'%3B%0A%0A//%20can%20be%20done%20in%206%20lines%0A//%20vwxyz%0A_%20%3D%20a%3B%20//z%0Aa%20%3D%20e%3B%20//v%0Ae%20%3D%20_%3B%20//z%0A_%20%3D%20b%3B%20//y%0Ab%20%3D%20d%3B%20//w%0Ad%20%3D%20_%3B%20//y%0A%0A%0A&curInstr=8&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    The fix
    ```js
    let a = "z", b = "y", c = "x", d = "w", e = "v";
    let _ = ' ';

    // vwxyz
    _ = a; //z
    a = e; //v
    e = _; //z
    _ = b; //y
    b = d; //w
    d = _; //y
    ```

## Sentences
To reassign variables so that at each step of execution the variables spell out the next word in a sentence.
1. Without extra holder variables:
* challenges:

    1. [the toad reads me](https://goo.gl/imKwgj)

    solution: [pytut](http://www.pythontutor.com/javascript.html#code=//%20the%20toad%20reads%20me%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20%22%20%22,%20_2%20%3D%20%22%20%22,%20_3%20%3D%20%22%20%22,%20_4%20%3D%20%22%20%22,%20_5%20%3D%20%22%20%22%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20the%0A_1%20%3D%20%22t%22,%20_2%20%3D%20%22h%22,%20_3%20%3D%20%22e%22%3B%0A%0A//%20toad%0A_2%20%3D%20%22o%22,%20_3%20%3D%20%22a%22,%20_4%20%3D%20%22d%22%3B%0A%0A//%20reads%0A_1%20%3D%20%22r%22,%20_2%20%3D%20%22e%22,%20_5%20%3D%20%22s%22%3B%0A%0A//%20me%0A_1%20%3D%20%22m%22,%20_3%20%3D%20%22%20%22,%20_4%20%3D%20%22%20%22,%20_5%20%3D%20%22%20%22%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    ```js
    let _1 = " ", _2 = " ", _3 = " ", _4 = " ", _5 = " ";
    // the
    _1 = "t", _2 = "h", _3 = "e";
    // toad
    _2 = "o", _3 = "a", _4 = "d";
    // reads
    _1 = "r", _2 = "e", _5 = "s";
    // me
    _1 = "m", _3 = " ", _4 = " ", _5 = " ";
    ```

    1. [eating meat every meal](https://goo.gl/cwZijk)


    solution : [pytut](http://www.pythontutor.com/javascript.html#code=//%20eating%20meat%20every%20meal%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20',%20_6%3D%20'%20'%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20eating%0A_1%20%3D%20%22e%22%20,%20_2%20%3D%20%22a%22%20,%20_3%20%3D%20%22t%22%20,%20_4%20%3D%20%22i%22%20,%20_5%20%3D%20%22n%22%20,%20_6%20%3D%20%22g%22%3B%0A//%20meat%0A%20_4%20%3D%20_3%20,%20_3%20%3D%20_2%20,%20_2%20%3D%20_1,%20_1%20%3D%20%22m%22%20,%20_5%20%3D%20%22%20%22%20,%20_6%20%3D%20%22%20%22%3B%0A//%20every%0A_1%20%3D%20_2,%20_2%20%3D%20%22v%22%20,%20_3%20%3D%20_1%20,%20_4%20%3D%20%22r%22,%20_5%20%3D%20%22y%22%20,%20_6%20%3D%20%22%20%22%3B%0A%0A//%20meal%0A_2%20%3D%20_1%20,%20_1%20%3D%20%22m%22,%20_3%20%3D%20%22a%22,%20_4%20%3D%20%22l%22,%20_5%20%3D%20%22%20%22%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)



    ```js
        // eating
        _1 = "e" , _2 = "a" , _3 = "t" , _4 = "i" , _5 = "n" , _6 = "g";
        // meat
        _4 = _3 , _3 = _2 , _2 = _1, _1 = "m" , _5 = " " , _6 = " ";
        // every
        _1 = _2, _2 = "v" , _3 = _1 , _4 = "r", _5 = "y" , _6 = " ";
        // meal
        _2 = _1 , _1 = "m", _3 = "a", _4 = "l", _5 = " ";
    ```

    1. [many men may melt my mind](https://goo.gl/16C62t)

    solution : [pytut](http://www.pythontutor.com/javascript.html#code=//%20many%20men%20may%20melt%20my%20mind%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20'%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20many%0A_1%20%3D%20%22m%22%20,%20_2%20%3D%20%22a%22,%20_3%20%3D%20%22n%22%20,%20_4%20%3D%20%22y%22%3B%0A//%20men%0A_2%20%3D%20%22e%22,%20_3%20%3D%20%22n%22%20,%20_4%20%3D%20%22%20%22%3B%0A//%20may%0A_2%20%3D%20%22a%22,%20_3%20%3D%20%22y%22%20,%20_4%20%3D%20%22%20%22%3B%0A%0A//%20melt%0A_2%20%3D%20%22e%22,%20_3%20%3D%20%22l%22%20,%20_4%20%3D%20%22t%22%3B%0A%0A//%20my%0A_2%20%3D%20%22y%22,%20_3%20%3D%20%22%20%22%20,%20_4%20%3D%20%22%20%22%3B%0A%0A//%20mind%0A_2%20%3D%20%22i%22,%20_3%20%3D%20%22n%22%20,%20_4%20%3D%20%22d%22%3B&curInstr=7&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    ```js
      // many
      _1 = "m" , _2 = "a", _3 = "n" , _4 = "y";
      // men
      _2 = "e", _3 = "n" , _4 = " ";
      // may
      _2 = "a", _3 = "y" , _4 = " ";

      // melt
      _2 = "e", _3 = "l" , _4 = "t";

      // my
      _2 = "y", _3 = " " , _4 = " ";

      // mind
      _2 = "i", _3 = "n" , _4 = "d";
    ```

    1. [if fir trees ever fall](https://goo.gl/8y5Lh2)

solution : [pytut]( http://www.pythontutor.com/javascript.html#code=//%20if%20fir%20trees%20ever%20fall%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20'%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20if%0A_1%20%3D%20'i',%20_2%20%3D%20'f',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20'%3B%0A//%20fir%0A%20_1%20%3D%20_2%20,%20_2%20%3D%20%22i%22%20,%20_3%20%3D%20'r',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20'%3B%0A%0A//%20trees%0A%20_1%20%3D%20%22t%22%20,%20_2%20%3D%20_3,%20_3%20%3D%20'e',%20_4%20%3D%20_3,%20_5%20%3D%20's'%3B%0A%0A//%20ever%0A%20_4%20%3D%20_2,%20_1%20%3D%20_3%20,%20_2%20%3D%20%22v%22,%20_3%20%3D%20_1%20,%20_5%20%3D%20''%3B%0A%0A//%20fall%0A%20_1%20%3D%20%22f%22%20,%20_2%20%3D%20%22a%22,%20_3%20%3D%20'l',%20_4%20%3D%20_3,%20_5%20%3D%20'%20'%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)



```js
  // if
  _1 = 'i', _2 = 'f', _3 = ' ', _4 = ' ', _5 = ' ';
  // fir
  _1 = _2 , _2 = 'i' , _3 = 'r', _4 = ' ', _5 = ' ';

  // trees
  _1 = 't' , _2 = _3, _3 = 'e', _4 = _3, _5 = 's';

  // ever
  _4 = _2, _1 = _3 , _2 = 'v', _3 = _1 , _5 = '';

  // fall
  _1 = 'f' , _2 = 'a', _3 = 'l', _4 = _3, _5 = ' ';
```

2. With extra holder variables:
* challenges:
    1. [the toad reads me](https://goo.gl/4eqhLb)

    solution : [pytut]( http://www.pythontutor.com/javascript.html#code=//%20the%20toad%20reads%20me%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20%22%20%22,%20_2%20%3D%20%22%20%22,%20_3%20%3D%20%22%20%22,%20_4%20%3D%20%22%20%22,%20_5%20%3D%20%22%20%22%3B%0Alet%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20the%0A_1%20%3D%20%22t%22,%20_2%20%3D%20%22h%22,%20_3%20%3D%20%22e%22%3B%0A%0A//%20toad%0Ax%20%3D%20_2%20,%20_2%20%3D%20%22o%22,%20y%20%3D%20_3,%20%20_3%20%3D%20%22a%22,%20_4%20%3D%20%22d%22%3B%0A%0A//%20reads%0A_1%20%3D%20%22r%22,%20_2%20%3D%20y%20,%20_5%20%3D%20%22s%22,%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A%0A//%20me%0A_1%20%3D%20%22m%22,%20%20_3%20%3D%20%22%20%22,%20_4%20%3D%20%22%20%22,%20_5%20%3D%20%22%20%22,%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    ```js
    // the
    _1 = "t", _2 = "h", _3 = "e";

    // toad
    x = _2 , _2 = "o", y = _3,  _3 = "a", _4 = "d";

    // reads
    _1 = "r", _2 = y , _5 = "s", x = ' ', y = ' ';

    // me
    _1 = "m",  _3 = " ", _4 = " ", _5 = " ", x = ' ', y = ' ';
    ```
    1. [eating meat every meal](https://goo.gl/F9Njwp)

    solution : [pytut](http://www.pythontutor.com/javascript.html#code=//%20eating%20meat%20every%20meal%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20',%20_6%3D%20'%20'%3B%0Alet%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20eating%0A_1%20%3D%20'e',%20_2%20%3D%20'a',%20_3%20%3D%20't',%20_4%20%3D%20'i',%20_5%20%3D%20'n',%20_6%3D%20'g'%3B%0A%0A//%20meat%0Ax%20%3D%20_1,%20_1%20%3D%20'm',%20y%20%3D%20_2%20,%20%20_2%20%3D%20x,%20_4%20%3D%20_3,%20_3%20%3D%20y%20,%20_5%20%3D%20'%20',%20_6%3D%20'%20'%3B%0A%0A//%20every%0Ay%20%3D%20_3%20,%20x%20%3D%20_1,%20_1%20%3D%20_2%20,%20_3%20%3D%20_2%20,%20_2%20%3D%20'v',%20%20_4%20%3D%20'r',%20_5%20%3D%20'y',%20_6%3D%20'%20'%3B%0A%0A//%20meal%0A%0A_1%20%3D%20x%20,%20_2%20%3D%20_3%20,%20_3%20%3D%20y,%20_4%20%3D%20'l',%20_5%20%3D%20'%20',%20_6%3D%20'%20',%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A%0A%0A&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    ```js

    // eating
    _1 = 'e', _2 = 'a', _3 = 't', _4 = 'i', _5 = 'n', _6= 'g';

    // meat
    x = _1, _1 = 'm', y = _2 ,  _2 = x, _4 = _3, _3 = y , _5 = ' ', _6= ' ';

    // every
    y = _3 , x = _1, _1 = _2 , _3 = _2 , _2 = 'v',  _4 = 'r', _5 = 'y', _6= ' ';

    // meal

    _1 = x , _2 = _3 , _3 = y, _4 = 'l', _5 = ' ', _6= ' ', x = ' ', y = ' ';



    ```
    1. [many men may melt my mind](http://www.pythontutor.com/javascript.html#code=//%20many%20men%20may%20melt%20my%20mind%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20'%3B%0Alet%20x,%20y%3B%0A//%20--%20you%20write%20this%20--%0A%0A//%20many%0A%0A//%20men%0A%0A//%20may%0A%0A//%20melt%0A%0A//%20my%0A%0A//%20mind&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)

    solution : [pytut](http://www.pythontutor.com/javascript.html#code=//%20many%20men%20may%20melt%20my%20mind%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20'%3B%0Alet%20x,%20y%3B%0A//%20--%20you%20write%20this%20--%0A%0A//%20many%0A_1%20%3D%20'm',%20_2%20%3D%20'a',%20_3%20%3D%20'n',%20_4%20%3D%20'y'%3B%0A//%20men%0A%20x%20%3D%20_2,%20_2%20%3D%20'e',%20_4%20%3D%20'%20'%3B%0A//%20may%0A%20y%20%3D%20_3,%20_2%20%3D%20x%20,%20_3%20%3D%20%22y%22,%20_4%20%3D%20'%20'%3B%0A%0A//%20melt%0A%20x%20%3D%20_3,%20_2%20%3D%20'e',%20_3%20%3D%20'l',%20_4%20%3D%20't'%3B%0A%0A//%20my%0A_2%20%3D%20x,%20_3%20%3D%20'%20',%20_4%20%3D%20'%20'%3B%0A%0A//%20mind%0A%20_2%20%3D%20'i',%20_4%20%3D%20'd',%20_3%20%3D%20y,%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)


    ```js

    // many
    _1 = 'm', _2 = 'a', _3 = 'n', _4 = 'y';
    // men
    x = _2, _2 = 'e', _4 = ' ';
    // may
    y = _3, _2 = x , _3 = "y", _4 = ' ';

    // melt
    x = _3, _2 = 'e', _3 = 'l', _4 = 't';

    // my
    _2 = x, _3 = ' ', _4 = ' ';

    // mind
    _2 = 'i', _4 = 'd', _3 = y, x = ' ', y = ' ';
    ```

    1. [if fir trees ever fall](https://goo.gl/BCC6pz)

    solution : [pytut]( http://www.pythontutor.com/javascript.html#code=//%20if%20fir%20trees%20ever%20fall%0A%0A//%20we%20give%20you%20this%0Alet%20_1%20%3D%20'%20',%20_2%20%3D%20'%20',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20'%3B%0Alet%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%20//%20to%20save%20extra%20values%20for%20later%0A%0A//%20--%20you%20write%20this%20--%0A%0A//%20if%0A%20_1%20%3D%20'i',%20_2%20%3D%20'f',%20_3%20%3D%20'%20',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20',%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A//%20fir%0Ax%20%3D%20_1%20,%20_1%20%3D%20_2,%20_2%20%3D%20x%20,%20_3%20%3D%20'r',%20_4%20%3D%20'%20',%20_5%20%3D%20'%20',%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A//%20trees%0Ay%20%3D_1,%20x%20%3D%20_3,%20_1%20%3D%20't',%20_2%20%3D%20x,%20_3%20%3D%20'e',%20_4%20%3D%20_3,%20_5%20%3D%20's',%20x%20%3D%20'%20'%3B%0A//%20ever%0Ax%20%3D%20_2,%20_1%20%3D%20_3%20,%20_2%20%3D%20'v',%20_3%20%3D%20_1,%20_4%20%3D%20x,%20_5%20%3D%20'%20',%20x%20%3D%20'%20'%3B%0A//%20fall%0A_1%20%3D%20y,%20_2%20%3D%20'a',%20_3%20%3D%20'l',%20_4%20%3D%20_3,%20_5%20%3D%20'%20',%20x%20%3D%20'%20',%20y%20%3D%20'%20'%3B%0A&curInstr=7&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)


    ```js

    // if
    _1 = 'i', _2 = 'f', _3 = ' ', _4 = ' ', _5 = ' ', x = ' ', y = ' ';
    // fir
    x = _1 , _1 = _2, _2 = x , _3 = 'r', _4 = ' ', _5 = ' ', x = ' ', y = ' ';
    // trees
    y =_1, x = _3, _1 = 't', _2 = x, _3 = 'e', _4 = _3, _5 = 's', x = ' ';
    // ever
    x = _2, _1 = _3 , _2 = 'v', _3 = _1, _4 = x, _5 = ' ', x = ' ';
    // fall
    _1 = y, _2 = 'a', _3 = 'l', _4 = _3, _5 = ' ', x = ' ', y = ' ';

    ```
