def calcular(operacao, num1, num2):
  """
  Calcula a operação entre dois números.

  Args:
    operacao: A operação matemática a ser realizada (+, -, *, /).
    num1: O primeiro número.
    num2: O segundo número.

  Returns:
    O resultado da operação.
  """
  if operacao == "+":
    return num1 + num2
  elif operacao == "-":
    return num1 - num2
  elif operacao == "*":
    return num1 * num2
  elif operacao == "/":
    if num2 == 0:
      return "Erro: Divisão por zero!"
    else:
      return num1 / num2
  else:
    return "Operação inválida!"

# Obter os números e a operação do usuário
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
operacao = input("Digite a operação (+, -, *, /): ")

# Calcular o resultado
resultado = calcular(operacao, num1, num2)

# Exibir o resultado
print(f"Resultado: {resultado}")
