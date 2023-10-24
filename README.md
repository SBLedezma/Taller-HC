# Taller-HC
def suma(num_1, num_2):
  result = num_1 + num_2
  print(f'{num_1} + {num_2} is equal to {result}')
  return result
def resta(num_1, num_2):
  result = num_1 - num_2
  print(f'{num_1} - {num_2} is equal to {result}')
  return result
def multiplicacion(num_1, num_2):
  result = num_1 * num_2
  print(f'{num_1} * {num_2} is equal to {result}')
  return result
def division(num_1, num_2):
  result = num_1 / num_2
  print(f'{num_1} / {num_2} is equal to {result}')
  return result
def potencia(num_1, num_2):
  result = num_1 ** num_2
  print(f'{num_1} ** {num_2} is equal to {result}')
  return result
def game():
  score = 0
  while True:
    print('======== Menu ========'
          '\n1. Add'
          '\n2. Subtract'
          '\n3. Multiply'
          '\n4. Divide'
          '\n5. Power'
          '\n0. Exit')
    option = int(input('\nChoose an option: '))
    if option == 0:
      break
    num_1 = float(input('Enter first number: '))
    num_2 = float(input('Enter second number: '))
    answer = float(input('Enter your answer: '))
    if option == 1:
      result = suma(num_1, num_2)
      if result == answer:
        score += 1
        print('Correct!!')
      else:
        print('Incorrect')
    elif option == 2:
      result = resta(num_1, num_2)
      if result == answer:
        score += 1
        print('Correct!!')
      else:
        print('Incorrect')
    elif option == 3:
      result = multiplicacion(num_1, num_2)
      if result == answer:
        score += 2
        print('Correct!!')
      else:
        print('Incorrect')
    elif option == 4:
      result = division(num_1, num_2)
      if result == answer:
        score += 2
        print('Correct!!')
      else:
        print('Incorrect')
    elif option == 5:
      result = potencia(num_1, num_2)
      if result == answer:
        score += 4
        print('Correct!!')
      else:
        print('Incorrect')
  print(f'======== Game Over ========'
        f'\nYour score is {score}'
        '\nKeep going!')
game()
