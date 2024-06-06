import random

num_x = random.randint(1, 101)
new_game = 'да'
print('Добро пожаловать в числовую УГАДАЙКУ!!! Давай поиграем :)')


def is_valid(input_number):
    if input_number.isdigit() and 1 <= int(input_number) <= 100:
        return True
    else:
        return False


def game_func():
    count = 0
    while True:
        input_number = input('Введи целое число от 1 до 100: ')
        count += 1
        if not is_valid(input_number):
            print('А может быть все-таки введем целое число от 1 до 100?')
            input_number = input()
        if is_valid(input_number):
            input_number = int(input_number)
        if input_number < num_x:
            print('Твое число меньше загаданного, попробуйте еще разок.')
        if input_number > num_x:
            print('Твое число больше загаданного, попробуйте еще разок.')
        if input_number == num_x:
            print('Поздравляю!!! Ты угадал с', count, 'раза!')
            break


game_func()
while True:
    print('Хочешь сыграть еще раз? (да/нет) ')
    answer = input()
    if answer.lower() == 'да':
        print('НОВАЯ ИГРА')
        game_func()
    elif answer.lower() == 'нет':
        print('Спасибо, что играл в числовую угадайку. Еще увидимся...')
        break
    else:
        print('Простите, я вас не понял, так вы хотите поиграть?')
