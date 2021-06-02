# Ufal_2020-1_Inteligencia_Artificial_AB2
Sistema Especialista; Migração de Expert Sinta para JavaScript; Entrada formatada; Checkbox


O Projeto é para compor a nota da AB2 da matéria Inteligência Artificial, Ufal - IC - 2020-1 (02/06/2021)

A proposta é apresentar um Sistema Especialista que é réplica do Sistema FITOCANA que já foi criado com o software Expert SINTA. Por isso este projeto é fruto de uma migração.

Pela natureza complexa e pela quantidade de ramificações encontradas no Sistema FITOCANA o escopo desse projeto foi diminuído para que fosse apresentado um sistema mais simples, tanto para o entendimento quanto para a implementação.

Inicialmente obtivemos todas as informações e dados necessários do sistema. Utilizamos uma função do Expert SINTA que exporta os dados no formato texto. Ver o arquivo '01 - fitocana_bcm - Sistema FITOCANA - Arquivo gerado pelo Expert SINTA.txt'.

Em seguida, analisando como funciona o Sistema FITOCANA, identificamos a variável objetivo (doença) para saber quantas conclusões eram possíveis. Rastreamos todas as regras e criamos uma lista contendo o número de regras totais para cada valor da variável objetivo. Ou seja, analisamos quantas regras haviam para cada doença com o intuito de reduzir o escopo. Ver o arquivo '02 - Preparação - Diminuição do escopo.txt'

Após a ordenção das doenças por quantidade de regras, as doenças aceitas no novo escopo foram as que tinham apenas uma única regra, totalizando 04 doenças. Assim, recuperamos todas as variáveis envolvidas nessas 04 conclusões assim como as devidas regras e criamos um banco de dados. Esse banco é um arquivo com dados devidamente formatados para serem lidos pelo novo sistema. Ver o arquivo '03 - Banco de dados.txt'. Esse é o arquivo que deve ser carregado pela aplicação quando é pedido para adicionar o Banco de Dados.

O novo sistema foi criado usando a linguagem JavaScript. Ele contém três funções principais, ler o arquivo do banco de dados, apresentar botões relacionados às variáveis permitindo que o usuário selecione as caractrísticas da amostra da planta e, após selecionadas, imprimir as possíveis conclusões acerca da doença.

Para acessar o sistema basta baixar o repositório e abrir "Fitocana.html" em um navegador. Clicar em "Adicionar..." e escolher o arquivo "03 - Bando de dados.txt". Em seguida pode marcar as caixas de seleção das variáveis e observar o comportamento das regras e da barra de progresso na parte inferior.

![image](https://user-images.githubusercontent.com/32186360/120549433-fb7c4400-c3c9-11eb-9aa1-3d9c50969681.png)
![image](https://user-images.githubusercontent.com/32186360/120549584-2a92b580-c3ca-11eb-8b31-af9e2a6f6527.png)
![image](https://user-images.githubusercontent.com/32186360/120549649-3ed6b280-c3ca-11eb-89c1-f3b50af25f71.png)


Lembrando que a barra de progresso está de acordo com o índice de confiança estabelicido para cada doença.


| Doença   |      CNF      |
|----------|:-------------:|
| estrias cloróticas | 70% |
| estrias pardas | 80% |
| estrias vermelhas | 100% |
| mancha parda | 80% |

Fontes de aprendizagem:

[Geeks for Geeks - Expert Systems](https://www.geeksforgeeks.org/expert-systems/)

[W3School](https://www.w3schools.com)

[Mozilla - Developer - docs - Web](https://developer.mozilla.org/en-US/docs/Web)

[Stack OverFlow 1 - Read text file](https://stackoverflow.com/questions/14446447/how-to-read-a-local-text-file)

[Stack OverFlow 2 - Read text file](https://stackoverflow.com/questions/9196954/how-to-read-line-by-line-of-a-text-area-html-tag)

[Stack OverFlow 3 - Add elements](https://stackoverflow.com/questions/3607291/javascript-and-getelementbyid-for-multiple-elements-with-the-same-id)

[Stack OverFlow 4 - Add elements](https://stackoverflow.com/questions/32848002/how-to-use-javascript-for-loop-to-create-buttons)

[Stack OverFlow 5 - Errors](https://stackoverflow.com/questions/59625312/syntaxerror-string-literal-contains-an-unescaped-line-break)

[Stack OverFlow 6 - Errors](https://stackoverflow.com/questions/10805125/how-to-remove-all-line-breaks-from-a-string)

[Stack OverFlow 7 - Search element](https://stackoverflow.com/questions/6991494/javascript-getelementbyid-based-on-a-partial-string)

[Stack OverFlow 8 - Search element](https://stackoverflow.com/questions/49417210/how-can-i-check-a-checkbox-when-another-checkbox-is-checked-javascript)

[Stack OverFlow 9 - Checkbox](https://stackoverflow.com/questions/21372829/check-checkbox-if-another-checkbox-is-checked/21372895)

[Stack OverFlow 10 - Checkbox](https://stackoverflow.com/questions/65297683/javascript-progress-bar-updating-by-checkboxes)
