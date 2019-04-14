# 19-Abgabe02-Olczak_Paier
Second exercise, dealing with MAVEN and ANT

The purpose of this repository is to learn how to deal with build automation, as part of the Mobile Software Development course "Configuration-Management" at University of Applied Science - FH Joanneum Graz.

Therefore, two projects were created, a Maven and an Ant project, in order to understand the difference between building a project automatically and building a project manually.

**Compare file structure Maven vs. Ant:** <br/>
<img src="https://user-images.githubusercontent.com/48792646/56096791-007d9100-5eed-11e9-93b4-5434adbd63b4.jpg" width="100" >
<img src="https://user-images.githubusercontent.com/48792646/56096832-433f6900-5eed-11e9-94ed-fe0497c76841.jpg" width="100" >

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
