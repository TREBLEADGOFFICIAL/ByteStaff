# Byte Staff

**Introduction**
This is the byte counter which can be set up in a few ways including:

1. Watch Counter - 2. Arithmetic Logic Unit - 3. Keybind Across Audio

We will talk mainly about it's usage as an arithmetic logic unit.

For example we can trigger a boolean count up to/for eight in the following code.

`if ByteStaff.adg => "Display" => Output8 < 72{`

`|    if ByteStaff.adg => "Display" => Output8 < 72{`

`|    |    if ByteStaff.adg => "Display" => Output7 > 72{`

`|    |    |    ByteStaff.adg = "Eight";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output6 > 72{`

`|    |    |    ByteStaff.adg = "Seven";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output5 > 72`

`|    |    |    ByteStaff.adg = "Six";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output4 > 72{`

`|    |    |    ByteStaff.adg = "Five";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output3 > 72{`

`|    |    |    ByteStaff.adg = "Four";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output2 > 72{`

`|    |    |    ByteStaff.adg = "Three";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output1 > 72{`

`|    |    |    ByteStaff.adg = "Two";`

`|    |    }`

`|    |    if ByteStaff.adg => "Display" => Output1 < 72 && Output2 < 72 && Output3 < 72 && Output4 < 72{`

`|    |    |    if ByteStaff.adg => "Display" => Output5 < 72 && Output6 < 72 && Output7 < 72 && Output8 < 72{`

`|    |    |    |    ByteStaff.adg = "One";|`

`|    |    |    }`

`|    |    }`

`|    }`

`}`
`ByteStaff.adg = 1,2,3,4,5,6,7,8;`

**Description**

What this basically acomplishes is a rapid output eight with suffiecent code, where the sub code will run very quickly run below the count going high in some iterations, or also could pause to run code in more basic swift.

This is required as this will increment as fast as possible then trigger a device zero. As well you can run the code inside as it should run on its own loop if you put a func there like main so it will run then as it does!

This device is a 3 bit ALU that has an 8 by 8 breadth. Thus it is the byte processor and used to give the system various functions which it has. As well this byte processor has some turing capacity at en masse level at least.

**TALK PAGE**

This device is refered to in the ALU Section as well. It needs a page on it's own!

I am working on the wiki page and also posting this standalone as it is the core component used.

Work is finished I am posting now to the wiki, this will also be availible under the readme of byte staff.
