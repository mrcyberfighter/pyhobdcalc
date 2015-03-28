=======================
pyhobdcalc description.
=======================

---------------------------------------------------------------------
**pyhobdcalc for Python Hexadecimal Octal Binary Decimal Calculation**
---------------------------------------------------------------------

:::::::::::::::::::::::
Module description    :
:::::::::::::::::::::::


                                                                                                                                     
  pyhobdcalc is a python module written in C which implement conversion and calculating functions in bases 2, 8, 10, 16.          
                                                                                                                                   
            Which python doesn't implement like signed binary, octal, hexadecimal conversion in integers.                            
                                                                                                                                   
            Or signed float conversion from decimal to base 2, 8, 16 or from base 2, 8, 16 in decimal base.                        
                                                                                                                                   
            And performs addition, subtraction, multiplication and division on integers and float strings using bases 2, 8, and 16 .                           
                                                                                                                                   

    
  
::::::::::::::::::::::
Module implementation:
::::::::::::::::::::::

++++++++++++++++++++++++++
Base conversion functions:
++++++++++++++++++++++++++

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Different bases integer string conversion to integer :
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~  
    
    1. **bintoint**:
    
        Convert a binary string given with optional the binary identifier "0b". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the converted value as an integer string.
        
    2. **octtoint**:
    
        Convert an octal string given with optional the octal identifier "0". The function can thread signed values in the C type *long long int* value range:               
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the converted value as an integer string.
        
    3. **hextoint**:
    
        Convert a hexadecimal string given with optional the hexadecimal identifier "0x". The function can thread signed values in the C type *long long int* value range:               
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the converted value as an integer string.
        
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 
Different bases float string conversion to float   : 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    1. **binfloattofloat**:
    
        Convert a binary string with optional binary identifier "0b" representing a floating-point value into a float with maximal precision from 15 digits.
        
        And return the converted value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
            
    2. **octfloattofloat**:
    
        Convert an octal string with optional octal identifier "0" representing a floating-point value into a float with maximal precision from 15 digits.
        
        And return the converted value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
            
    3. **hexfloattofloat**:
    
        Convert a hexadecimal string with optional hexadecimal identifier "0x" representing a floating-point value into a float with maximal precision from 15 digits.
        
        And return the converted value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
            
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Float to different base float  :
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~                     

    1. **floattobinfloat**:
    
        Convert a float given as a string into a floating-point binary string with a maximum length of 16 binary digits. The given float integer part has a maximum length of 8 bytes.
        
        And return the floating-point binary string corresponding to the given float with the given limitations.
        
    2. **floattooctfloat**:
    
        Convert a float given as a string into a floating-point octal string with a maximum length of 16 octal digits. The given float integer part has a maximum length of 8 bytes.
        
        And return the floating-point octal string corresponding to the given float with the given limitations.
        
    3. **floattohexfloat**:
    
        Convert a float given as a string into a floating-point hexadecimal string with a maximum length of 16 hexadecimal digits. The given float integer part has a maximum length of 8 bytes.
        
        And return the floating-point hexadecimal string corresponding to the given float with the given limitations.
                   
                   
