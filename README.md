# GUI4MalSynGen: Para executar o experimento usando a interface grtáfica basta seguir o passo a passo abaixo:

I. Para executar o experimento utilizando a interface, é necessário baixar ou clonar o repositório

II. Após ter o projeto em sua máquina, siga os passos abaixo:
  Abra o terminal.
  Navegue até a pasta “autodroid”.
  Execute o comando ./start.sh.
  
  Observações: 
  1- Caso o script ./start.sh não estiver como executável basta dar esse comando chmod +x start.sh. Faça isso em todos os script ./start.sh caso não consiga executá-los.
  2- Caso apareça a mensagem de ‘permission denied’ quando você tentar  executar o script do ./start.sh, basta dar um sudo su e tentar novamente.
  
  Lembre-se de que, na primeira execução, o download das imagens do Docker pode levar algum tempo, dependendo da velocidade da sua conexão com a internet. Quando o download estiver concluído e o Docker estiver iniciado, o terminal deverá exibir as mensagens relevantes.

III. Em seguida será necessário executar o container do frontend, e para isso siga os passos abaixo:
  Abra um novo terminal.
  Navegue até a pasta raiz do projeto baixado.
  Acesse a pasta “frontend”.
  Execute o script com o comando ./start.sh.

IV. Para acessar a interface, será necessário que você:
  Abra o seu navegador.
  Pesquise http://localhost:3000/ na barra de endereços.

V. Para executar, as campanhas estipuladas,basta seguir esse passo a passo:
  1-Entre em ambiente de execução
	
  2- Para selecionar as campanhas de treinamento, siga os passos abaixo:
      a- No card de parâmetros de treinamento, selecione o custom e preenche com seguintes valores:
      	verbosity: 20
      	dense layer sizes g: 256
      	dense layer sizes d: 256
      	number epochs: 1000
      
      b- Escolha o mesmo dataset que foi usado na primeira etapa. Ele estará presente na pasta chamada Dataset baixada no clone do repositório. O nome do dataset é drebin215_small_64Malwares_64Benign
      
      c- Por fim, clique em “Adicionar” para que esses parâmetros entrem na lista para a execução.
  3- Depois de selecionados as campanhas o card de campanhas deve estar dessa maneira:
  
  Agora para iniciar o treinamento basta clicar no botão iniciar.
  
  4- Após iniciado o treinamento caso não apareça nada em no card processos, basta clicar no botão de refresh que ele mostrar algo como isso:
  
  5- Quando o processo estiver com status com o ícone check basta clicar sobre ele para abrir os resultados.
  
  
  
  6- Na página de resultados, você encontrará os gráficos gerados durante o treinamento do dataset com os parâmetros selecionados. Além disso, se desejar, poderá baixar o dataset treinado.

