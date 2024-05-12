# 19AI308-Object-Oriented-Programming-using-CSharp--Exp-8-Name-Hiding-with-interface-inheritance
# AIM:
To implement name hiding with interface inheritance. Aim is to create an interface IMario with a method Ability(). 
Implement this interface in a class Mario and override the Ability() method also to create another class SuperMario that inherits from Mario 
and hides the Ability() method using the new keyword.
# ALGORITHM:
Step 1:
Create interface IMario with method Ability for Mario classes.
Step 2:
Mario class implements IMario and defines the virtual Ability method.
Step 3:
SuperMario extends Mario and overrides the Ability method with a new one.
Step 4:
Instantiate SuperMario and Mario, call Ability on each.
Step 5:
SuperMario's Ability prints "This is inside SuperMario", and Mario's prints "This is inside Mario".
# PROGRAM:
```
using System;
public interface IMario
{
    void Ability();
}

class Mario : IMario
{
    public virtual void Ability()
    {
        Console.WriteLine("Mario's normal ability is Jumping");
    }
}

class SuperMario : Mario
{
    public new void Ability()
    {
        Console.WriteLine("Super Mario's ability is  Flying and shooting fireballs");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Mario mario = new Mario();
        SuperMario superMario = new SuperMario();

        mario.Ability(); 
        superMario.Ability();
    }
}
```
# OUTPUT:
![image](https://github.com/Kousalya22008930/19AI308-Object-Oriented-Programming-using-CSharp--Exp-8-Name-Hiding-with-interface-inheritance/assets/119389108/27e87807-7789-439b-a2e0-63b924abb1dd)

# RESULT:
Thus, the C# program has been executed successfully.


