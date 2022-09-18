 ## Um problema de treinamento 
 
 Uma empresa tem um programa de treinamento para operadores de máquinas.
 Operadores treinados podem trabalhar como instrutores, assumindo <strong> 10 </strong>
 trainess,mas destes, aempresa aproveira apenas <strong> 7 </strong>.
 Atualmente há <strong> 130 </strong> operadores treinados disponiveis 
 na empresa.
 Eles também são necessários na linha de fabricação. e sabe-se que serão necessários para os próximos meses :
 
  | Janeiro | Fevereiro | Março | Abril |
  |:-------:|:---------:|:-----:|:-----:|
  |   100   |   150     |  200  |  250  |
  
  ## Custos 
  
  Trainees .......................................................$ 400,00
  
  Operador treinado <strong> trabalhando </strong> .......$ 700,00
  
  Operador treinado <strong> ocioso </strong>..................$ 500,00
  
  Desenvolver um modelo PL para encontrar o programa de treinamento de custo mínimo e satisfazer os requisitos da empresa a cada 
  mês.
  
  Umacordo firmado com o sindicato <strong> proibe demissôes </strong> de operadores treinados no periodol.
  
  ## Resolução 
  
  A cada mês um operador treinado está: operando máquina, trabalhando como instrutor, ou está ocioso.Além disto, o n°. de operadores treinados trabalhando nas máquinas é conhecido: 100 em janeiro, 
  150 em fevereiro , 200 em março e 250 em abril. <strong> As variáveis de decisão para o modelo são :
  
  |Operadores| janeiro | Fevereiro | Março |
  |:--------:|:-------:|:---------:|:-----:|
  |Instrutores| x1| x3| x5|
  |ociosos|x2|x4|x6|
  
  
  ## Função objetivo 
  
  "Custo total = custo trainees + custo instrutores + custo ociosos + custo operadores trabalhando em máquinas ".
  
  Min Z = 400 * (10X<sub>1</sub> + 10X<sub>3</sub> + 10X<sub>5</sub>) + 700* (X<sub>1</sub> + X<sub>3</sub> + X<sub>5</sub>)
  
  +500* (X<sub>2</sub> + X<sub>4</sub> + X<sub> 6 </sub>) + 700*(100 + 150 + 200)
          
  Min Z = 4700X<sub>1</sub> + 500X<sub>2</sub> + 4700X<sub>3</sub> + 500X<sub>4</sub> + 4700X<sub>5</sub>
  
  Min Z = 4700X<sub>1</sub> + 500X<sub>2</sub> + 4700X<sub>3</sub> + 500X<sub>4</sub> + 4700<sub>5</sub> + 500X<sub>6</sub> + 315.000
  
  ## Restriçôes 
  
  Equaçâo de balanço mensal:
  
  operadores treinados no inicio do mês = 
  
  operadores nas máquinas + instrutores + ociosos 
  
  Janeiro: 130 = 100 + X<sub>1</sub> + X<sub>2</sub> ↔ X<sub>1</sub> + X<sub>2</sub> = 30
  
  Fevereiro: 130 + 7X<sub>1</sub> = 150 + X<sub>3</sub> + X<sub>4</sub> ↔ 7X<sub>1</sub> - X<sub>3</sub> - X<sub>4</sub> = 20
  
  Março: 130 + 7X<sub>1</sub> + 7X<sub>3</sub> = 200 + X<sub>5</sub> + X<sub>6</sub>
  
  Abril: 250 = 130 + 7X<sub>1</sub> + 7X<sub>3</sub> + 7X<sub>5</sub>
  
  X<sub>1,X<sub>2</sub>,X<sub>3</sub>,X<sub>4</sub>,X<sub>5</sub>,X<sub>6</sub> ≥ 0
  
  Aula 4 10: 30
