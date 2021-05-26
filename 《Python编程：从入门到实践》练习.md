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
