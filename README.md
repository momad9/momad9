import random

# لیست حیوانات موجود در بازی
animals = ['گربه', 'سگ', 'خرگوش', 'خر', 'موش', 'پرنده', 'پلنگ', 'شیر', 'گوزن', 'پلنگ']

def get_random_animal():
    # برگرداندن یک حیوان تصادفی از لیست
    return random.choice(animals)

def main():
    print("بازی حیوان گم‌شده")
    target_animal = get_random_animal()
    
    while True:
        guess = input("حدس بزنید کدام حیوان گمشده است؟: ")
        
        if guess == target_animal:
            print("تبریک! شما حیوان گم‌شده را پیدا کردید!")
            break
        else:
            print("حیوان گم‌شده درسترسی نیست. مجدد امتحان کنید.")

if __name__ == "__main__":
    main()
