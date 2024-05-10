# Cp2-Edge-Computing

Arthur Abonizio RM: 555506
Gustavo Pierre RM:558928
Gabriel Belo RM: 551669
Enzo Vinycius RM: 558225

Descrição do projeto: 
O sistema de monitoramento ambiental é completamente implementado pelo código. A leitura de temperatura e umidade é feita usando o sensor DHT22, a luminosidade é bloqueada com o sensor de luz LDR, alertas sonoros são produzidos pelo buzzer e os dados são exibidos no display LCD.
Depois de importar as bibliotecas LiquidCrystal e DHT, os pinos de conexão para os componentes são configurados e os objetos necessários são criados para interagir com eles.
No início, o programa lê a luminosidade, temperatura e umidade do ambiente, sem usar loop. Com base na análise desses textos, são identificadas três condições fundamentais.
 Condições perfeitas: Pouca luminosidade (<= 250), temperatura de 10 a 15 graus Celsius, e umidade de 50% a 70%. Desta forma, o sistema ativa um LED verde para confirmar as condições ideais e mostra mensagens no display LCD diminuindo a temperatura e umidade corretas.
  Além das normas: Intensidade luminosa elevada (> 250 e <= 400) OU temperatura acima do limite ideal (acima de 15 ou abaixo de 10 graus Celsius). Quando estas situações são identificadas, o sistema aciona um LED amarelo, produz um som de aviso com o buzzer e mostra mensagens no display LCD informando a condição específica (alta luminosidade ou temperatura fora do intervalo).
 Aviso: Intensidade luminosa alta (> 400) ou níveis de umidade abaixo de 50% ou acima de 70% não estão dentro da faixa ideal. Nos momentos de urgência, o sistema acende um LED vermelho, emite um som mais alto com o buzzer e mostra mensagens no display LCD diminuindo problemas com a luz ou a umidade.
Além disso, todas as notificações são enviadas através da porta serial para permitir monitoramento adicional, resultando em um sistema total de monitoramento ambiental com feedback visual e sonoro em tempo real.
