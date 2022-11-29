# web

XML-XSL
```
<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/xsl" href="style.xsl"?>

<details>
    <student>
        <name>Anish the elite</name>
        <age>19</age>
    </student>

    <student>
        <name>Vamsi the best</name>
        <age>19</age>
    </student>

    <student>
        <name>Siddharth the best friend</name>
        <age>19</age>
    </student>
</details>
```

```
<?xml version="1.0" encoding="UTF-8"?>
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">

<xsl:template match="/">

<html>

<body>
    <h1>ABOUT STUDENT</h1>
    <table border="3">
    <tr bgcolor = "blue">
    <th>name</th>
    <th>age</th>
    </tr>

    <xsl:for-each select="details/student">
        <tr>
        <td> <xsl:value-of select="name"/> </td>
        <td> <xsl:value-of select="age"/> </td>
        </tr>
    </xsl:for-each>


    </table>
</body>
</html>


</xsl:template>
</xsl:stylesheet>
```

LAB-7
```
<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/css" href="6 .css" ?> 
<!DOCTYPE HTML> 
<html> 
<head> 
<h1>
 STUDENTS DESCRIPTION</h1> 
</head> 
<students> 
<student> 
<usn>USN : 1CG15CS001</usn> 
<name>NAME : Divyank Singh Sikarwar</name> 
<college>COLLEGE : SRM</college> 
<branch>BRANCH : Computer Science and Engineering</branch> 
<year>YEAR : 2015</year> 
<e-mail>E-Mail : santosh@gmail.com</e-mail> 
</student> 
<student> 
<usn>USN : 1CG15IS002</usn> 
<name>NAME : Aniket Chauhan</name> 
<college>COLLEGE : CITIT</college> 
<branch>BRANCH : Information Science and Engineering</branch> 
<year>YEAR : 2015</year> 
<e-mail>E-Mail : manoranjan@gmail.com</e-mail> 
</student> 
<student> 
<usn>USN : 1CG15EC101</usn> 
<name>NAME : Simran Agarwal</name> 
<college>COLLEGE : CITIT</college> 
<branch>BRANCH : Electronics and Communication Engineering 
</branch> 
<year>YEAR : 2015</year> 
<e-mail>E-Mail : chethan@gmail.com</e-mail> 
</student> 
<student> 
<usn>USN : 1CG15IS002</usn> 
<name>NAME :Abhay Chauhan</name> 
<college>COLLEGE : CITIT</college> 
<branch>BRANCH : Information Science and Engineering</branch> 
<year>YEAR : 2015</year> 
<e-mail>E-Mail : manoranjan@gmail.com</e-mail> 
</student> 
<student> 
<usn>USN : 1CG15IS002</usn> 
<name>NAME :Himanshu Bhatia</name> 
<college>COLLEGE : CITIT</college> 
<branch>BRANCH : Information Science and Engineering</branch> 
<year>YEAR : 2015</year> 
<e-mail>E-Mail : manoranjan@gmail.com</e-mail> 
</student> 
</students> 
</html> 
```
CSS
```
student{ 
    display:block; margin-top:10px; color:Navy;
    } 
    usn{ 
    display:block; margin-left:10px;font-size:14pt; color:Red; 
    } 
    name{display:block; margin-left:20px;font-size:14pt; color:Blue; 
    } 
    college{ 
    display:block; margin-left:20px;font-size:12pt; color:Maroon; 
    } 
    branch{ 
    display:block; margin-left:20px;font-size:12pt; color:Purple; 
    } 
    year{ 
    display:block; margin-left:20px;font-size:14pt; color:Green; 
    } 
    e-mail{ 
    display:block; margin-left:20px;font-size:12pt; color:Blue; 
    } 
    ```
