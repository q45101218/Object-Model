
In c++,there are two flavors of class data members--static and nonstatic--and three flavors of class member functions--static,nonstatic,and virtual.

A Simple Object Model
an object is a sequence of slots,where each slot points to a member.The members are assigned a slot in the order of their delarations.There is a slot for each data or function member.In this model,only pointers addressing the members are placed within the object.

A Table-driven Object Model
This model factor out all member specific information,placing it in a data member and member function pair of tables.

The C++ Object Model
Nonstatic


