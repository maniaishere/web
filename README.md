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

