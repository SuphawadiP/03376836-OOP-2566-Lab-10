# Lab 10 Exercise 2

## Constructor ใน derived class

1.สร้าง console application project

```cmd
dotnet new console --name Lab10_Ex02
```

2.เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
var circle = new Circle();
var rectangle = new Rectangle();
var triangle = new Triangle();

class Shape
{
    public Shape()
    {
        System.Console.WriteLine("This is some shape");
    }
}
class Circle :Shape
{
    public Circle()
    {
        System.Console.WriteLine("This is a circle");
    }
}
class Rectangle :Shape
{
    public Rectangle()
    {
        System.Console.WriteLine("This is a rectangle");
    }
}
class Triangle :Shape
{
   public Triangle()
    {
        System.Console.WriteLine("This is a triangle");
    }
}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab10_Ex02
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="797" alt="Screenshot 2024-03-29 130106" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-10/assets/144196049/5f5374fb-8572-4c86-94d3-73974ef7626d">

#### สามารถ Build ได้ เพราะ สร้าง Constructor แต่มีการเรียกใช้ Constructor จาก class ที่สืบทอด baseclass ด้วยคำสั่ง Shape()
5.Run project โดยการใช้คำสั่ง
5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab10_Ex02
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="797" alt="Screenshot 2024-03-29 130131" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-10/assets/144196049/a1333573-a436-4b23-884c-08ecd6b5d343">

#### สามารถ Run ได้ ปกติ
7.อธิบายสิ่งที่พบในการทดลอง
#### โปรแกรมจะแสดงผล
#### This is some shape
#### This is a circle
#### This is some shape
#### This is a rectangle
#### This is some shape
#### This is a triangle
