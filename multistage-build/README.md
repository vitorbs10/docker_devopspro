## Descrição
Este diretório foi criado para realizar testes com o **Multistage Build** no Docker. Nesse processo, uma aplicação em Golang foi desenvolvida na primeira etapa, gerando um arquivo binário, que posteriormente foi copiado para a segunda etapa. 

O **Multistage Build** é uma abordagem eficiente porque descarta todo o ambiente de construção das etapas intermediárias, preservando apenas o que é explicitamente copiado para a última etapa. Dessa forma, ele garante que a imagem final seja mais enxuta, sem dependências ou arquivos desnecessários.

Neste exemplo, o uso do Multistage Build permitiu reduzir o tamanho da imagem final de aproximadamente **300 MB para apenas 15 MB**, demonstrando como essa técnica contribui para otimizar o uso de recursos e melhorar a performance do ambiente de execução.

Também usei o Target para conseguir testar as outras etapas do Multistage além da final e ter certeza de que todos as etapas estão funcionando corretamente.
