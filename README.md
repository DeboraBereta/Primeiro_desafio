# Primeiro_desafio

/* 2. Crie um programa em C# que deverá solicitar a digitação de 10 números, os números digitados deverão ser obrigatoriamente maiores que 50 e menores que 100. Após receber todos os números, o programa deverá limpar a tela e listar os números pares.*/

int[] v = newint[5];
intcont = 0;

Console.WriteLine("Digite 10 números maiores que 50 e menores de 100");

  while (cont< 4) {

    for (int i = 0; i < 5; i++){
      cont++;
      Console.WriteLine("digite o N°:" + cont);
      v[i] = int.Parse(Console.ReadLine());

      if (v[i] <= 49 || v[i] >= 100){
        Console.WriteLine("Erro!! Algo incerido fora do que foi pedido.");
        Console.WriteLine("insira novamente o número dentro do solicitado");
        v[i] = int.Parse(Console.ReadLine());
        break;
      }
    }
  }
  Console.WriteLine("Lista dos números inseridos: ");

  Console.Clear();
  for (int i = 0; i < 5; i++){
    Console.WriteLine("Números pares");
    if (v[i] % 2 == 0){
      Console.WriteLine(v[i]);
    }
  }
 Console.ReadKey();
}
