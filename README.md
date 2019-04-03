# P3prova2
Prova Programação 3 - 03/04/2019

Sistema iSoccer

  A classe principal do programa é a "Isoccer", que controla todas as funcionalidades do sistema, utiliza o padrão Singleton para garantir que todos os dados do sistema sejam únicos, uma vez que ela armazena todos os dados. A classe "Login" tambem utiliza o Singleton para garantir que apenas uma conta de administrador possa existir, impedindo a classe principal de instanciar outras contas de usuário.
  
  O processo de criação de funcionários utiliza o padrão Factory para que a classe principal não precise se preocupar com o tipo de funcionário que ela está lidando, pois a factory (criadorFuncionario) irá retornar sempre um objeto do tipo Funcionario (programar orientado à interfaces e não à instâncias). Além do fato de que qualquer modificação no processo de criação de funcionários necessitará alterar apenas a classe da factory (CriadorFuncionario) melhorando a manutenibilidade do sistema.
  
  O processo de criação de sócios utiliza o padrão Prototype uma vez que pode haver um grande número de sócios sendo criados, evitando um grande número de instanciações. A priori instanciar sócios não é custoso computacionalmente pois o sistema é simples, mas pensando na extensibilidade, onde ele pode se tornar muito mais complexo, haveria um impacto positivo na eficiência se esse processo de criação exigir um número maior de instruções.
