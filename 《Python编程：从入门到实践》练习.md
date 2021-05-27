print("Hello Python interpreter!")
print("Hello world!")
print("Hello Python interpreter!")
message = "Hello Python Crash Course reader!"
print(message)
mesage = "Hello Python Crash Course reader!"
print(mesage)
name = "Ada Lovelace"
#大小写
print(name.upper())
print(name.lower())

first_name = "ada"
last_name = "lovelace"
full_name = first_name + " " + last_name
print("Hello, " + full_name.title() + "!")
#换行
print("Languages:\nPython\nC\nJavaScript")

print(0.2+0.1)
print(3*0.1)

#转换
age = 23
message = "Happy " + str(age) + "rd Birthday!"
print(message)
#yuanze
import this
print(this)

#列表
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles)
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[0].title())

#添加列表
motorcycles = []
motorcycles.append('younlenms')
print(motorcycles)

#在在列列表表中中插插入入元元素素
motorcycles = ['honda', 'yamaha', 'suzuki']
motorcycles.insert(2,'younlens')
print(motorcycles)

#　　从从列列表表中中删删除除元元素素
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)
del motorcycles[2]
print(motorcycles)


####使用用方方法法pop() 删删除除元元素素
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles)
popped_motorcycle = motorcycles.pop()
print(motorcycles)
print(popped_motorcycle)


motorcycles = ['honda', 'yamaha', 'suzuki']
last_owner=motorcycles.pop()
print('The last motorcycle I owned was a'+last_owner.title()+'.')

#弹出列表中任何位置处的元素
motorcycles = ['honda', 'yamaha', 'suzuki']
first_owned=motorcycles.pop(1)
print('The first motorcycle I owned was a '+first_owned.title()+'.')

#根据据值值删删除除元元素素
motorcycles = ['honda', 'yamaha', 'suzuki', 'ducati']
print(motorcycles)
motorcycles.remove('honda')
print(motorcycles)

#3.3　　组组织织列列表表
#3.3.1　　使使用用方方法法sort() 对对列列表表进进行行永永久久性性排排序序
cars=['bmw','audi','toyota','subaru']
cars.sort()
print(cars)

cars=['bmw','audi','toyota','subaru']
cars.sort(reverse=True)
print(cars)

#3.3.2　　使使用用函函数数sorted() 对对列列表表进进行行临临时时排排序序
cars = ['bmw', 'audi', 'toyota', 'subaru']
print('Here is the original list:')
print(cars)
print("\nHere is the sorted list:")
print(sorted(cars))
print("\nHere is the original list again:")
print(cars)

#3.3.3　　倒倒着着打打印印列列表表
cars = ['bmw', 'audi', 'toyota', 'subaru']
print(cars)
cars.reverse()
print(cars)

#确定定列列表表的的长长度度
cars = ['bmw', 'audi', 'toyota', 'subaru']
len(cars)
print(len(cars))

#3.4　　使使用用列列表表时时避避免免索索引引错错误误
motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles[0])

motorcycles = ['honda', 'yamaha', 'suzuki']
print(motorcycles[-1])

#motorcycles = [ print(motorcycles[-1])


#第第 4 章章　　操操作作列列表表

magicians = ['alice', 'david', 'carolina']
for magician in magicians:
    print(magician)

#4.1.1　　深深入入地地研研究究循循环环
#4.1.2　　在在for 循循环环中中执执行行更更多多的的操操作作

magicians = ['alice', 'david', 'carolina']
for magician in magicians:
    print(magician.title()+ ' that was agreat trick!')
    print("I can't wait to see your next trick, " + magician.title() + ".\n")

#4.1.3　　在在for 循循环环结结束束后后执执行行一一些些操操作作
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
    print(magician.title() + ", that was a great trick!")
    print("I can't wait to see your next trick, " + magician.title() + ".\n")
print("Thank you, everyone. That was a great magic show!")

#4.2.2　　忘忘记记缩缩进进额额外外的的代代码码行行
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
    print(magician.title() + ", that was a great trick!")
    print("I can't wait to see your next trick, " + magician.title() + ".\n")

#4.2.3　　不不必必要要的的缩缩进进
message = "Hello Python world!"
#print(message)

#4.3　　创创建建数数值值列列表表
for value in range(1,5):
    print(value)

#4.3.2　　使使用用range() 创创建建数数字字列列表表
numbers=list(range(1,5))
print(numbers)

even_numbers=list(range(2,15,3))
print(even_numbers)

squares = []
for value in range(1,11):
    square = value ** 3
    squares.append(square)
    print(squares)

#4.3.3　　对对数数字字列列表表执执行行简简单单的的统统计计
digits = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
min(digits)
max(digits)
sum(digits)
print(min(digits),max(digits),sum(digits))

#4.3.4　　列列表表解解析析
squares = [value**2 for value in range(1,11)]
print(squares)


#4.4　　使使用用列列表表的的一一部部分分
#4.4.1　　切切片片
players = ['charles', 'martina', 'michael', 'florence', 'eli']
print(players[0:4])
#4.4.2　　遍遍历历切切片片
players = ['charles', 'martina', 'michael', 'florence', 'eli']
print("Here are the first three players on my team:")
for player in players[:2]:
    print(player.title())
