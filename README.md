# Onde abrir um restaurante italiano em Toronto?

O nosso problema de negócio nesse projeto é identificar possíveis locais onde possa ser interessante abrir um restaurante italiano em Toronto, Canadá. O solicitante deseja que seja o mais perto possível de seu bairro.
Para isso, utilizamos dados do Wikipedia para nomes de regiões e localizações, e principalmente, o site Foursquare, onde coletamos os estabelecimentos que existem nas regiões.
Utilizamos a biblioteca 'request' para acessarmos os dados do arquivo do tipo JSON gerado no API para desenvolvedores do Foursquare.
Com isso, conseguimos identificar os tipos de negócios presentes e mais frequentes em cada bairro, utilizando a técnica de One Hot Encoding.
Foi aplicado o algoritmo KMeans, do pacote ScikitLearn para agruparmos as vizinhanças semelhantes (Clustering) em 5 grupos.
Dentre os bairros que não possuíam nenhum restaurante italiano, listamos os 10 bairros mais próximos de Berczy Park, onde reside o solicitante.
Como resultado, o próprio bairro de Berczy Park não possui restaurantes italianos e, de acordo com a distância e a semelhança determinada na clusterização, selecionamos mais 3 regiões como possíveis escolhas: Richmond/Adelaide/King, Regent Park/Harbourfront and CN Tower/King and Spadina/Railway Lands.
Concluindo, com esse projeto, podemos listar as quatro melhores opções de acordo com as exigências do solicitante, incluindo a própria região onde habita o solicitante, mas a escolha final ainda deve levar em consideração preços de venda/aluguel e pesquisas de mercado.
