# calculator1
armature cal for python
def jame(x, y):
    return x + y

def tafrigh(x, y):
    return x - y

def zarb(x, y):
    return x * y

def taghsim(x, y):
    if y == 0:
        return "تقسیم بر صفر ممکن نیست"
    return x / y

while True:
    print("انتخاب عملیات:")
    print("1. جمع")
    print("2. تفریق")
    print("3. ضرب")
    print("4. تقسیم")
    print("5. خروج")
    
    choice = input("لطفاً یک عدد را انتخاب کنید (1/2/3/4/5): ")
    
    if choice == '5':
        print("ماشین حساب بسته شد.")
        break
    
    num1 = float(input("لطفاً عدد اول را وارد کنید: "))
    num2 = float(input("لطفاً عدد دوم را وارد کنید: "))
    
    if choice == '1':
        print("جواب: ", jame(num1, num2))
    elif choice == '2':
        print("جواب: ", tafrigh(num1, num2))
    elif choice == '3':
        print("جواب: ", zarb(num1, num2))
    elif choice == '4':
        print("جواب: ", taghsim(num1, num2))
    else:
        print("ورودی نامعتبر")
