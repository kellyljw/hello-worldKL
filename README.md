# hello-worldKL
import random
secret = random.randint(1,10)
print('...............V大酱...............')
temp = input("不妨猜猜我现在心里想的是哪个数字：")
guess = int(temp)
while type(temp) != type(1):
    print("抱歉，输入不合法，", end='')
    temp = input("请输入一个整数：")
while guess != secret:
    temp = input("哎哟~猜错惹，请重新输入吧：")
    guess = int(temp)
    if guess == secret:
        print("哎哟喂，你是我心里的蛔虫吗？！")
        print("哼，猜中了也没有奖励！")
    else:
        if guess > secret:
            print("哥，大了大了~~~")
        else:
            print("嘿~小了小了~~~")
print("游戏结束，不玩啦~")
