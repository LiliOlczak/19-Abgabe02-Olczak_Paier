# 19-Abgabe02-Olczak_Paier
Second exercise, dealing with MAVEN and ANT

The purpose of this repository is to learn how to deal with build automation, as part of the Mobile Software Development course "Configuration-Management" at University of Applied Science - FH Joanneum Graz.

Therefore, two projects were created, a Maven and an Ant project, in order to understand the difference between building a project automatically and building a project manually.

**Compare file structure Maven vs. Ant:** <br/>
<img src="https://user-images.githubusercontent.com/45802610/56097877-35dcab80-5efa-11e9-82e0-20752e326718.png" width="300" >
<img src="https://user-images.githubusercontent.com/45802610/56097863-07f76700-5efa-11e9-900d-8b5235e8c56d.png" width="250">

**Main-Class:** <br/>
Includes the main() and sayHello() method.

```
public class Main {

    public static void main(String[] args)
    {
        Main hello = new Main();
        int number = hello.sayHello(args[0]);
        System.out.println("Anzahl der ausgegebenen Zeichen: " + number);
    }

    public int sayHello(String name)
    {
        String msg = "Hello " + name + "!";
        System.out.println(msg);
        return msg.length();
	}

}
```

**Maven:** <br/>
Includes the plugins to build a jar file.
* compiler
* jar 
* maven
* site

**Ant:** <br/>
Includes the targets to build a jar file.
* init
* clean
* compile
* jar
* install
* run
