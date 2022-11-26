# Learning
import random
num = random.randint(1,10)
guess_num = int(input("请输入你猜测的数字"))
if guess_num == num :
    print("恭喜你第一次就猜对了")
elif guess_num > num:
    print("很抱歉猜大了")
    guess_num = int(input("请再次猜测"))
    if guess_num == num :
        print("恭喜你第二次猜对了")
    elif guess_num > num :
        print("猜大了")
        guess_num = int(input("请再次猜测"))
        if guess_num == num:
            print("恭喜你第三次猜对了")
        else:
            print("猜错了")
    else :
        print("猜小了")
        guess_num = int(input("请再次猜测"))
        if guess_num == num:
            print("恭喜你第三次猜对了")
        else:
            print("猜错了")
else :
    print("很抱歉猜小了")
    guess_num = int(input("请再次猜测"))
    if guess_num == num:
        print("恭喜你第二次猜对了")
    elif guess_num > num :
        print("猜大了")
        guess_num = int(input("请再次猜测"))
        if guess_num == num :
            print("恭喜你第三次猜对了")
        else:
            print("很抱歉猜错了")
    else:
        print("猜小了")
        guess_num = int(input("请再次猜测"))
        if guess_num == num :
            print("恭喜你第三次猜对了")
        else:
            print("很抱歉猜错了")
