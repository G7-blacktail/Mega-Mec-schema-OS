 # Mega Mec Officina schema - ordem de serviço

Neste projeto eu criei um Diagrama Entidade relacionamento para conceituar o banco de dados de um estabelecimento de mecânicos de carros, onde ela gerará ordens de serviço com data, tipo de serviço, modelo de carros, data de entrega, valor calculado, mecânico responsável, dono do carro.

Primeiramente defini uma entidade pessoa contendo todos os atributos que serão usados para a entidade cliente e mecânico.

Ao definir cliente apenas relacionei que o cliente terá um veiculo associado utilizando uma outra classe chamada veículo e definindo a FK do veiculo ao cliente. 

Após eu criei uma entidade para relacionar o cliente, o veiculo a ordem de serviço o serviço (podendo retornar null caso não haja) e paças (também usando o mesmo critério anterior. Por ultimo defini o Status na entidade Cliente_has_ordem de serviço.

do lado da empresa (Mega Mec) temos a entidade Mecânico onde coloquei os atributos código e especialidade e então criei uma entidade Mecânico_has_ordem de serviço para associar o mecânico a ordem de servço.

Para finalizar criei separadamente duas entidades: serviços (que armazenará o nome, descrição, tipo e valor da mão de obra) e Peças para armazenar o nome o tipo e o valor das peças. 

Assim consigo representar meu mini-mundo contendo todos os dados necessários para armazenar no banco uma ordem de serviço.
