<div align="center">

## Java String Replace


</div>

### Description

This piece of code takes three arguments, you give it a string that you want to do the replace on, what you want to replace, and what you want to replace it with! Simple!
 
### More Info
 
String to do replace on,

String to search for,

String to replace search String with

String


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Martyn B](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/martyn-b.md)
**Level**          |Beginner
**User Rating**    |3.3 (13 globes from 4 users)
**Compatibility**  |Java \(JDK 1\.1\)
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__2-60.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/martyn-b-java-string-replace__2-1859/archive/master.zip)





### Source Code

```
// Example:
// replace("He/\£$llo", "/\£$", " ")
// it will return "He llo"
public static String replace(String checkMe, String toberep, String repwith)
	{
	String temp = checkMe;
	int a = 0;
	try {
			for(int i = 0; i < checkMe.length(); i++)
			{
				a = temp.indexOf(toberep);
				temp = temp.substring(0 , a) + repwith + temp.substring((a + toberep.length()));
				if (a == -1)
				{
				break;
				}
			}
		} catch (Exception e) {/*IGNORE*/}
		return temp;
	}
```

