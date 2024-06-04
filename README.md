# Projeto motor.

O código apresentado implementa um sistema de controle de velocidade simples para um motor utilizando um botão como interface. A seguir, uma análise mais aprofundada de cada parte do código:

  *Funcionamento Detalhado:*

  ° Inicialização: Ao iniciar o programa, o código define os pinos do botão e do motor, inicializa as variáveis estado e velocidade e define o motor na velocidade mínima (0).
  
  ° Verificação do Botão: A cada ciclo do loop, o programa verifica o estado do botão. Se o botão estiver pressionado:
  
  ° Incremento da Etapa: A variável estado é incrementada em 1, alterando a etapa da progressão da velocidade.
  
  ° Verificação de Limite: Se a etapa ultrapassar o valor máximo (3), ela é redefinida para 0, iniciando um novo ciclo de progressão.
  
  ° Definição da Velocidade: A variável velocidade é definida com base na etapa atual, determinando a velocidade do motor.
  
  ° Controle do Motor: A função analogWrite() é utilizada para enviar o valor da variável velocidade para o pino do motor, controlando sua velocidade.
  
  ° Atraso: Um atraso de 1 segundo é aplicado para evitar que o botão seja pressionado repetidamente em rápida sucessão.
  
  ° Repetição: O ciclo do loop se repete, verificando o estado do botão e controlando a velocidade do motor de acordo com as etapas definidas.
