# Teste de PSI 1 - Turno 1 - Versão 2

## Informação do aluno

    Nome: Artur

Teste termina às 10:45.

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### P1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    bool b = 5 < 2;
    double d = Convert.ToDouble(b);
    
    Console.WriteLine(d);

P1 - Resposta

    Vai ser impresso 0. Vai ser impresso 0 porque, false é representado por 0, e como 5 não é menor que 2 a condição é falsa.

### P2. Considera o seguinte código com um *bug*

    string s = "2.5";
    double d = Convert.ToInt32(s);

    Console.WriteLine(d);

### Indica uma possível correção para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

    Foi necessário trocar o Convert.ToInt32 para double.Parse porque a variavel d é uma double é não é possivel converter um double para int.

### P3. Escreve um programa que solicite ao utilizador dois números inteiros e os multiplique, apresentando o resultado. Caso este seja um número divisível por 3, deve também ser impressa a mensagem "Múltiplo de 3!"

P3 - Resposta

            Console.WriteLine("Insira um numero inteiro");
            string num1 = Console.ReadLine();
            Console.WriteLine("Insira outro numero inteiro");
            string num2 = Console.ReadLine();
            int n1, n2, n3;

            n1 = Convert.ToInt32(num1);
            n2 = Convert.ToInt32(num2);

            n3 = n1 * n2;

            

            Console.WriteLine(n3);

            if (n3 % 3 == 0)
        {
            Console.WriteLine("Múltiplo de 3!");
        }

### P4. Tens um repositório git criado localmente, onde estás no ramo 'master'. Queres associá-lo ao repositório remoto contido no url 'https://github.com/PSI/OMeuRepositorioRemotoV2'. Queres também alterar o nome do ramo atual para 'main'. Deverás enviar os *commits* já feitos localmente para o repositório remoto. Indica os comandos necessários

P4 - Resposta

    git remote add origin https://github.com/PSI/OMeuRepositorioRemotoV2
    git branch -M main
    git push -u origin main