+++++++++++++++++++++++++++++++++++++++++++++
Base 2, 8, 16 integers calculating functions:
+++++++++++++++++++++++++++++++++++++++++++++

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Binary integer calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  1. **binaddbin**:
        
        Add 2 binary strings given with optional the binary identifier "0b". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the addition result as an integer string.    
            
            :note: The addition result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  2. **binsubbin**:
        
        Subtract 2 binary strings given with optional the binary identifier "0b". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the subtraction result as an integer string.    
            
            :note: The subtraction result cannot overflow the same maximal and minimal range as for the given arguments values. 
            
  3. **binmultbin**:
        
        Multiply 2 binary strings given with optional the binary identifier "0b". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the multiplication result as an integer string.    
            
            :note: The multiplication result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  4. **bindivbin**:
        
        Divide 2 binary strings given with optional the binary identifier "0b". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the division result as an integer string.    
            
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
            
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Octal integer calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  1. **octaddoct**:
        
        Add 2 octal strings given with optional the octal identifier "0". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the addition result as an integer string.    
            
            :note: The addition result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  2. **octsuboct**:
        
        Subtract 2 octal strings given with optional the octal identifier "0". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the subtraction result as an integer string.    
            
            :note: The subtraction result cannot overflow the same maximal and minimal range as for the given arguments values. 
            
  3. **octmultoct**:
        
        Multiply 2 octal strings given with optional the octal identifier "0". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the multiplication result as an integer string.    
            
            :note: The multiplication result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  4. **octdivoct**:
        
        Divide 2 octal strings given with optional the octal identifier "0". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the division result as an integer string.    
            
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
            
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Hexadecimal integer calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  1. **hexaddhex**:
        
        Add 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the addition result as an integer string.    
            
            :note: The addition result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  2. **hexsubhex**:
        
        Subtract 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the subtraction result as an integer string.    
            
            :note: The subtraction result cannot overflow the same maximal and minimal range as for the given arguments values. 
            
  3. **hexmulthex**:
        
        Multiply 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the multiplication result as an integer string.    
            
            :note: The multiplication result cannot overflow the same maximal and minimal range as for the given arguments values.
            
  4. **hexdivhex**:
        
        Divide 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts signed values in the C type *long long int* value range:
        
            * Maximal value:  9223372036854775807.
            
            * Minimal value: -9223372036854775808.
            
        And return the division result as an integer string.    
            
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.
                                   
            
++++++++++++++++++++++++++++++++++++++++++
Base 2, 8, 16 float calculating functions:
++++++++++++++++++++++++++++++++++++++++++                               

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Binary float calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    1. **binfloataddbinfloat**:
    
        Add 2 binary strings given with optional the binary identifier "0b". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire binary string can contains 128 binary digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    2. **binfloatsubbinfloat**:
    
        Subtract 2 binary strings given with optional the binary identifier "0b". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire binary string can contains 128 binary digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                  
    3. **binfloatmultbinfloat**:
    
        Multiply 2 binary strings given with optional the binary identifier "0b". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire binary string can contains 128 binary digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    4. **binfloatdivbinfloat**:
    
        Divide 2 binary strings given with optional the binary identifier "0b". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire binary string can contains 128 binary digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                                
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Octal float calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    1. **octfloataddoctfloat**:
    
        Add 2 octal strings given with optional the octal identifier "0". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire octal string can contains 48 octal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    2. **octfloatsuboctfloat**:
    
        Subtract 2 octal strings given with optional the octal identifier "0". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire octal string can contains 48 octal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                  
    3. **octfloatmultoctfloat**:
    
        Multiply 2 octal strings given with optional the octal identifier "0". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire octal string can contains 48 octal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    4. **octfloatdivoctfloat**:
    
        Divide 2 octal strings given with optional the octal identifier "0". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire octal string can contains 48 octal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                                
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Hexadecimal float calculating functions:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    1. **hexfloataddhexfloat**:
    
        Add 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire hexadecimal string can contains 16 hexadecimal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    2. **hexfloatsubhexfloat**:
    
        Subtract 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire hexadecimal string can contains 16 hexadecimal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                  
    3. **hexfloatmulthexfloat**:
    
        Multiply 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire hexadecimal string can contains 16 hexadecimal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
            
    4. **hexfloatdivhexfloat**:
    
        Divide 2 hexadecimal strings given with optional the hexadecimal identifier "0x". The function accepts 8 bytes values for the integer part from the float, in the C type *long long int* value range:
        
            * Maximal integer part value:  9223372036854775807.
            
            * Minimal integer part value: -9223372036854775808.
            
        The entire hexadecimal string can contains 16 hexadecimal digits (without identifier, sign and comma.).
        
        And return the result value as a float string.
        
            :note: The returned value is limited to the C type *double* (15 digits precision) but internally the module uses the C type *long double* (19 digits precision) for getting an exact value.                                                          
                                                               
Thank's to gtackett 

for the improved English style, grammar, and spelling correction from this file.                                           
              
 
