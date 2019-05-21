# easyexcel
Excel快速生成工具



在现有实体类的基础上构建最简单的Excel，代码只需4行。

实体类：

`Student{name, idcard, sex, ...}`

生成XSSFWorkbook：

```java
String sheetName = "sheet name";
String[] columnNames = {"姓名", "身份证号", "性别", ...};
String[] classFieldNames = {"name", "idcard", "sex", ...};
XSSFWorkbook workbook = ExcelBuilder.createWorkbook(new SheetInfo(sheetName, columnNames, classFieldNames, studentList));
```

使用方法详见test目录。

