# DesafioTarget
1) 12
2)```
    #include <stdio.h>
    int verificaFibonacci(int num){
        int a = 0, b = 1, c;
        if (num == 0) 
            return 1;
        while (c <= num){
            c = a + b;
            if (c == num) 
                return 1;
            a = b;
            b = c;
        }
        return 0;
    }
    
    int main(void){
        int num;
        printf("Digite um número: ");
        scanf("%d", &num); 
        if (verificaFibonacci(num))
            printf("%d pertence à sequência de Fibonacci.", num);
        else
            printf("%d não pertence à sequência de Fibonacci.", num);  
        return 0;
    }
   ```                
3) 
  a) 9
  b) 128
  c) 49
  d) 100
  e) 13
  f) 200

4) Ligo o primeiro interruptor e deixo ligado por alguns minutos. Depois, ligo o segundo interruptor e deixo ligado. 
   Em seguida, vou para a primeira sala. 
    Se a lâmpada estiver apagada, mas quente, ela pertence ao primeiro interruptor. 
    Se estiver acesa, pertence ao segundo. 
    Se não estiver quente nem acesa, pertence ao terceiro interruptor. 
  Repetindo a mesma lógica de eliminação para a próxima (segunda) lâmpada, posso descobrir qual o é o seu interruptor e também o interruptor da terceira lampada sem nem mesmo vê-la.

5)     
          import java.util.Scanner;
        
          public class Main
          {
          	public static void main(String[] args) {
                  Scanner scanner = new Scanner(System.in);
          
          System.out.print("Digite uma string: ");
          String str = scanner.nextLine();
          
          char[] charArray = str.toCharArray();
          
          int i = 0; 
          int j = str.length() - 1;
          
          while (i < j) {
              char temp = charArray[i];
              charArray[i] = charArray[j];
              charArray[j] = temp;
              i++;
              j--;
          }
          String stringInvertida = new String(charArray);
          System.out.println("String invertida: " + stringInvertida);
          }
      }
