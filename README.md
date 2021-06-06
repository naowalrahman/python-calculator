# python-calculator
A basic terminal calculator in python that uses the `eval()` function with user input for its main usage. 

Though there are lots of GUI calculators for \*NIX systems, many of them are either so feature packed that they become annoying to use for basic use, or are just impractical to use. Thus, I wanted to create a calculator in python that could be used from the terminal but also make sure that it was hackable and not bloated. 

To add more functionality into the calculator, simply import more functions from the `math` module at the beginning of the `main.py` file. For example, the default functions available are imported as: 

```python 
########## USER IMPORTS ##########
from math import radians, degrees, sqrt, pi
```

But, if you wanted to add, say, the `ceil` function, simply append it to the end of the first line with a comma, like so: 

```python
########## USER IMPORTS ##########
from math import radians, degrees, sqrt, pi, ceil
```

This non-bloated and suckless approach to adding more functionality makes for more practicality of the calculator. However, the other import functions after the user imports should be modified as they are designed to be used for the custom functions defined later on, which are used for degree-based trigonometry. 

## Basic Usage

The default functions included are sine, cosine, tangent, inverse sine, inverse cosine, inverse tangent, square root, and pi. The default trigonometry functions are calculated in degrees. However, if you wish to use radians, there are trigonmetric functions available starting with r and then the function name that calculate values in radians (like `rsin` or `artan`). The inverse functions in radians start with ar and then the function name. This is the reference list for the names of the functions:

```
                        add:   + 
                   subtract:   - 
                   multiply:   *
                     divide:   /
                   exponent:   **
             sine (degrees):   sin()
           cosine (degrees):   cos()
          tangent (degrees):   tan()
     inverse sine (degrees):   asin()
   inverse cosine (degrees):   acos()
  inverse tangent (degrees):   atan()
              sine (radian):   rsin()
            cosine (radian):   rcos()
           tangent (radian):   rtan()
      inverse sine (radian):   arsin()
    inverse cosine (radian):   arcos()
   inverse tangent (radian):   artan()
                square root:   sqrt() 
                         pi:   pi
```

At anytime, you can type `help` into the calculator to get a list of these function names. To exit the calculator, type `exit` or `q`. To clear the screen, type `clear`. 

## Installation

There is an installation script provided that automatically adds the program to `$PATH` for all users, so it is a very easy installation. To install, use the following commands: 
```sh 
git clone https://github.com/naowalrahman/python-calculator.git
cd python-calculator 
sudo sh ./install.sh 
```

To update the calculator simply run `calc-update` in your  terminal. To uninstall the calculator, run the `uninstall.sh` file from the cloned git repository with the command `sudo sh ./uninstall.sh`. 

## Contributions 
Any contributions are welcome! If any issue arises, make an issue in the issues tab. If you want to contribute to this calculator, feel free to start a pull request! 

## To Do
- [ ] Make two different versions of the calculator - one minimal edition and another feature edition. 
- [ ] Put algebra support into the calculator. 
- [ ] Make the calculator ignore python-specific functions and expressions and only recognize math expressions. 
- [X] Make uninstall script. 
