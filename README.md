# Inheritance
//NAME: Mayur
//PRN: 24070123507
//Exp-14

//Program-1
#include<iostream>
#include<string>
usingnamespacestd;

classUni {
    public:
    stringuni="Symbiosis: ";
    voiddiscipline(){
        cout<<"Engineering"<<endl;
    }
};
classDep: publicUni {
    public:
    stringdept="Electronics & Communication";
};

intmain(){
    Depu1;
    u1.discipline();
    cout<<u1.uni+" "+u1.dept;
}

•	Multiple inheritance In Multiple Inheritance a class can inherit from more than one class. (i.e.) one subclass is inherited from more than one base class.

EXAMPLE CODE:
//NAME: Mayur
//PRN: 24070123507
//Exp-14

//Program-2
#include<iostream>
#include<string>
usingnamespacestd;

//Parent Class-1
classVehicle {
    public:
    stringcompany="Ford";
    voidtype(){
        cout<<"Mustang"<<endl;
    }
};
//Parent Class-2
classSpecs {
    public:
    stringmileage="8 kmpl";
    voidcolour(){
        cout<<"Grey"<<endl;
    }
};
//Child Class-1 (derived from parent-1&2)
classCar: publicVehicle, publicSpecs {
    public:
    stringseater="4 seater";
};

intmain(){
    //Multiple Inheritance
    Carf2;
    f2.colour();
    cout<<f2.company<<" ";
    f2.type();
    cout<<"("<<f2.seater<<")"<<endl<<"MILEAGE: "<<f2.mileage<<endl;
}


OUTPUT:


•	Multilevel inheritance In this type of inheritance, a derived class is created from another derived class.



EXAMPLE CODE:
//NAME: Mayur
//PRN: 24070123507
//Exp-14

//Program-3
#include<iostream>
#include<string>
usingnamespacestd;

//Parent Class-1
classFood {
    public:
    stringcuisine="Indian";
    voidtype(){
        cout<<"Asian"<<endl;
    }
};
//Child Class-1 (derived from parent-1)
classDish: publicFood {
    public:
    stringdish="Biryani";
};
//Child Class-2 (derived from child-1)
classRestaurant: publicDish {
    public:
    stringname="Spice Kitchen";
};

intmain(){
    //Multilevel Inheritance
    Restaurantf3;
    f3.type();
    cout<<f3.cuisine<<": "<<f3.dish<<endl;
    cout<<"Restaurant: "<<f3.name;
}





OUTPUT:


•	Hierarchical inheritance In this type of inheritance, more than one subclass is inherited from a single base class. i.e. more than one derived class is created from a single base class.

EXAMPLE CODE:
//NAME: Mayur
//PRN: 24070123507
//Exp-14

//Program-4
#include<iostream>
#include<string>
usingnamespacestd;

//Parent Class-1
classJeans {
    public:
    stringtype[3]= {"Bootcut", "Wide Leg", "Skinny"};
    voidbrand(){
        cout<<"H&M - &Denim"<<endl;
    }
};
//Child Class-1
classBootcut: publicJeans {
    public:
    stringcolor="Dark Blue";
};
//Child Class-2
classWL: publicJeans {
    public:
    stringcolor="Black";
};
//Child Class-3
classSkinny: publicJeans {
    public:
    stringcolor="Grey";
};

//Hierarchical Inheritance
intmain(){
    Bootcutj1;
    cout<<endl;
    j1.brand();
    cout<<j1.type[0]<<": "<<j1.color<<endl;

    WLj2;
    cout<<endl;
    j2.brand();
    cout<<j2.type[1]<<": "<<j2.color<<endl;

    Skinnyj3;
    cout<<endl;
    j3.brand();
    cout<<j3.type[2]<<": "<<j3.color<<endl;
}

OUTPUT:



