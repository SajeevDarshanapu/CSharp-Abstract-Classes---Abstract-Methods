# CSharp-Abstract-Classes---Abstract-Methods


# Abstract Class


abstract class Language {

                                                     // abstract method
  public abstract void display1();

                                                      // non-abstract method
  public void display2() {
    Console.WriteLine("Non abstract method");
  }
}

#  Inheriting Abstract Class

using System;
namespace AbstractClass {

  abstract class Language {

                                                                         // non-abstract method
    public void display() {
      Console.WriteLine("Non abstract method");
    }
  }

                                                                // inheriting from abstract class
  class Program : Language {

    static void Main (string [] args) {
      
                                                                     // object of Program class
      Program obj = new Program();

                                                             // access method of an abstract class
      obj.display();

      Console.ReadLine();
    }
  }
}


====================================

# Implementation of Abstract Methods

using System;
namespace AbstractClass {

  abstract class Animal {

    // abstract method
    public abstract void makeSound();
  }

  // inheriting from abstract class
  class Dog : Animal {

    // provide implementation of abstract method
    public override void makeSound() {

      Console.WriteLine("Bark Bark");

    }
  }
  class Program  {
    static void Main (string [] args) {
      // create an object of Dog class
      Dog obj = new Dog();
      obj.makeSound();    

      Console.ReadLine(); 
    }
  }
}

# ABSTRACTION


using System;
namespace AbstractClass {
  abstract class MotorBike {
    
    public abstract void brake();
  }

  class SportsBike : MotorBike {

    // provide implementation of abstract method
    public override void brake() {
      Console.WriteLine("Sports Bike Brake");
    }
   
  }

  class MountainBike : MotorBike {

    // provide implementation of abstract method
    public override void brake() {      
      Console.WriteLine("Mountain Bike Brake");
    }
   
  }
  class Program  {
    static void Main (string [] args) {
      // create an object of SportsBike class
      SportsBike s1 = new SportsBike();  
      s1.brake();

      // create an object of MountainBike class
      MountainBike m1 = new MountainBike();
      m1.brake();

      Console.ReadLine();
    }
  }
}
