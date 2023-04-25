# Codigos-em-Java


Aprendendo a lógica de JAVA e colocando em prática: 





          //Codigo para saber hora mensal
                    System.out.println("Digite suas horas trabalhadas no dia: ");
                    int hr = sc.nextInt();

                    System.out.println("Digite seus dias trabalhados na semana: ");
                    int ts = sc.nextInt();

                    System.out.println("Digite quantas semana no mês você trabalha: ");
                    int mes = sc.nextInt();

                    int resul = hr * ts * mes;
                    System.out.printf("Você trabalha %d horas no mês!", resul);

          //Codigo para saber salario hora, um complementa o outro

                    float ht,sm,sal;

                    System.out.println("Digite sua hora mensal trabalhada: ");
                    ht = sc.nextFloat();

                    System.out.println("Digite seu salário mensal: ");
                    sm = sc.nextFloat();

                    sal = sm/ht;
                    System.out.printf("Seu salário hora é de: %.2f", sal);

              
              
              
              
             
        // Codigo para calcular a media de 4 alunos 
            
                    String[] nome = new String[4];
                    double[] n1 = new double[4];
                    double[] n2 = new double[4];
                    double[] m = new double[4];

                    Scanner scanner = new Scanner(System.in);

                    for (int i = 0; i < 4; i++) {
                        System.out.println("Aluno " + (i + 1));
                        System.out.print("Nome: ");
                        nome[i] = scanner.nextLine();
                        System.out.print("Primeira nota: ");
                        n1[i] = scanner.nextDouble();
                        System.out.print("Segunda nota: ");
                        n2[i] = scanner.nextDouble();
                        m[i] = (n1[i] + n2[i]) * 2 / 4;
                        scanner.nextLine();
                    }

                    System.out.println("LISTAGEM DE ALUNOS");
                    System.out.println("-------------------");

                    for (int i = 0; i < 4; i++) {
                        System.out.printf(" %-10s %2.1f\n", nome[i], m[i]);
                    }

                    scanner.close();






        //  sistema de votação


                  Scanner sc = new Scanner(System.in);

                          int idade;

                         System.out.print("Qual sua idade? ");
                         idade = sc.nextInt();
                         if (idade<16){
                          System.out.println("Não precisa voltar");
                         }else if(idade>=16 && idade<18) {
                          System.out.println("Seu voto é opcional");
                         }else if(idade>=18 && idade<70) {
                          System.out.println("Voto obrigatório");
                         }else {
                          System.out.println("Voto opcional");
                         }



				//forma com menos condicionais > 

                        int idade;

                System.out.println("Qual sua idade? ");
                       idade = sc.nextInt();
                       if (idade<16){
                         System.out.println("Não vota");
                       } else {
                         if ((idade>=16 && idade<18) || idade>70){ 
                         System.out.println("Voto opcional");
                       } else {
                         System.out.println("Voto obrigatório");
                        }
                      }

                    }

                     }


			//outra forma (mais simplificada) >


                        int idade;

                  System.out.println("Qual sua idade? ");
                       idade = sc.nextInt();
                       if (idade<16){
                         System.out.println("Não vota");
                       } else if ((idade>=16 && idade<18) || idade>70){ 
                         System.out.println("Voto opcional");
                       } else {
                         System.out.println("Voto obrigatório");
                       }

                    
                    
                    
                    
     //Formula de bhaskara 

                        Scanner sc = new Scanner(System.in);

                         int a,b,c;
                         double delta,x1,x2;

                         System.out.println("\nQual é o A, B e C?");
                         System.out.print("A: ");
                         a = sc.nextInt();
                         System.out.print("B: ");
                         b = sc.nextInt();
                         System.out.print("C: ");
                         c = sc.nextInt();

                         delta = Math.pow(b, 2) - 4 * a * c;
                         System.out.println("\nDelta Δ é: " + delta);
                         if (delta < 0){
                           System.out.println(" Não existem raízes");
                         }else{
                           x1 = ((-(b) + Math.sqrt(delta)) / 2 * a);
                           x2 = ((-(b) - Math.sqrt(delta)) / 2 * a); 
                           System.out.println("   x1 =  " + x1);
                           System.out.println("   x2 =  " + x2);
                         }


              
              
              
       // Triângulos 

                          System.out.print("\nSegmento A: ");
                           int a = sc.nextInt();
                           System.out.print("Segmento B: ");
                           int b = sc.nextInt();
                           System.out.print("Segmento C: ");
                           int c = sc.nextInt();
                           if (a<b+c && b<a+c && c<a+b){
                               System.out.println("\nFormam um triângulo");
                               if(a==b && b==c) {
                                System.out.println("    Equilátero");
                               } else if(a!=b && b!=c && a!=c) {
                                System.out.println("    Escaleno");
                               } else {
                                System.out.println("    Isóceles");
                               }
                           } else {
                             System.out.println("Não formam um triângulo");
                           }
              
              
            //Usando WHILE
                         int n, s=0;
                      String resposta;
                      do{
                          System.out.println("Digite um número:  ");
                          n = sc.nextInt();
                          s += n;
                          System.out.println("quer continuar? [S/N] ");
                          resposta = sc.next();
                      }while(resposta.equals("S"));
                        System.out.println("A soma de todos os valores é " + s);
                        
                        
                        
       // Com JOptionPane    *inacabado, tentando terminar*              
                       
                          int n,s=0,quant=0;
                          double media;
                          boolean par;
                          do{
                            n = Integer.parseInt(JOptionPane.showInputDialog(null,"<html>Informe um número <br><br><em>(valor 0 interrompe)</em></html>"));

                            s += n;
                            quant++;
                            par = n % 2 ==0 ;


                          } while(n != 0 );
                          media = (double) s/quant; 
                          JOptionPane.showMessageDialog(null,"<html>Resultado<hr> " + "<br> Somatório: " + s + "</html>" + "\n" + "Média: " + media + "\n" + "Total de pares: " + par );
                         
                         
                         
                         

      //Soma dos n numeros naturais

                    int n;
                    int soma=0;
                    int i;
                    System.out.print("Digite um numero ");
                    n = sc.nextInt();

                    if(n>0){
                      for( i = 0; i<=n; i++)
                      soma += i;
                      System.out.println("Para n = " + i +" a soma é: "+ soma);
                      System.out.println("Pronto! A soma dos "+ n + " primeiros numeros naturais é: " + soma);
                    }else {
                      System.out.println("Somente numeros positivos!");
                    }





          //Descobrir numeros IMPARES

                          int a,b;
                          int i;

                          System.out.print("\n  Digite o nº de onde você quer começar: ");
                          a = sc.nextInt();

                          System.out.print("  O nº onde você quer terminar: ");
                          b = sc.nextInt();

                          System.out.println("  Os nº ímpares entre " + a + " e " + b + " são: ");
                          for(i=a; i<=b; i++){
                            if((i % 2) !=0){
                              System.out.print("\t\t"+i+"\n");
                            }
                          }








     //Saber quantos dias tem o mês e se for bissexto mudar o mês de fev

                            String mes[] = {"Jan","Fev","Mar","Abr","Mai","Jun","Jul","Ago",
                            "Set","Out","Nov","Dez",};

                            int totd[] = {31, 28, 31, 30, 31, 30, 31, 31, 
                            30, 31, 30, 31};

                            int bi[] = {31, 29, 31, 30, 31, 30, 31, 31, 
                              30, 31, 30, 31};

                            int ano;
                            System.out.print("Qual o ano? ");
                            ano = sc.nextInt();


                            if(ano % 4 == 0 && ano % 100 != 0){
                              System.out.print("O ano de " + ano + " é bissexto: " + bi + mes +"\n");
                              for(int i = 0; i<mes.length; i++){
                                System.out.println("\t" + mes[i] + "  tem " + bi[i] + "  dias." );
                              }
                            }else{
                              for(int i = 0; i<mes.length; i++){
                            System.out.println("\t" + mes[i] + "  tem  " + totd[i] + "  dias. ");

                              }
                            }


        //outra forma

                          String mes[] = {"Jan","Fev","Mar","Abr","Mai","Jun","Jul","Ago",
                          "Set","Out","Nov","Dez",};

                          int totd[] = {31, 28, 31, 30, 31, 30, 31, 31, 
                          30, 31, 30, 31};

                          String bi[] = {"31", "-29-", "31", "30", "31", "30", "31", "31", 
                            "30", "31", "30", "31"};

                          int ano;
                          System.out.print("Qual o ano? ");
                          ano = sc.nextInt();


                          if(ano % 4 == 0 && ano % 100 != 0){
                            System.out.print("O ano de " + ano + " é bissexto: \n");
                            for(int i = 0; i<mes.length; i++){
                              System.out.println("\t" + mes[i] + "  tem " + bi[i] + " dias." );
                            }
                          }else{
                            for(int i = 0; i<mes.length; i++){
                          System.out.println("\t" + mes[i] + "  tem  " + totd[i] + "  dias. ");

                            }
                          }



    // 5 números aleátorio e imprimir a soma dos vetores (usando vetor)

                    Random random = new Random();
                     int vetor[] = new int [5];
                     int soma=0;

                     for(int i=0; i<vetor.length; i++){
                     vetor[i] = 0 + random.nextInt(50); //Gera números aleatórios com limite 50 e minimo 0.
                      soma+=vetor[i]; // soma = soma + vetor
                      System.out.println("Vetores: " + vetor[i]);
                     }
                    System.out.println("A soma dos vetores aleatórios é: " + soma);


     // Mostrar 10 numeros e imprimir somente os pares (usando vetor)


                        Random random = new Random();
                         int vetor[] = new int [10];

                         for(int i=0; i<vetor.length; i++){
                          vetor[i] = 0 + random.nextInt(50); //Gera números aleatórios com limite 50 e minimo 0.
                         if (vetor[i] % 2 == 0){
                          System.out.println("pares: " + vetor[i]);
                         }






        // Imprimir 7 nomes em ordem albatéfica 

                              String vetor[] = {"Marco","Paulo","David","Abel","Ivo","Zildo",
                               "Hilton"};
                                for(int i=0; i<vetor.length;i++){
                                 Arrays.sort(vetor);// função para por em ordem alfabética
                                 System.out.println(vetor[i]);
                                }



     // 7 Nomes inseridos pelo usuário e pôr em ordem alfabética: 


                          Random random = new Random();
                           String vetor[] = new String [7];

                            for(int i=0; i<vetor.length;i++){
                             System.out.printf("Digite 7 nomes: %d ", i+1);
                             vetor[i] = sc.nextLine();
                            }
                          Arrays.sort(vetor);// função para por em ordem alfabética
                          for(String nome : vetor){
                            System.out.println("Ordem alfabética:  " + nome);
                          }

    // Código melhorado:: 

                        Random random = new Random();
                         String vetor[] = new String [7];

                          for(int i=0; i<vetor.length;i++){
                           System.out.printf("Digite 7 nomes: (%d) ", i+1);
                           vetor[i] = sc.nextLine();
                          }
                        Arrays.sort(vetor);// função para por em ordem alfabética
                        for(String nome : vetor){
                          int posicao = Arrays.asList(vetor).indexOf(nome) + 1; // cria uma variavel 'posicao' para retornar a posição do nome atual na lista ordenada
                          System.out.printf("\tOrdem alfabética %d:  %s%n", posicao, nome);// %d é um inteiro com valor da variavel 'posicao', %s é uma String com valor 'nome', %n é para pular linha.
                        }






          //Crie um vetor com 5 números e multiplique cada um deles por 2. Imprima o vetor resultante.

                                  int mult;
                                  int vetor[] = new int [5];

                                  for(int i = 0; i<vetor.length; i++){
                                     System.out.printf("Digite 5 números: (%d) ", i+1);
                                     vetor[i] = sc.nextInt();


                                  }
                                  for(int i = 0; i<vetor.length; i++){
                                  mult = vetor[i] * 2;
                                  System.out.println("Multiplicado por 2:  " + mult);
                                  }



           //Código melhorado

                                    int vetor[] = new int [5];
                                    int mult;

                                    for(int i=0; i<vetor.length; i++){
                                    System.out.printf("Digite 5 números: (%d) ", i+1);
                                    vetor[i] = sc.nextInt();
                                    }
                                    System.out.print("\nPor qual número quer multiplicar? ");
                                    int n = sc.nextInt();

                                    System.out.printf("Os 5 números digitados multiplicado por %d: \n", n);
                                    for(int i=0; i<vetor.length; i++){
                                    mult = vetor[i] * n;
                                    System.out.print( mult + " ");
                                    }
                                    System.out.println("\n");



          //Código melhorado do melhorado 2.0 hahaha

                                  int mult;
                                  int vetor[] = new int [5];

                                  for(int i = 0; i<vetor.length; i++){
                                     System.out.printf("Digite 5 números: (%d) ", i+1);
                                     vetor[i] = sc.nextInt();
                                  }

                                  for(int i = 0; i<vetor.length; i++){
                                    System.out.println("");
                                      System.out.printf("Quer multiplicar %d por qual número? ", vetor[i]);
                                      int n = sc.nextInt();
                                      mult = vetor[i] * n;
                                      System.out.printf("  %d Multiplicado por %d:  %s%n\n",vetor[i], n,  mult);
                                  }




















              
