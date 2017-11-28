
In c++,there are two flavors of class data members--static and nonstatic--and three flavors of class member functions--static,nonstatic,and virtual.

A Simple Object Model
an object is a sequence of slots,where each slot points to a member.The members are assigned a slot in the order of their delarations.There is a slot for each data or function member.In this model,only pointers addressing the members are placed within the object.

A Table-driven Object Model
This model factor out all member specific information,placing it in a data member and member function pair of tables.

The C++ Object Model
Nonstatic members are allocated dirctly within each class object.Static data members are stored outside the individual class object.Static and nonstatic functions are also hoisted outside the class object.Virtual functions are supported in two steps:
    1.A table of pointers to virtual functions is generated for each class(this is called the virtual table).
    2.A single pointer to the associated virtual table is inserted in each class object.


