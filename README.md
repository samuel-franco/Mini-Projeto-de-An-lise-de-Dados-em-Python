# Mini-Projeto-de-An-lise-de-Dados-em-Python
Mini Projeto de Análise de Dados na linguagem Python

Mini Projeto de Análise de Dados na Linguagem Python Este mini projeto consiste básicamente fazer tratamentos de dados e treinar habildidades em Python, especificamente na area do desenvolvimento de análise de dados. A ideia do projeto é bem simples, o objetivo é pegar os dados de vendas de uma empresa do ramo de produtos eletrônicos e fazer o tratamento desses dados por meio de passo a passo. Com isso é possivel mostrar com o Python as informações das vendas nas lojas como por exemplo, a quantidade de produtos vendidos, o faturamento qual a loja que mais vendeu. Por último fiz bem simples um gráfico/dashboard para mostrar a performace das lojas.

Passo a passo da solução do Desafio

Atenção LEMBRETE!

Toda vez que eu for resolver algum problema de programação

Tenho que escrever o passo a passo até o final

ou seja é a lógica de programação da solução do problema.

Lógica de programação

Passo 0 - Entender o desafio ou problema para ser resolvido

Passo 1 - Percorrer todos os arquivos da base de dados da pasta (Vendas)

Passo 2 - Importar as bases de dados de vendas

Passo 3 - Tratar / compilar a base de dados

Passo 4 - Calcular o produtor mais vendido (em quantidade)

Passo 5 - Calcular o produtor que mais faturou (em faturamento)

Passo 6 - Calcular a loja/cidade que mais vendeu (faturamento) - criar gráfico/dashboard

Uma outra forma de exibir os arquivos da pasta vendas é

É usar em vez da função print() usar a função display(). A função display faz a mesma coisa que função print. A diferença é que o display deixa o código mais clean



![image](https://user-images.githubusercontent.com/84928607/232652172-1e62fd1d-49bf-456a-86eb-8fcd87427d0c.png)


![image](https://user-images.githubusercontent.com/84928607/232652313-00bcf92b-9193-4217-b9b0-de311ab7e548.png)


|index|Unnamed: 0|SKU|Produto|Quantidade Vendida|Primeiro Nome|Sobrenome|Data|Loja|Preco Unitario|Unnamed: 8|Faturamento|
|---|---|---|---|---|---|---|---|---|---|---|---|
|0|8|HL4379|Televisão|4|Jessica|Cordovil|2/11/2018|Rio de Janeiro|2500|NaN|10000|
|1|12|HL1918|iPhone|2|Camilla|Guimarães|10/4/2018|Rio de Janeiro|5300|NaN|10600|
|2|21|HL4379|Televisão|5|Katharina|Barros|3/26/2018|Rio de Janeiro|2500|NaN|12500|
|3|39|HL9962|Android|1|Rodrigo|Silva|1/14/2018|Rio de Janeiro|3400|NaN|3400|
|4|41|HL4379|Televisão|3|Júlio|Freire|6/30/2018|Rio de Janeiro|2500|NaN|7500|
|5|63|HL1148|Câmera|5|Jackson|Derossi|11/30/2018|Rio de Janeiro|2100|NaN|10500|
|6|65|HL1148|Câmera|1|Willian|Albino|1/30/2018|Rio de Janeiro|2100|NaN|2100|
|7|72|HL2714|Tablet|4|Jéssica|Resinente|2/26/2018|Rio de Janeiro|1600|NaN|6400|
|8|73|HL1918|iPhone|3|Stephanie|Gonçalves|9/24/2018|Rio de Janeiro|5300|NaN|15900|
|9|76|HL8851|Notebook|1|Guilherme|Vianna|4/24/2018|Rio de Janeiro|3500|NaN|3500|
|10|77|HL7348|SmartWatch|5|Thiago|Lima|1/29/2018|Rio de Janeiro|1400|NaN|7000|
|11|82|HL1918|iPhone|3|Livia|Codeceira|1/8/2018|Rio de Janeiro|5300|NaN|15900|
|12|88|HL1918|iPhone|3|Victoria|Tavares|9/15/2018|Rio de Janeiro|5300|NaN|15900|
|13|93|HL1918|iPhone|1|João|Aires|10/2/2018|Rio de Janeiro|5300|NaN|5300|
|14|99|HL1148|Câmera|4|Lucas|Aragão|3/24/2018|Rio de Janeiro|2100|NaN|8400|
|15|102|HL1148|Câmera|3|Carolina|Rocha|2/7/2018|Rio de Janeiro|2100|NaN|6300|
|16|103|HL4379|Televisão|1|Caio|Fernandes|7/25/2018|Rio de Janeiro|2500|NaN|2500|
|17|115|HL4379|Televisão|2|Roberta|Pimenta|10/17/2018|Rio de Janeiro|2500|NaN|5000|
|18|121|HL1918|iPhone|1|Raphael|Guedes|7/12/2018|Rio de Janeiro|5300|NaN|5300|
|19|124|HL4379|Televisão|1|David|Assumpção|4/7/2018|Rio de Janeiro|2500|NaN|2500|
|20|153|HL1148|Câmera|1|Aline|Morais|9/14/2018|Rio de Janeiro|2100|NaN|2100|
|21|158|HL1918|iPhone|1|Thais|Rodrigues|3/23/2018|Rio de Janeiro|5300|NaN|5300|
|22|167|HL4379|Televisão|3|João|Rodrigues|1/25/2018|Rio de Janeiro|2500|NaN|7500|
|23|168|HL1918|iPhone|5|Stephanie|Gonçalves|12/1/2018|Rio de Janeiro|5300|NaN|26500|
|24|171|HL4379|Televisão|5|Pedro|Sena|7/22/2018|Rio de Janeiro|2500|NaN|12500|
|25|174|HL2714|Tablet|2|Philipe|Morete|7/11/2018|Rio de Janeiro|1600|NaN|3200|
|26|175|HL4379|Televisão|2|Larissa|Florim|3/11/2018|Rio de Janeiro|2500|NaN|5000|
|27|178|HL4379|Televisão|4|Platini|Heimlich|8/4/2018|Rio de Janeiro|2500|NaN|10000|
|28|183|HL9962|Android|5|Gustavo|Azevedo|5/2/2018|Rio de Janeiro|3400|NaN|17000|
|29|185|HL2714|Tablet|4|Isabelle|Firmino|12/16/2018|Rio de Janeiro|1600|NaN|6400|
|30|188|HL1148|Câmera|4|Caio|Silva|1/24/2018|Rio de Janeiro|2100|NaN|8400|
|31|190|HL4379|Televisão|5|Adriana|Carneiro|7/15/2018|Rio de Janeiro|2500|NaN|12500|
|32|201|HL1918|iPhone|2|Brenno|Santos|9/1/2018|Rio de Janeiro|5300|NaN|10600|
|33|207|HL8851|Notebook|1|Gabrielle|Vasconcelos|6/14/2018|Rio de Janeiro|3500|NaN|3500|
|34|208|HL4379|Televisão|1|Marcela|Medeiros|12/1/2018|Rio de Janeiro|2500|NaN|2500|
|35|212|HL7348|SmartWatch|4|Eric|Carvalho|12/25/2018|Rio de Janeiro|1400|NaN|5600|
|36|219|HL8851|Notebook|2|Thales|Santos|10/15/2018|Rio de Janeiro|3500|NaN|7000|
|37|227|HL1918|iPhone|2|Adrielle|Vieira|8/9/2018|Rio de Janeiro|5300|NaN|10600|
|38|237|HL1148|Câmera|2|Pedro|Santos|4/24/2018|Rio de Janeiro|2100|NaN|4200|
|39|242|HL9962|Android|1|Camilla|Vieira|12/28/2018|Rio de Janeiro|3400|NaN|3400|
|40|249|HL9962|Android|3|Roberta|Teixeira|7/12/2018|Rio de Janeiro|3400|NaN|10200|
|41|257|HL1918|iPhone|1|João|Silva|10/6/2018|Rio de Janeiro|5300|NaN|5300|
|42|258|HL1918|iPhone|3|Eduardo|Veiga|8/21/2018|Rio de Janeiro|5300|NaN|15900|
|43|259|HL1148|Câmera|3|Wilson|Brandão|4/24/2018|Rio de Janeiro|2100|NaN|6300|
|44|269|HL1918|iPhone|1|Katharina|Barros|12/14/2018|Rio de Janeiro|5300|NaN|5300|
|45|284|HL4379|Televisão|5|Marcelo|Guadagnino|10/22/2018|Rio de Janeiro|2500|NaN|12500|
|46|295|HL1918|iPhone|4|Victor|Zakhm|1/9/2018|Rio de Janeiro|5300|NaN|21200|
|47|297|HL7348|SmartWatch|3|Isabella|Rodrigues|7/16/2018|Rio de Janeiro|1400|NaN|4200|
|48|306|HL1148|Câmera|5|Natalia|Andrade|9/5/2018|Rio de Janeiro|2100|NaN|10500|
|49|308|HL4379|Televisão|3|Pedro|Lyra|10/25/2018|Rio de Janeiro|2500|NaN|7500|
|50|310|HL4379|Televisão|2|Sandy|Figueiredo|7/15/2018|Rio de Janeiro|2500|NaN|5000|
|51|311|HL1918|iPhone|5|Ana|Silva|6/23/2018|Rio de Janeiro|5300|NaN|26500|
|52|324|HL1148|Câmera|2|Victor|Lira|5/28/2018|Rio de Janeiro|2100|NaN|4200|
|53|334|HL4379|Televisão|5|William|Mendonça|11/25/2018|Rio de Janeiro|2500|NaN|12500|
|54|336|HL1148|Câmera|4|Letícia|Leal|11/10/2018|Rio de Janeiro|2100|NaN|8400|
|55|348|HL4379|Televisão|2|Norman|Jimbo|11/15/2018|Rio de Janeiro|2500|NaN|5000|
|56|351|HL2714|Tablet|4|Carolina|Carneiro|8/10/2018|Rio de Janeiro|1600|NaN|6400|
|57|352|HL1918|iPhone|3|Raísa|Rodrigues|10/27/2018|Rio de Janeiro|5300|NaN|15900|
|58|353|HL1918|iPhone|3|Elena|Barreto|8/4/2018|Rio de Janeiro|5300|NaN|15900|
|59|362|HL1148|Câmera|1|Eduardo|Soares|2/15/2018|Rio de Janeiro|2100|NaN|2100|
|60|363|HL2714|Tablet|4|Bruna|Soares|3/28/2018|Rio de Janeiro|1600|NaN|6400|
|61|364|HL4379|Televisão|1|Arthur|Fernandes|9/2/2018|Rio de Janeiro|2500|NaN|2500|
|62|374|HL4379|Televisão|1|Gabriel|Brito|3/7/2018|Rio de Janeiro|2500|NaN|2500|
|63|378|HL2714|Tablet|4|Alon|Palmeira|10/23/2018|Rio de Janeiro|1600|NaN|6400|
|64|379|HL9962|Android|3|Anna|Figueiredo|5/16/2018|Rio de Janeiro|3400|NaN|10200|
|65|389|HL1918|iPhone|5|Cézar|Santos|10/11/2018|Rio de Janeiro|5300|NaN|26500|
|66|390|HL4379|Televisão|4|Izabel|Miura|10/27/2018|Rio de Janeiro|2500|NaN|10000|
|67|404|HL1918|iPhone|4|Gustavo|Aragão|5/22/2018|Rio de Janeiro|5300|NaN|21200|
|68|414|HL1918|iPhone|1|David|Vasconcelos|1/29/2018|Rio de Janeiro|5300|NaN|5300|
|69|418|HL7348|SmartWatch|4|Victor|Oliveira|9/7/2018|Rio de Janeiro|1400|NaN|5600|
|70|435|HL4379|Televisão|1|Maria|Gasperi|8/25/2018|Rio de Janeiro|2500|NaN|2500|
|71|446|HL9962|Android|2|Rachel|Restum|8/22/2018|Rio de Janeiro|3400|NaN|6800|
|72|451|HL2714|Tablet|1|Fabio|Ramos|12/15/2018|Rio de Janeiro|1600|NaN|1600|
|73|456|HL1918|iPhone|4|Carolina|Brum|4/27/2018|Rio de Janeiro|5300|NaN|21200|
|74|469|HL2714|Tablet|1|Thainá|Binello|5/25/2018|Rio de Janeiro|1600|NaN|1600|
|75|487|HL4379|Televisão|2|Luiz|Freire|1/20/2018|Rio de Janeiro|2500|NaN|5000|
|76|516|HL7348|SmartWatch|1|Tayla|Lima|11/9/2018|Rio de Janeiro|1400|NaN|1400|
|77|528|HL7348|SmartWatch|4|Milena|Pereira|6/8/2018|Rio de Janeiro|1400|NaN|5600|
|78|531|HL4379|Televisão|2|Mayara|Soares|11/5/2018|Rio de Janeiro|2500|NaN|5000|
|79|539|HL4379|Televisão|5|Rogério|Gentile|3/13/2018|Rio de Janeiro|2500|NaN|12500|
|80|544|HL2714|Tablet|3|Gabriel|Thoni|10/22/2018|Rio de Janeiro|1600|NaN|4800|
|81|549|HL2714|Tablet|4|Thales|Santos|2/24/2018|Rio de Janeiro|1600|NaN|6400|
|82|558|HL8851|Notebook|2|David|Campelo|9/2/2018|Rio de Janeiro|3500|NaN|7000|
|83|561|HL4379|Televisão|1|Paula|Cavalcanti|11/7/2018|Rio de Janeiro|2500|NaN|2500|
|84|563|HL1148|Câmera|4|William|Mendonça|2/12/2018|Rio de Janeiro|2100|NaN|8400|
|85|571|HL1918|iPhone|3|Antonio|Manhães|10/12/2018|Rio de Janeiro|5300|NaN|15900|
|86|577|HL7348|SmartWatch|1|Carolina|Bernardes|10/30/2018|Rio de Janeiro|1400|NaN|1400|
|87|587|HL9962|Android|4|Matheus|Tostes|11/21/2018|Rio de Janeiro|3400|NaN|13600|
|88|626|HL2714|Tablet|1|Joao|Pereira|5/14/2018|Rio de Janeiro|1600|NaN|1600|
|89|628|HL8851|Notebook|4|Vitor|Arruda|6/1/2018|Rio de Janeiro|3500|NaN|14000|
|90|638|HL9962|Android|2|Fernanda|Bhering|1/30/2018|Rio de Janeiro|3400|NaN|6800|
|91|645|HL9962|Android|2|Luíza|Goulart|6/14/2018|Rio de Janeiro|3400|NaN|6800|
|92|653|HL7348|SmartWatch|2|David|Vasconcelos|6/23/2018|Rio de Janeiro|1400|NaN|2800|
|93|654|HL9962|Android|2|Antônio|Soares|9/18/2018|Rio de Janeiro|3400|NaN|6800|
|94|659|HL1918|iPhone|1|Caroline|Delgado|3/11/2018|Rio de Janeiro|5300|NaN|5300|
|95|661|HL1148|Câmera|2|Guilherme|Jordao|3/19/2018|Rio de Janeiro|2100|NaN|4200|
|96|664|HL7348|SmartWatch|5|Vanessa|Rodrigues|4/30/2018|Rio de Janeiro|1400|NaN|7000|
|97|672|HL1918|iPhone|4|Joyce|Souza|12/11/2018|Rio de Janeiro|5300|NaN|21200|
|98|673|HL9962|Android|5|Roberto|Nogueira|3/31/2018|Rio de Janeiro|3400|NaN|17000|
|99|675|HL9962|Android|2|Rogério|Gentile|8/2/2018|Rio de Janeiro|3400|NaN|6800|
|100|678|HL9962|Android|3|Pedro|Santos|5/16/2018|Rio de Janeiro|3400|NaN|10200|
|101|681|HL4379|Televisão|5|Luis|Garcia|8/10/2018|Rio de Janeiro|2500|NaN|12500|
|102|684|HL4379|Televisão|2|Fernanda|Silva|6/11/2018|Rio de Janeiro|2500|NaN|5000|
|103|686|HL9962|Android|1|Wellington|Duarte|11/24/2018|Rio de Janeiro|3400|NaN|3400|
|104|688|HL4379|Televisão|2|Manuela|Ferreira|2/23/2018|Rio de Janeiro|2500|NaN|5000|
|105|692|HL9962|Android|4|Iuri|Barbosa|2/6/2018|Rio de Janeiro|3400|NaN|13600|
|106|696|HL1148|Câmera|4|Anderson|Cavalcanti|7/22/2018|Rio de Janeiro|2100|NaN|8400|
|107|697|HL1918|iPhone|1|Marina|Gama|11/20/2018|Rio de Janeiro|5300|NaN|5300|
|108|706|HL7348|SmartWatch|5|Rodrigo|Ramos|6/27/2018|Rio de Janeiro|1400|NaN|7000|
|109|710|HL7348|SmartWatch|4|Ana|Leite|7/27/2018|Rio de Janeiro|1400|NaN|5600|
|110|711|HL4379|Televisão|1|Lenon|Fernandes|9/15/2018|Rio de Janeiro|2500|NaN|2500|
|111|715|HL1918|iPhone|5|Izabel|Miura|11/10/2018|Rio de Janeiro|5300|NaN|26500|
|112|720|HL2714|Tablet|3|Guilherme|Barbosa|4/19/2018|Rio de Janeiro|1600|NaN|4800|
|113|733|HL1918|iPhone|3|David|Vasconcelos|8/18/2018|Rio de Janeiro|5300|NaN|15900|
|114|735|HL1918|iPhone|2|Beatriz|Silva|12/14/2018|Rio de Janeiro|5300|NaN|10600|
|115|739|HL7348|SmartWatch|1|Manuela|Ferreira|7/15/2018|Rio de Janeiro|1400|NaN|1400|
|116|742|HL1918|iPhone|4|Danilo|Rubim|5/24/2018|Rio de Janeiro|5300|NaN|21200|
|117|748|HL1918|iPhone|1|Aline|Morais|4/29/2018|Rio de Janeiro|5300|NaN|5300|
|118|757|HL9962|Android|2|Giuseppe|Bhering|12/16/2018|Rio de Janeiro|3400|NaN|6800|
|119|760|HL7348|SmartWatch|3|Marina|Delgado|1/23/2018|Rio de Janeiro|1400|NaN|4200|
|120|771|HL7348|SmartWatch|2|Julia|Leite|1/2/2018|Rio de Janeiro|1400|NaN|2800|
|121|777|HL4379|Televisão|5|Raphael|Guedes|6/21/2018|Rio de Janeiro|2500|NaN|12500|
|122|783|HL1148|Câmera|2|Carlos|Azevedo|10/5/2018|Rio de Janeiro|2100|NaN|4200|
|123|788|HL1918|iPhone|2|Jonatas|Essaber|5/23/2018|Rio de Janeiro|5300|NaN|10600|
|124|791|HL1148|Câmera|2|Pedro|Santos|12/28/2018|Rio de Janeiro|2100|NaN|4200|
|125|813|HL8851|Notebook|5|Antônio|Oliveira|8/4/2018|Rio de Janeiro|3500|NaN|17500|
|126|824|HL1918|iPhone|4|Anízio|Carvalho|7/26/2018|Rio de Janeiro|5300|NaN|21200|
|127|834|HL4379|Televisão|1|Priscila|Carvalho|12/1/2018|Rio de Janeiro|2500|NaN|2500|
|128|846|HL1918|iPhone|1|Wendela|Veloso|1/13/2018|Rio de Janeiro|5300|NaN|5300|
|129|854|HL4379|Televisão|4|Eduardo|Veiga|7/27/2018|Rio de Janeiro|2500|NaN|10000|
|130|889|HL4379|Televisão|1|Fernanda|Coutinho|6/26/2018|Rio de Janeiro|2500|NaN|2500|
|131|910|HL1148|Câmera|4|Wilson|Meirelles|3/28/2018|Rio de Janeiro|2100|NaN|8400|
|132|913|HL1918|iPhone|3|Carlos|Portela|2/23/2018|Rio de Janeiro|5300|NaN|15900|
|133|919|HL1918|iPhone|3|Leandro|Melo|5/6/2018|Rio de Janeiro|5300|NaN|15900|
|134|929|HL1148|Câmera|3|Jessica|Ferreira|11/11/2018|Rio de Janeiro|2100|NaN|6300|
|135|941|HL2714|Tablet|5|Andressa|Rotsztejn|2/6/2018|Rio de Janeiro|1600|NaN|8000|
|136|943|HL8851|Notebook|5|João|Rodrigues|3/25/2018|Rio de Janeiro|3500|NaN|17500|
|137|945|HL7348|SmartWatch|5|Gabriel|Rubim|9/15/2018|Rio de Janeiro|1400|NaN|7000|
|138|949|HL1918|iPhone|4|Sthefeson|Kohn|12/7/2018|Rio de Janeiro|5300|NaN|21200|
|139|963|HL8851|Notebook|5|Guilherme|Castilho|11/1/2018|Rio de Janeiro|3500|NaN|17500|
|140|970|HL4379|Televisão|5|Patrícia|Ferreira|8/14/2018|Rio de Janeiro|2500|NaN|12500|
|141|973|HL9962|Android|5|Cícero|Lima|10/27/2018|Rio de Janeiro|3400|NaN|17000|
|142|975|HL8851|Notebook|4|Mariana|Miranda|5/11/2018|Rio de Janeiro|3500|NaN|14000|
|143|976|HL1918|iPhone|5|Rebeca|Taylor|7/14/2018|Rio de Janeiro|5300|NaN|26500|
|144|979|HL8851|Notebook|1|Jéssica|Teixeira|2/11/2018|Rio de Janeiro|3500|NaN|3500|
|145|991|HL1918|iPhone|1|Carolina|Figueiredo|2/6/2018|Rio de Janeiro|5300|NaN|5300|
|146|997|HL4379|Televisão|3|Thomáz|Vannier|11/26/2018|Rio de Janeiro|2500|NaN|7500|
|147|998|HL1918|iPhone|3|Giulia|Lopes|10/23/2018|Rio de Janeiro|5300|NaN|15900|
|148|1003|HL1918|iPhone|3|Breno|Caputo|8/28/2018|Rio de Janeiro|5300|NaN|15900|
|149|1006|HL7348|SmartWatch|3|Rafael|Ramos|1/10/2018|Rio de Janeiro|1400|NaN|4200|
|150|1008|HL1918|iPhone|5|Brenno|Santos|12/5/2018|Rio de Janeiro|5300|NaN|26500|
|151|1029|HL8851|Notebook|3|Fernanda|Ferreira|10/3/2018|Rio de Janeiro|3500|NaN|10500|
|152|1030|HL1148|Câmera|3|Jorge|Carvalho|10/2/2018|Rio de Janeiro|2100|NaN|6300|
|153|1038|HL4379|Televisão|5|Marcela|Gasperi|1/12/2018|Rio de Janeiro|2500|NaN|12500|
|154|1045|HL1918|iPhone|1|Mariana|Baptista|1/19/2018|Rio de Janeiro|5300|NaN|5300|
|155|1058|HL4379|Televisão|3|Thayane|Resende|5/16/2018|Rio de Janeiro|2500|NaN|7500|
|156|1059|HL7348|SmartWatch|2|Mateus|Polastri|8/16/2018|Rio de Janeiro|1400|NaN|2800|
|157|1064|HL2714|Tablet|1|Bianca|Procaci|1/23/2018|Rio de Janeiro|1600|NaN|1600|
|158|1065|HL1918|iPhone|5|Anderson|Barreto|5/27/2018|Rio de Janeiro|5300|NaN|26500|
|159|1068|HL1148|Câmera|5|Carlos|Mesquita|10/31/2018|Rio de Janeiro|2100|NaN|10500|
|160|1083|HL2714|Tablet|4|Caio|Ferreira|9/16/2018|Rio de Janeiro|1600|NaN|6400|
|161|1087|HL9962|Android|5|Marcela|Medeiros|10/5/2018|Rio de Janeiro|3400|NaN|17000|
|162|1090|HL4379|Televisão|1|Danilo|Rubim|10/27/2018|Rio de Janeiro|2500|NaN|2500|
|163|1096|HL1918|iPhone|4|Livia|Codeceira|2/9/2018|Rio de Janeiro|5300|NaN|21200|
|164|1121|HL8851|Notebook|3|Michelle|Figueiredo|6/20/2018|Rio de Janeiro|3500|NaN|10500|
|165|1134|HL7348|SmartWatch|2|Mônica|Rotolo|11/15/2018|Rio de Janeiro|1400|NaN|2800|
|166|1141|HL2714|Tablet|3|Júlia|Almeida|7/27/2018|Rio de Janeiro|1600|NaN|4800|
|167|1160|HL2714|Tablet|2|Wen|Braga|12/17/2018|Rio de Janeiro|1600|NaN|3200|
|168|1167|HL8851|Notebook|2|Clara|Bruno|11/12/2018|Rio de Janeiro|3500|NaN|7000|
|169|1168|HL4379|Televisão|5|Lucas|Rocha|12/25/2018|Rio de Janeiro|2500|NaN|12500|
|170|1171|HL7348|SmartWatch|3|Melissa|Nucci|4/4/2018|Rio de Janeiro|1400|NaN|4200|
|171|1173|HL1918|iPhone|4|Paula|Calbucci|10/8/2018|Rio de Janeiro|5300|NaN|21200|
|172|1176|HL1148|Câmera|3|Bruna|Silva|10/8/2018|Rio de Janeiro|2100|NaN|6300|
|173|1177|HL1918|iPhone|1|Leandro|Melo|10/5/2018|Rio de Janeiro|5300|NaN|5300|
|174|1178|HL1918|iPhone|1|Cézar|Santos|7/10/2018|Rio de Janeiro|5300|NaN|5300|
|175|1185|HL1918|iPhone|1|Isabella|Montanholi|6/26/2018|Rio de Janeiro|5300|NaN|5300|
|176|1193|HL4379|Televisão|2|Matheus|Gomes|7/18/2018|Rio de Janeiro|2500|NaN|5000|
|177|1197|HL2714|Tablet|4|Bruno|Silva|1/7/2018|Rio de Janeiro|1600|NaN|6400|
|178|1202|HL4379|Televisão|4|João|Tabet|11/30/2018|Rio de Janeiro|2500|NaN|10000|
|179|1207|HL1918|iPhone|2|Caio|Vianna|1/28/2018|Rio de Janeiro|5300|NaN|10600|
|180|1208|HL1918|iPhone|1|Isabelle|Gonçalves|4/17/2018|Rio de Janeiro|5300|NaN|5300|
|181|1209|HL1918|iPhone|2|Pedro|Bitencourt|5/25/2018|Rio de Janeiro|5300|NaN|10600|
|182|1220|HL7348|SmartWatch|5|Thiago|Costa|1/17/2018|Rio de Janeiro|1400|NaN|7000|
|183|1228|HL4379|Televisão|3|Matheus|Tostes|5/9/2018|Rio de Janeiro|2500|NaN|7500|
|184|1232|HL8851|Notebook|2|Julia|Silva|5/27/2018|Rio de Janeiro|3500|NaN|7000|
|185|1236|HL1918|iPhone|1|Thays|Castro|4/3/2018|Rio de Janeiro|5300|NaN|5300|
|186|1244|HL9962|Android|2|Maurício|Dias|4/30/2018|Rio de Janeiro|3400|NaN|6800|
|187|1264|HL7348|SmartWatch|4|Alexandre|Rodriguez|8/3/2018|Rio de Janeiro|1400|NaN|5600|
|188|1266|HL7348|SmartWatch|4|Guilherme|Vianna|10/25/2018|Rio de Janeiro|1400|NaN|5600|
|189|1271|HL7348|SmartWatch|3|Priscila|Carvalho|7/13/2018|Rio de Janeiro|1400|NaN|4200|
|190|1280|HL7348|SmartWatch|3|Amanda|Procaci|10/20/2018|Rio de Janeiro|1400|NaN|4200|
|191|1286|HL1148|Câmera|4|Pedro|Lyra|6/24/2018|Rio de Janeiro|2100|NaN|8400|
|192|1290|HL7348|SmartWatch|2|Joyce|Souza|9/24/2018|Rio de Janeiro|1400|NaN|2800|
|193|1300|HL4379|Televisão|3|Rebeca|Reis|7/1/2018|Rio de Janeiro|2500|NaN|7500|
|194|1332|HL9962|Android|5|Tadeu|Sousa|7/9/2018|Rio de Janeiro|3400|NaN|17000|
|195|1338|HL8851|Notebook|1|Patrícia|Fernandes|1/10/2018|Rio de Janeiro|3500|NaN|3500|
|196|1340|HL1148|Câmera|5|Sandy|Moreira|9/28/2018|Rio de Janeiro|2100|NaN|10500|
|197|1343|HL4379|Televisão|3|Marcelo|Borges|8/13/2018|Rio de Janeiro|2500|NaN|7500|
|198|1348|HL1918|iPhone|2|Lunna|Vannier|5/19/2018|Rio de Janeiro|5300|NaN|10600|
|199|1352|HL4379|Televisão|2|Raísa|Rodrigues|9/23/2018|Rio de Janeiro|2500|NaN|5000|
|200|1354|HL4379|Televisão|5|Chan|Santos|11/6/2018|Rio de Janeiro|2500|NaN|12500|
|201|1355|HL4379|Televisão|3|Elaine|Santos|5/30/2018|Rio de Janeiro|2500|NaN|7500|
|202|1363|HL1148|Câmera|3|David|Campelo|12/11/2018|Rio de Janeiro|2100|NaN|6300|
|203|1367|HL2714|Tablet|5|Victoria|Mazza|9/22/2018|Rio de Janeiro|1600|NaN|8000|
|204|1372|HL8851|Notebook|3|Vanessa|Neves|11/15/2018|Rio de Janeiro|3500|NaN|10500|
|205|1375|HL1148|Câmera|3|Stephanie|Gonçalves|9/16/2018|Rio de Janeiro|2100|NaN|6300|
|206|1379|HL9962|Android|2|Felipe|Mendonça|6/27/2018|Rio de Janeiro|3400|NaN|6800|
|207|1380|HL1918|iPhone|4|Bruna|Londero|4/5/2018|Rio de Janeiro|5300|NaN|21200|
|208|1382|HL1918|iPhone|3|Wilson|Vianna|11/22/2018|Rio de Janeiro|5300|NaN|15900|
|209|1383|HL4379|Televisão|1|Raphael|Kurtz|11/24/2018|Rio de Janeiro|2500|NaN|2500|
|210|1389|HL9962|Android|1|Lucas|Assunção|7/26/2018|Rio de Janeiro|3400|NaN|3400|
|211|1390|HL4379|Televisão|1|Caio|Moraes|6/28/2018|Rio de Janeiro|2500|NaN|2500|
|212|1391|HL2714|Tablet|5|Alex|Fernandes|10/24/2018|Rio de Janeiro|1600|NaN|8000|
|213|1400|HL8851|Notebook|2|Caio|Ferreira|6/21/2018|Rio de Janeiro|3500|NaN|7000|
|214|1406|HL9962|Android|5|Ana|Gonzaga|7/15/2018|Rio de Janeiro|3400|NaN|17000|
|215|1408|HL1918|iPhone|2|Bernardo|Nauenberg|6/20/2018|Rio de Janeiro|5300|NaN|10600|
|216|1421|HL1918|iPhone|4|Diogo|Ressurreição|5/19/2018|Rio de Janeiro|5300|NaN|21200|
|217|1427|HL4379|Televisão|2|Livia|Corrêa|9/10/2018|Rio de Janeiro|2500|NaN|5000|
|218|1438|HL1918|iPhone|4|Marina|Perdomo|11/8/2018|Rio de Janeiro|5300|NaN|21200|
|219|1439|HL8851|Notebook|2|Matheus|Miranda|2/2/2018|Rio de Janeiro|3500|NaN|7000|
|220|1440|HL7348|SmartWatch|4|Matheus|Silva|5/28/2018|Rio de Janeiro|1400|NaN|5600|
|221|1466|HL1918|iPhone|3|Adriana|Carneiro|9/20/2018|Rio de Janeiro|5300|NaN|15900|
|222|1467|HL1918|iPhone|1|Ana|Bôas|8/24/2018|Rio de Janeiro|5300|NaN|5300|
|223|1468|HL1918|iPhone|5|José|Marques|12/18/2018|Rio de Janeiro|5300|NaN|26500|
|224|1470|HL1918|iPhone|3|Arthur|Rocha|1/27/2018|Rio de Janeiro|5300|NaN|15900|
|225|1473|HL1918|iPhone|1|Yasmim|Bittencourt|1/11/2018|Rio de Janeiro|5300|NaN|5300|
|226|1474|HL1918|iPhone|5|Victor|Lira|2/19/2018|Rio de Janeiro|5300|NaN|26500|
|227|1475|HL7348|SmartWatch|1|João|Silva|11/23/2018|Rio de Janeiro|1400|NaN|1400|
|228|1476|HL4379|Televisão|5|Paula|Carneiro|11/5/2018|Rio de Janeiro|2500|NaN|12500|
|229|1481|HL4379|Televisão|4|Daniela|Andrada|10/20/2018|Rio de Janeiro|2500|NaN|10000|
|230|1484|HL1148|Câmera|3|Roger|Rosa|5/18/2018|Rio de Janeiro|2100|NaN|6300|
|231|1487|HL1148|Câmera|3|Joao|Pereira|3/20/2018|Rio de Janeiro|2100|NaN|6300|
|232|1491|HL9962|Android|2|Rafael|Rocha|12/9/2018|Rio de Janeiro|3400|NaN|6800|
|233|1498|HL4379|Televisão|5|Thiago|Veiga|3/7/2018|Rio de Janeiro|2500|NaN|12500|
|234|1522|HL7348|SmartWatch|3|Raphael|Kurtz|3/3/2018|Rio de Janeiro|1400|NaN|4200|
|235|1523|HL1918|iPhone|3|Célio|Xavier|5/25/2018|Rio de Janeiro|5300|NaN|15900|
|236|1524|HL1918|iPhone|3|Júlio|Fraga|7/18/2018|Rio de Janeiro|5300|NaN|15900|
|237|1532|HL1918|iPhone|4|João|Menezes|2/26/2018|Rio de Janeiro|5300|NaN|21200|
|238|1548|HL8851|Notebook|3|Stela|Mendonça|3/12/2018|Rio de Janeiro|3500|NaN|10500|
|239|1550|HL9962|Android|5|Lara|Moreira|1/8/2018|Rio de Janeiro|3400|NaN|17000|
|240|1558|HL1918|iPhone|1|Stephanie|Oliveira|5/10/2018|Rio de Janeiro|5300|NaN|5300|
|241|1567|HL7348|SmartWatch|1|Rodrigo|Alves|5/30/2018|Rio de Janeiro|1400|NaN|1400|
|242|1599|HL1918|iPhone|4|Camila|Sobral|1/14/2018|Rio de Janeiro|5300|NaN|21200|
|243|1606|HL1148|Câmera|3|Sthefeson|Barroso|6/12/2018|Rio de Janeiro|2100|NaN|6300|
|244|1615|HL7348|SmartWatch|3|Amanda|Procaci|9/29/2018|Rio de Janeiro|1400|NaN|4200|
|245|1619|HL4379|Televisão|1|Milena|Pereira|10/4/2018|Rio de Janeiro|2500|NaN|2500|
|246|1623|HL4379|Televisão|5|Carlos|Portela|3/11/2018|Rio de Janeiro|2500|NaN|12500|
|247|1626|HL4379|Televisão|2|Caio|Vianna|9/5/2018|Rio de Janeiro|2500|NaN|5000|
|248|1640|HL1918|iPhone|4|Marcos|Nucci|1/16/2018|Rio de Janeiro|5300|NaN|21200|
|249|1641|HL9962|Android|3|Luis|Villanova|10/24/2018|Rio de Janeiro|3400|NaN|10200|
|250|1651|HL9962|Android|5|Rilson|Guedes|12/28/2018|Rio de Janeiro|3400|NaN|17000|
|251|1665|HL1918|iPhone|1|Gabriel|Ribeiro|11/8/2018|Rio de Janeiro|5300|NaN|5300|
|252|1671|HL4379|Televisão|4|Daniel|Monteiro|12/5/2018|Rio de Janeiro|2500|NaN|10000|
|253|1675|HL1148|Câmera|2|Luíza|Melo|11/21/2018|Rio de Janeiro|2100|NaN|4200|
|254|1677|HL9962|Android|1|Fernanda|Coutinho|10/22/2018|Rio de Janeiro|3400|NaN|3400|
|255|1692|HL7348|SmartWatch|4|Mariana|Freire|7/5/2018|Rio de Janeiro|1400|NaN|5600|
|256|1693|HL1918|iPhone|5|Gabrielle|Wanderley|12/23/2018|Rio de Janeiro|5300|NaN|26500|
|257|1696|HL1918|iPhone|2|David|Campelo|11/21/2018|Rio de Janeiro|5300|NaN|10600|
|258|1707|HL9962|Android|5|Thales|Portillo|2/9/2018|Rio de Janeiro|3400|NaN|17000|
|259|1715|HL1918|iPhone|5|Gabriel|Azevedo|1/15/2018|Rio de Janeiro|5300|NaN|26500|
|260|1724|HL4379|Televisão|3|Adrielle|Forte|9/22/2018|Rio de Janeiro|2500|NaN|7500|
|261|1727|HL7348|SmartWatch|3|Paulo|Campos|1/30/2018|Rio de Janeiro|1400|NaN|4200|
|262|1739|HL1918|iPhone|3|Deysiane|Medronho|5/31/2018|Rio de Janeiro|5300|NaN|15900|
|263|1741|HL1918|iPhone|2|Rafaela|Ferreira|7/3/2018|Rio de Janeiro|5300|NaN|10600|
|264|1744|HL8851|Notebook|2|Pedro|Sena|2/15/2018|Rio de Janeiro|3500|NaN|7000|
|265|1753|HL8851|Notebook|3|Raul|Junqueira|2/23/2018|Rio de Janeiro|3500|NaN|10500|
|266|1758|HL1918|iPhone|1|Vitor|Boccaletti|11/21/2018|Rio de Janeiro|5300|NaN|5300|
|267|1766|HL1918|iPhone|1|Leandro|Ferreira|1/16/2018|Rio de Janeiro|5300|NaN|5300|
|268|1769|HL2714|Tablet|4|Caio|Ferreira|12/30/2018|Rio de Janeiro|1600|NaN|6400|
|269|1773|HL1918|iPhone|2|Thomáz|Vannier|11/3/2018|Rio de Janeiro|5300|NaN|10600|
|270|1778|HL1148|Câmera|3|Eduardo|Peluzo|7/2/2018|Rio de Janeiro|2100|NaN|6300|
|271|1781|HL8851|Notebook|5|André|Alves|12/31/2018|Rio de Janeiro|3500|NaN|17500|
|272|1787|HL1918|iPhone|4|Carolina|Carneiro|6/10/2018|Rio de Janeiro|5300|NaN|21200|
|273|1790|HL8851|Notebook|2|Luiz|Campista|10/26/2018|Rio de Janeiro|3500|NaN|7000|
|274|1791|HL9962|Android|4|Mônica|Rotolo|7/4/2018|Rio de Janeiro|3400|NaN|13600|
|275|1803|HL1918|iPhone|5|Isabella|Scalabrin|8/12/2018|Rio de Janeiro|5300|NaN|26500|
|276|1811|HL8851|Notebook|2|Marina|Correa|1/11/2018|Rio de Janeiro|3500|NaN|7000|
|277|1824|HL1918|iPhone|2|Ana|Campos|2/28/2018|Rio de Janeiro|5300|NaN|10600|
|278|1826|HL1918|iPhone|3|Sarah|Souza|9/8/2018|Rio de Janeiro|5300|NaN|15900|
|279|1828|HL1148|Câmera|2|Matheus|Moraes|8/10/2018|Rio de Janeiro|2100|NaN|4200|
|280|1832|HL4379|Televisão|3|Izabel|Miura|2/2/2018|Rio de Janeiro|2500|NaN|7500|
|281|1833|HL1918|iPhone|1|Maria|Mello|4/25/2018|Rio de Janeiro|5300|NaN|5300|
|282|1846|HL1148|Câmera|3|Vitor|Arruda|4/21/2018|Rio de Janeiro|2100|NaN|6300|
|283|1847|HL8851|Notebook|3|Raphael|Ferman|2/12/2018|Rio de Janeiro|3500|NaN|10500|
|284|1848|HL2714|Tablet|1|Matheus|Ramos|1/13/2018|Rio de Janeiro|1600|NaN|1600|
|285|1856|HL4379|Televisão|3|Camilla|Cardeman|4/16/2018|Rio de Janeiro|2500|NaN|7500|
|286|1878|HL7348|SmartWatch|3|João|Peçanha|7/7/2018|Rio de Janeiro|1400|NaN|4200|
|287|1887|HL1918|iPhone|1|Wellington|Duarte|1/21/2018|Rio de Janeiro|5300|NaN|5300|
|288|1894|HL1148|Câmera|1|Luíza|Garcia|8/30/2018|Rio de Janeiro|2100|NaN|2100|
|289|1909|HL1918|iPhone|5|Thiago|Veiga|2/18/2018|Rio de Janeiro|5300|NaN|26500|
|290|1915|HL1148|Câmera|4|Raphael|Rezende|5/16/2018|Rio de Janeiro|2100|NaN|8400|
|291|1917|HL7348|SmartWatch|2|Juliana|Goes|9/18/2018|Rio de Janeiro|1400|NaN|2800|
|292|1925|HL2714|Tablet|2|Sthefeson|Pereira|7/25/2018|Rio de Janeiro|1600|NaN|3200|
|293|1930|HL4379|Televisão|5|Isabella|Santos|9/26/2018|Rio de Janeiro|2500|NaN|12500|
|294|1939|HL8851|Notebook|4|Juan|Barbosa|3/15/2018|Rio de Janeiro|3500|NaN|14000|
|295|1940|HL4379|Televisão|2|Patrick|Silva|4/28/2018|Rio de Janeiro|2500|NaN|5000|
|296|1941|HL4379|Televisão|4|Antônio|Oliveira|1/10/2018|Rio de Janeiro|2500|NaN|10000|
|297|1942|HL2714|Tablet|4|Brenno|Santos|6/20/2018|Rio de Janeiro|1600|NaN|6400|
|298|1944|HL4379|Televisão|3|Rachel|Restum|12/24/2018|Rio de Janeiro|2500|NaN|7500|
|299|1949|HL7348|SmartWatch|1|Rafael|Guimarães|12/30/2018|Rio de Janeiro|1400|NaN|1400|
|300|1969|HL1918|iPhone|1|Guilherme|Jordao|2/4/2018|Rio de Janeiro|5300|NaN|5300|
|301|1973|HL9962|Android|3|Ives|Teixeira|11/14/2018|Rio de Janeiro|3400|NaN|10200|
|302|1977|HL4379|Televisão|3|Daniel|Araujo|1/21/2018|Rio de Janeiro|2500|NaN|7500|
|303|1988|HL8851|Notebook|4|Eduardo|Vargas|6/13/2018|Rio de Janeiro|3500|NaN|14000|
|304|1992|HL9962|Android|1|Thays|Castro|11/9/2018|Rio de Janeiro|3400|NaN|3400|
|305|1998|HL1918|iPhone|1|Michelle|Figueiredo|10/15/2018|Rio de Janeiro|5300|NaN|5300|
|306|2003|HL4379|Televisão|4|Luiza|Cabral|10/16/2018|Rio de Janeiro|2500|NaN|10000|
|307|2007|HL8851|Notebook|4|Anderson|Barreto|4/2/2018|Rio de Janeiro|3500|NaN|14000|
|308|2009|HL7348|SmartWatch|4|Wellington|Duarte|7/12/2018|Rio de Janeiro|1400|NaN|5600|
|309|2025|HL7348|SmartWatch|4|Hanna|Fonseca|7/2/2018|Rio de Janeiro|1400|NaN|5600|
|310|2031|HL1918|iPhone|5|Gabriel|Pereira|7/29/2018|Rio de Janeiro|5300|NaN|26500|
|311|2038|HL4379|Televisão|3|Bruno|Souza|12/17/2018|Rio de Janeiro|2500|NaN|7500|
|312|2049|HL1918|iPhone|4|Lívia|Marques|10/2/2018|Rio de Janeiro|5300|NaN|21200|
|313|2054|HL1918|iPhone|2|Julia|Teixeira|6/16/2018|Rio de Janeiro|5300|NaN|10600|
|314|2061|HL1148|Câmera|3|Bruno|Silva|3/17/2018|Rio de Janeiro|2100|NaN|6300|
|315|2066|HL2714|Tablet|5|Elaine|Santos|2/27/2018|Rio de Janeiro|1600|NaN|8000|
|316|2067|HL4379|Televisão|2|Lucas|Freitas|9/12/2018|Rio de Janeiro|2500|NaN|5000|
|317|2070|HL8851|Notebook|3|Stephanie|Novak|5/1/2018|Rio de Janeiro|3500|NaN|10500|
|318|2071|HL4379|Televisão|1|Lorena|Carvalho|9/10/2018|Rio de Janeiro|2500|NaN|2500|
|319|2104|HL1918|iPhone|1|Breno|Quinto|6/19/2018|Rio de Janeiro|5300|NaN|5300|
|320|2107|HL2714|Tablet|3|Ruan|Gonçalves|1/13/2018|Rio de Janeiro|1600|NaN|4800|
|321|2111|HL9962|Android|1|Wendela|Veloso|12/31/2018|Rio de Janeiro|3400|NaN|3400|
|322|2116|HL4379|Televisão|2|Vivianne|Rodrigues|12/16/2018|Rio de Janeiro|2500|NaN|5000|
|323|2124|HL7348|SmartWatch|3|Michelle|Miura|12/13/2018|Rio de Janeiro|1400|NaN|4200|
|324|2129|HL1918|iPhone|1|Felipe|Jorge|1/4/2018|Rio de Janeiro|5300|NaN|5300|
|325|2144|HL4379|Televisão|4|Lucas|Valim|3/2/2018|Rio de Janeiro|2500|NaN|10000|
|326|2161|HL7348|SmartWatch|1|Joao|Pereira|8/5/2018|Rio de Janeiro|1400|NaN|1400|
|327|2164|HL4379|Televisão|3|Allan|Guedes|5/13/2018|Rio de Janeiro|2500|NaN|7500|
|328|2167|HL2714|Tablet|5|Jéssica|Resinente|1/13/2018|Rio de Janeiro|1600|NaN|8000|
|329|2174|HL7348|SmartWatch|3|Letícia|Rodrigues|10/20/2018|Rio de Janeiro|1400|NaN|4200|
|330|2178|HL4379|Televisão|2|Lucas|Rocha|3/20/2018|Rio de Janeiro|2500|NaN|5000|
|331|2180|HL4379|Televisão|1|Guilherme|Merotto|7/30/2018|Rio de Janeiro|2500|NaN|2500|
|332|2181|HL4379|Televisão|4|Rebeca|Taylor|1/14/2018|Rio de Janeiro|2500|NaN|10000|
|333|2184|HL1918|iPhone|1|Camille|Silva|2/15/2018|Rio de Janeiro|5300|NaN|5300|
|334|2204|HL9962|Android|1|Lucas|Chagas|11/11/2018|Rio de Janeiro|3400|NaN|3400|
|335|2206|HL1918|iPhone|2|Eduardo|Quindeler|9/27/2018|Rio de Janeiro|5300|NaN|10600|
|336|2209|HL1148|Câmera|4|Elaine|Santos|11/9/2018|Rio de Janeiro|2100|NaN|8400|
|337|2219|HL8851|Notebook|3|Carolina|Bernardes|5/18/2018|Rio de Janeiro|3500|NaN|10500|
|338|2221|HL4379|Televisão|4|Thaís|Pereira|2/21/2018|Rio de Janeiro|2500|NaN|10000|
|339|2230|HL4379|Televisão|3|Gustavo|Erthal|4/5/2018|Rio de Janeiro|2500|NaN|7500|
|340|2234|HL1918|iPhone|2|Marcelo|Magalhães|12/14/2018|Rio de Janeiro|5300|NaN|10600|
|341|2254|HL1918|iPhone|1|Isabela|Rodrigues|11/4/2018|Rio de Janeiro|5300|NaN|5300|
|342|2263|HL9962|Android|3|Clarissa|Santos|8/2/2018|Rio de Janeiro|3400|NaN|10200|
|343|2266|HL1918|iPhone|5|José|Vieira|4/3/2018|Rio de Janeiro|5300|NaN|26500|
|344|2269|HL8851|Notebook|1|Bruna|Gomes|3/16/2018|Rio de Janeiro|3500|NaN|3500|
|345|2272|HL2714|Tablet|1|Lorena|Carvalho|9/6/2018|Rio de Janeiro|1600|NaN|1600|
|346|2275|HL1918|iPhone|1|Mariana|Miranda|8/4/2018|Rio de Janeiro|5300|NaN|5300|
|347|2278|HL9962|Android|4|João|Bach|8/18/2018|Rio de Janeiro|3400|NaN|13600|
|348|2279|HL4379|Televisão|5|Rogério|Gentile|7/5/2018|Rio de Janeiro|2500|NaN|12500|
|349|2288|HL7348|SmartWatch|5|Vitor|Campos|1/20/2018|Rio de Janeiro|1400|NaN|7000|
|350|2295|HL1148|Câmera|3|Rafael|Rocha|3/2/2018|Rio de Janeiro|2100|NaN|6300|
|351|2299|HL1918|iPhone|5|Marina|Mesquita|4/6/2018|Rio de Janeiro|5300|NaN|26500|
|352|2302|HL9962|Android|2|Breno|Quinto|5/22/2018|Rio de Janeiro|3400|NaN|6800|
|353|2315|HL8851|Notebook|5|Luis|Oliveira|5/14/2018|Rio de Janeiro|3500|NaN|17500|
|354|2318|HL8851|Notebook|5|Julia|Figueiredo|8/17/2018|Rio de Janeiro|3500|NaN|17500|
|355|2323|HL2714|Tablet|4|Victor|Franco|11/4/2018|Rio de Janeiro|1600|NaN|6400|
|356|2337|HL1918|iPhone|2|Hércules|Júnior|1/20/2018|Rio de Janeiro|5300|NaN|10600|
|357|2346|HL8851|Notebook|1|Yasser|Calbucci|7/4/2018|Rio de Janeiro|3500|NaN|3500|
|358|2357|HL2714|Tablet|3|Luiz|Xavier|11/18/2018|Rio de Janeiro|1600|NaN|4800|
|359|2375|HL2714|Tablet|1|Camille|Silva|2/19/2018|Rio de Janeiro|1600|NaN|1600|
|360|2377|HL1918|iPhone|1|Cassio|Faria|1/22/2018|Rio de Janeiro|5300|NaN|5300|
|361|2378|HL1918|iPhone|3|Wendela|Mariz|8/8/2018|Rio de Janeiro|5300|NaN|15900|
|362|2383|HL7348|SmartWatch|2|Roberto|Nogueira|10/24/2018|Rio de Janeiro|1400|NaN|2800|
|363|2389|HL2714|Tablet|1|Fabio|Ramos|8/14/2018|Rio de Janeiro|1600|NaN|1600|
|364|2390|HL4379|Televisão|3|Jorge|Carvalho|4/11/2018|Rio de Janeiro|2500|NaN|7500|
|365|2397|HL7348|SmartWatch|5|Stephanie|Oliveira|9/6/2018|Rio de Janeiro|1400|NaN|7000|
|366|2423|HL9962|Android|5|Fernanda|Ferreira|9/9/2018|Rio de Janeiro|3400|NaN|17000|
|367|2442|HL1918|iPhone|4|Marcela|Gasperi|12/8/2018|Rio de Janeiro|5300|NaN|21200|
|368|2444|HL1918|iPhone|2|Clarissa|Santos|6/1/2018|Rio de Janeiro|5300|NaN|10600|
|369|2445|HL8851|Notebook|4|Carlos|Assis|10/20/2018|Rio de Janeiro|3500|NaN|14000|
|370|2457|HL1918|iPhone|1|Guido|Monteiro|2/24/2018|Rio de Janeiro|5300|NaN|5300|
|371|2459|HL1918|iPhone|5|Marina|Aragão|1/1/2018|Rio de Janeiro|5300|NaN|26500|
|372|2460|HL1918|iPhone|2|Felipe|Mendonça|8/30/2018|Rio de Janeiro|5300|NaN|10600|
|373|2461|HL1918|iPhone|3|Maria|Cardoso|7/22/2018|Rio de Janeiro|5300|NaN|15900|
|374|2466|HL1918|iPhone|2|Mariana|Sousa|11/16/2018|Rio de Janeiro|5300|NaN|10600|
|375|2485|HL8851|Notebook|3|Matheus|Santos|7/17/2018|Rio de Janeiro|3500|NaN|10500|
|376|2495|HL4379|Televisão|4|Arthur|Pereira|10/30/2018|Rio de Janeiro|2500|NaN|10000|
|377|2498|HL2714|Tablet|5|Karina|Camara|10/19/2018|Rio de Janeiro|1600|NaN|8000|
|378|2500|HL1918|iPhone|2|Rodrigo|Silva|11/28/2018|Rio de Janeiro|5300|NaN|10600|
|379|2506|HL9962|Android|2|Jorge|Fonseca|10/17/2018|Rio de Janeiro|3400|NaN|6800|
|380|2508|HL1918|iPhone|1|Bruno|Ferreira|1/20/2018|Rio de Janeiro|5300|NaN|5300|
|381|2509|HL2714|Tablet|3|Luiz|Conceição|4/20/2018|Rio de Janeiro|1600|NaN|4800|
|382|2513|HL1918|iPhone|1|Bernardo|Souza|11/19/2018|Rio de Janeiro|5300|NaN|5300|
|383|2520|HL8851|Notebook|4|Gabriel|Assis|5/8/2018|Rio de Janeiro|3500|NaN|14000|
|384|2521|HL1918|iPhone|1|Matheus|Delgado|11/12/2018|Rio de Janeiro|5300|NaN|5300|
|385|2522|HL4379|Televisão|3|Carolina|Bernardes|4/12/2018|Rio de Janeiro|2500|NaN|7500|
|386|2529|HL9962|Android|5|Bruna|Ramos|1/24/2018|Rio de Janeiro|3400|NaN|17000|
|387|2531|HL7348|SmartWatch|1|João|Matheus|7/21/2018|Rio de Janeiro|1400|NaN|1400|
|388|2532|HL1918|iPhone|4|Guilherme|Seixas|6/20/2018|Rio de Janeiro|5300|NaN|21200|
|389|2534|HL1918|iPhone|4|Ramon|Araujo|7/15/2018|Rio de Janeiro|5300|NaN|21200|
|390|2538|HL9962|Android|3|Raissa|Pinheiro|8/8/2018|Rio de Janeiro|3400|NaN|10200|
|391|2553|HL1918|iPhone|4|Rafaela|Gonçalves|10/17/2018|Rio de Janeiro|5300|NaN|21200|
|392|2558|HL1918|iPhone|1|Giulia|Pessanha|8/2/2018|Rio de Janeiro|5300|NaN|5300|
|393|2559|HL1918|iPhone|5|Daniela|Pereira|9/6/2018|Rio de Janeiro|5300|NaN|26500|
|394|2562|HL9962|Android|3|Eric|Carvalho|5/12/2018|Rio de Janeiro|3400|NaN|10200|
|395|2572|HL1918|iPhone|3|João|Castilho|3/12/2018|Rio de Janeiro|5300|NaN|15900|
|396|2577|HL1918|iPhone|3|Joyce|Medina|4/15/2018|Rio de Janeiro|5300|NaN|15900|
|397|2583|HL1918|iPhone|1|Bruno|Salomão|1/2/2018|Rio de Janeiro|5300|NaN|5300|
|398|2588|HL9962|Android|2|Larissa|Jesus|9/14/2018|Rio de Janeiro|3400|NaN|6800|
|399|2598|HL1918|iPhone|5|Carolina|Siqueira|6/1/2018|Rio de Janeiro|5300|NaN|26500|
|400|2613|HL7348|SmartWatch|1|Vitor|Boccaletti|3/1/2018|Rio de Janeiro|1400|NaN|1400|
|401|2617|HL4379|Televisão|3|Laura|Araujo|8/24/2018|Rio de Janeiro|2500|NaN|7500|
|402|2621|HL8851|Notebook|1|Breno|Caputo|2/2/2018|Rio de Janeiro|3500|NaN|3500|
|403|2623|HL1918|iPhone|3|Fernanda|Coutinho|7/13/2018|Rio de Janeiro|5300|NaN|15900|
|404|2629|HL9962|Android|4|Gustavo|Gomes|11/13/2018|Rio de Janeiro|3400|NaN|13600|
|405|2636|HL1148|Câmera|3|Tainah|Nogueira|11/19/2018|Rio de Janeiro|2100|NaN|6300|
|406|2650|HL1918|iPhone|3|Laís|Oliveira|7/2/2018|Rio de Janeiro|5300|NaN|15900|
|407|2660|HL4379|Televisão|1|Isabelle|Firmino|7/8/2018|Rio de Janeiro|2500|NaN|2500|
|408|2667|HL7348|SmartWatch|5|Daniel|Araujo|1/18/2018|Rio de Janeiro|1400|NaN|7000|
|409|2668|HL7348|SmartWatch|3|Carlos|Assis|8/30/2018|Rio de Janeiro|1400|NaN|4200|
|410|2680|HL1918|iPhone|4|Wilson|Miranda|7/11/2018|Rio de Janeiro|5300|NaN|21200|
|411|2689|HL7348|SmartWatch|5|João|Costa|6/9/2018|Rio de Janeiro|1400|NaN|7000|
|412|2703|HL8851|Notebook|2|Carolina|Abrahão|5/7/2018|Rio de Janeiro|3500|NaN|7000|
|413|2704|HL4379|Televisão|3|Débora|Lopes|6/9/2018|Rio de Janeiro|2500|NaN|7500|
|414|2714|HL9962|Android|2|Tayla|Lima|5/7/2018|Rio de Janeiro|3400|NaN|6800|
|415|2715|HL1918|iPhone|5|Gabriel|Puntel|12/28/2018|Rio de Janeiro|5300|NaN|26500|
|416|2718|HL1148|Câmera|3|Danilo|Alves|12/14/2018|Rio de Janeiro|2100|NaN|6300|
|417|2724|HL4379|Televisão|5|Carolina|Rocha|11/30/2018|Rio de Janeiro|2500|NaN|12500|
|418|2726|HL4379|Televisão|4|Camila|Sobral|10/31/2018|Rio de Janeiro|2500|NaN|10000|
|419|2734|HL1918|iPhone|2|Beatriz|Rodrigues|7/7/2018|Rio de Janeiro|5300|NaN|10600|
|420|2748|HL1148|Câmera|1|Marcos|Nucci|6/28/2018|Rio de Janeiro|2100|NaN|2100|
|421|2751|HL1918|iPhone|5|Maria|Gasperi|4/6/2018|Rio de Janeiro|5300|NaN|26500|
|422|2765|HL7348|SmartWatch|5|Gabrielle|Costa|3/30/2018|Rio de Janeiro|1400|NaN|7000|
|423|2766|HL8851|Notebook|4|Dandara|Reis|4/29/2018|Rio de Janeiro|3500|NaN|14000|
|424|2767|HL1918|iPhone|3|Rubens|Netto|6/29/2018|Rio de Janeiro|5300|NaN|15900|
|425|2773|HL1918|iPhone|3|Caio|Cardoso|8/17/2018|Rio de Janeiro|5300|NaN|15900|
|426|2794|HL1148|Câmera|2|Milena|Pereira|4/20/2018|Rio de Janeiro|2100|NaN|4200|
|427|2797|HL1918|iPhone|2|Julia|Leig|3/13/2018|Rio de Janeiro|5300|NaN|10600|
|428|2801|HL4379|Televisão|2|Pedro|Dalforne|11/4/2018|Rio de Janeiro|2500|NaN|5000|
|429|2811|HL2714|Tablet|2|Carolina|Silva|5/25/2018|Rio de Janeiro|1600|NaN|3200|
|430|2812|HL4379|Televisão|2|Ives|Teixeira|8/7/2018|Rio de Janeiro|2500|NaN|5000|
|431|2818|HL1918|iPhone|4|Eduardo|Ferreira|8/3/2018|Rio de Janeiro|5300|NaN|21200|
|432|2822|HL4379|Televisão|3|Lucas|Rodrigues|3/6/2018|Rio de Janeiro|2500|NaN|7500|
|433|2830|HL8851|Notebook|2|Breno|Caputo|5/5/2018|Rio de Janeiro|3500|NaN|7000|
|434|2836|HL1918|iPhone|3|Carlos|Cardoso|8/14/2018|Rio de Janeiro|5300|NaN|15900|
|435|2846|HL9962|Android|5|Dandara|Reis|3/19/2018|Rio de Janeiro|3400|NaN|17000|
|436|2861|HL1918|iPhone|3|Caroline|Pinto|1/13/2018|Rio de Janeiro|5300|NaN|15900|
|437|2863|HL9962|Android|3|Marina|Marins|6/10/2018|Rio de Janeiro|3400|NaN|10200|
|438|2864|HL1918|iPhone|1|Juliana|Barreira|5/7/2018|Rio de Janeiro|5300|NaN|5300|
|439|2865|HL4379|Televisão|3|Pedro|Lyra|9/22/2018|Rio de Janeiro|2500|NaN|7500|
|440|2871|HL1918|iPhone|3|Beatriz|Biase|1/20/2018|Rio de Janeiro|5300|NaN|15900|
|441|2877|HL1918|iPhone|4|Luiz|Conceição|12/12/2018|Rio de Janeiro|5300|NaN|21200|
|442|2889|HL1918|iPhone|1|Raissa|Sales|4/11/2018|Rio de Janeiro|5300|NaN|5300|
|443|2909|HL2714|Tablet|3|Alexandre|Rodriguez|10/8/2018|Rio de Janeiro|1600|NaN|4800|
|444|2913|HL1918|iPhone|5|Breno|Quinto|6/9/2018|Rio de Janeiro|5300|NaN|26500|
|445|2915|HL8851|Notebook|4|Carolina|Abrahão|1/16/2018|Rio de Janeiro|3500|NaN|14000|
|446|2940|HL4379|Televisão|4|Breno|Farias|10/5/2018|Rio de Janeiro|2500|NaN|10000|
|447|2948|HL9962|Android|5|Pedro|Oliveira|2/1/2018|Rio de Janeiro|3400|NaN|17000|
|448|2955|HL7348|SmartWatch|5|Rafaela|Gonçalves|2/8/2018|Rio de Janeiro|1400|NaN|7000|
|449|2966|HL4379|Televisão|4|Thales|Gouvêa|10/24/2018|Rio de Janeiro|2500|NaN|10000|
|450|2969|HL2714|Tablet|3|Izabel|Lopes|5/10/2018|Rio de Janeiro|1600|NaN|4800|
|451|2980|HL7348|SmartWatch|1|Isabela|Resende|10/1/2018|Rio de Janeiro|1400|NaN|1400|
|452|2981|HL1918|iPhone|2|Nathan|Cunha|9/27/2018|Rio de Janeiro|5300|NaN|10600|
|453|2994|HL7348|SmartWatch|3|Fernanda|Bhering|3/31/2018|Rio de Janeiro|1400|NaN|4200|
|454|3002|HL1918|iPhone|1|Mariana|Sousa|2/8/2018|Rio de Janeiro|5300|NaN|5300|
|455|3010|HL4379|Televisão|5|Livia|Cozendey|8/16/2018|Rio de Janeiro|2500|NaN|12500|
|456|3013|HL1148|Câmera|1|Ives|Pinheiro|2/11/2018|Rio de Janeiro|2100|NaN|2100|
|457|3014|HL1918|iPhone|3|Rubens|Netto|1/31/2018|Rio de Janeiro|5300|NaN|15900|
|458|3019|HL1918|iPhone|3|Carolina|Carneiro|11/8/2018|Rio de Janeiro|5300|NaN|15900|
|459|3027|HL2714|Tablet|5|Eduardo|Soares|3/25/2018|Rio de Janeiro|1600|NaN|8000|
|460|3030|HL4379|Televisão|3|Lais|Candido|4/15/2018|Rio de Janeiro|2500|NaN|7500|
|461|3042|HL7348|SmartWatch|4|Priscila|Garcia|12/7/2018|Rio de Janeiro|1400|NaN|5600|
|462|3044|HL8851|Notebook|3|Mariana|Miranda|5/4/2018|Rio de Janeiro|3500|NaN|10500|
|463|3045|HL8851|Notebook|1|Wilson|Miranda|6/27/2018|Rio de Janeiro|3500|NaN|3500|
|464|3050|HL1918|iPhone|4|Gustavo|Aragão|11/7/2018|Rio de Janeiro|5300|NaN|21200|
|465|3054|HL7348|SmartWatch|2|Guilherme|Lima|10/13/2018|Rio de Janeiro|1400|NaN|2800|
|466|3057|HL4379|Televisão|3|Gabrielle|Porto|6/5/2018|Rio de Janeiro|2500|NaN|7500|
|467|3067|HL2714|Tablet|4|Carlos|Melo|11/5/2018|Rio de Janeiro|1600|NaN|6400|
|468|3068|HL2714|Tablet|3|Leonardo|Ferreira|4/11/2018|Rio de Janeiro|1600|NaN|4800|
|469|3080|HL4379|Televisão|4|Tadeu|Sousa|4/23/2018|Rio de Janeiro|2500|NaN|10000|
|470|3082|HL1148|Câmera|2|Andre|Sampaio|6/29/2018|Rio de Janeiro|2100|NaN|4200|
|471|3084|HL1918|iPhone|5|Anna|Silva|9/7/2018|Rio de Janeiro|5300|NaN|26500|
|472|3085|HL1148|Câmera|2|Bruno|Silva|10/2/2018|Rio de Janeiro|2100|NaN|4200|
|473|3092|HL1918|iPhone|4|Gustavo|Guimarães|10/28/2018|Rio de Janeiro|5300|NaN|21200|
|474|3093|HL2714|Tablet|3|Maria|Mello|2/6/2018|Rio de Janeiro|1600|NaN|4800|
|475|3099|HL9962|Android|5|Marcelo|Pereira|2/3/2018|Rio de Janeiro|3400|NaN|17000|
|476|3113|HL9962|Android|2|Daniel|Nauenberg|1/3/2018|Rio de Janeiro|3400|NaN|6800|
|477|3118|HL9962|Android|5|Daniel|Felippe|7/7/2018|Rio de Janeiro|3400|NaN|17000|
|478|3119|HL1918|iPhone|3|Danilo|Alves|6/19/2018|Rio de Janeiro|5300|NaN|15900|
|479|3124|HL1148|Câmera|1|Lucas|Junior|4/24/2018|Rio de Janeiro|2100|NaN|2100|
|480|3127|HL2714|Tablet|5|Natali|Rangel|6/12/2018|Rio de Janeiro|1600|NaN|8000|
|481|3144|HL1918|iPhone|5|Amanda|Amaral|10/29/2018|Rio de Janeiro|5300|NaN|26500|
|482|3151|HL1148|Câmera|5|Norman|Jimbo|5/10/2018|Rio de Janeiro|2100|NaN|10500|
|483|3156|HL1918|iPhone|1|Caroline|Cavalcanti|9/25/2018|Rio de Janeiro|5300|NaN|5300|
|484|3158|HL7348|SmartWatch|2|Rodrigo|Alves|3/13/2018|Rio de Janeiro|1400|NaN|2800|
|485|3159|HL1918|iPhone|5|Lucas|Valim|6/9/2018|Rio de Janeiro|5300|NaN|26500|
|486|3162|HL4379|Televisão|1|Adriane|Gomes|3/28/2018|Rio de Janeiro|2500|NaN|2500|
|487|3167|HL8851|Notebook|4|Letícia|Rodrigues|8/17/2018|Rio de Janeiro|3500|NaN|14000|
|488|3168|HL1918|iPhone|4|Raissa|Sales|11/29/2018|Rio de Janeiro|5300|NaN|21200|
|489|3175|HL2714|Tablet|2|Guilherme|Assis|11/12/2018|Rio de Janeiro|1600|NaN|3200|
|490|3183|HL1918|iPhone|5|Caio|Moraes|2/24/2018|Rio de Janeiro|5300|NaN|26500|
|491|3185|HL8851|Notebook|2|Adriana|Carneiro|4/4/2018|Rio de Janeiro|3500|NaN|7000|
|492|3190|HL1148|Câmera|4|Natalia|Marinho|10/9/2018|Rio de Janeiro|2100|NaN|8400|
|493|3191|HL4379|Televisão|4|Mariana|Barrozo|7/25/2018|Rio de Janeiro|2500|NaN|10000|
|494|3193|HL9962|Android|3|Giovanna|Santos|1/8/2018|Rio de Janeiro|3400|NaN|10200|
|495|3195|HL1918|iPhone|3|Rogério|Pereira|7/31/2018|Rio de Janeiro|5300|NaN|15900|
|496|3203|HL1148|Câmera|3|Thaís|Ribeiro|8/26/2018|Rio de Janeiro|2100|NaN|6300|
|497|3209|HL1918|iPhone|4|Lucas|Junior|8/21/2018|Rio de Janeiro|5300|NaN|21200|
|498|3223|HL2714|Tablet|4|Marcela|Johnson|12/22/2018|Rio de Janeiro|1600|NaN|6400|
|499|3228|HL1918|iPhone|2|Priscila|Garcia|6/24/2018|Rio de Janeiro|5300|NaN|10600|
|500|3231|HL1918|iPhone|4|Débora|Lopes|9/25/2018|Rio de Janeiro|5300|NaN|21200|
|501|3239|HL4379|Televisão|2|Julia|Aliani|11/25/2018|Rio de Janeiro|2500|NaN|5000|
|502|3241|HL9962|Android|4|Gabriel|Rocha|1/22/2018|Rio de Janeiro|3400|NaN|13600|
|503|3245|HL1918|iPhone|1|Roberta|Pimenta|9/15/2018|Rio de Janeiro|5300|NaN|5300|
|504|3254|HL1918|iPhone|5|Andressa|Rotsztejn|2/14/2018|Rio de Janeiro|5300|NaN|26500|
|505|3256|HL8851|Notebook|3|Victor|Zakhm|8/12/2018|Rio de Janeiro|3500|NaN|10500|
|506|3267|HL4379|Televisão|4|Gustavo|Accardo|4/14/2018|Rio de Janeiro|2500|NaN|10000|
|507|3270|HL1148|Câmera|3|Joyce|Souza|8/26/2018|Rio de Janeiro|2100|NaN|6300|
|508|3273|HL4379|Televisão|2|Bernard|Pedrosa|1/16/2018|Rio de Janeiro|2500|NaN|5000|
|509|3276|HL1918|iPhone|4|Raísa|Berto|2/4/2018|Rio de Janeiro|5300|NaN|21200|
|510|3280|HL4379|Televisão|1|Isabel|Leite|9/8/2018|Rio de Janeiro|2500|NaN|2500|
|511|3287|HL1918|iPhone|1|Karina|Camara|7/19/2018|Rio de Janeiro|5300|NaN|5300|
|512|3293|HL1148|Câmera|2|Ian|Almeida|8/26/2018|Rio de Janeiro|2100|NaN|4200|
|513|3301|HL4379|Televisão|3|Arthur|Pereira|8/7/2018|Rio de Janeiro|2500|NaN|7500|
|514|3302|HL7348|SmartWatch|3|Izabel|Miura|3/21/2018|Rio de Janeiro|1400|NaN|4200|
|515|3305|HL1918|iPhone|4|Guilherme|Merotto|7/19/2018|Rio de Janeiro|5300|NaN|21200|
|516|3307|HL1148|Câmera|2|Marina|Gama|6/29/2018|Rio de Janeiro|2100|NaN|4200|
|517|3311|HL2714|Tablet|4|Isabella|Santos|6/16/2018|Rio de Janeiro|1600|NaN|6400|
|518|3313|HL7348|SmartWatch|4|Giulia|Lopes|8/11/2018|Rio de Janeiro|1400|NaN|5600|
|519|3318|HL8851|Notebook|5|Amanda|Delgado|3/20/2018|Rio de Janeiro|3500|NaN|17500|
|520|3319|HL8851|Notebook|2|Gabrielle|Viríssimo|8/15/2018|Rio de Janeiro|3500|NaN|7000|
|521|3320|HL9962|Android|5|Wilson|Miranda|11/26/2018|Rio de Janeiro|3400|NaN|17000|
|522|3322|HL9962|Android|4|Priscila|Suzano|11/4/2018|Rio de Janeiro|3400|NaN|13600|
|523|3340|HL1918|iPhone|4|Rodrigo|Mendes|9/6/2018|Rio de Janeiro|5300|NaN|21200|
|524|3342|HL7348|SmartWatch|1|Karina|Camara|1/23/2018|Rio de Janeiro|1400|NaN|1400|
|525|3346|HL1918|iPhone|3|Marcela|Gasperi|4/17/2018|Rio de Janeiro|5300|NaN|15900|
|526|3360|HL1918|iPhone|2|Natalia|Marinho|12/15/2018|Rio de Janeiro|5300|NaN|10600|
|527|3367|HL8851|Notebook|4|Sylvio|Bernhardt|2/25/2018|Rio de Janeiro|3500|NaN|14000|
|528|3382|HL2714|Tablet|4|Rebeca|Taylor|4/8/2018|Rio de Janeiro|1600|NaN|6400|
|529|3383|HL1918|iPhone|3|Vitor|Boccaletti|7/7/2018|Rio de Janeiro|5300|NaN|15900|
|530|3386|HL1148|Câmera|3|Carlos|Araujo|5/24/2018|Rio de Janeiro|2100|NaN|6300|
|531|3393|HL4379|Televisão|4|Guilherme|Jordao|2/28/2018|Rio de Janeiro|2500|NaN|10000|
|532|3401|HL7348|SmartWatch|4|David|Campelo|10/26/2018|Rio de Janeiro|1400|NaN|5600|
|533|3409|HL9962|Android|3|Rafaela|Gonçalves|12/4/2018|Rio de Janeiro|3400|NaN|10200|
|534|3415|HL9962|Android|4|Bruna|Rangel|4/16/2018|Rio de Janeiro|3400|NaN|13600|
|535|3433|HL4379|Televisão|1|Pedro|Martins|12/11/2018|Rio de Janeiro|2500|NaN|2500|
|536|3439|HL7348|SmartWatch|2|João|Fonseca|4/25/2018|Rio de Janeiro|1400|NaN|2800|
|537|3465|HL1918|iPhone|5|João|Siqueira|5/11/2018|Rio de Janeiro|5300|NaN|26500|
|538|3466|HL1918|iPhone|4|Jéssica|Netto|2/2/2018|Rio de Janeiro|5300|NaN|21200|
|539|3472|HL8851|Notebook|3|Antonio|Manhães|2/12/2018|Rio de Janeiro|3500|NaN|10500|
|540|3474|HL1148|Câmera|3|Lunna|Vannier|6/13/2018|Rio de Janeiro|2100|NaN|6300|
|541|3477|HL9962|Android|5|Luiz|Freire|12/12/2018|Rio de Janeiro|3400|NaN|17000|
|542|3493|HL4379|Televisão|1|Carlos|Souza|8/24/2018|Rio de Janeiro|2500|NaN|2500|
|543|3500|HL1918|iPhone|5|Thainá|Binello|6/5/2018|Rio de Janeiro|5300|NaN|26500|
|544|3514|HL8851|Notebook|4|João|Aires|7/27/2018|Rio de Janeiro|3500|NaN|14000|
|545|3523|HL2714|Tablet|4|Caio|Silva|2/4/2018|Rio de Janeiro|1600|NaN|6400|
|546|3524|HL1918|iPhone|2|João|Pedrazza|4/23/2018|Rio de Janeiro|5300|NaN|10600|
|547|3528|HL4379|Televisão|3|Gabriel|Pereira|5/10/2018|Rio de Janeiro|2500|NaN|7500|
|548|3529|HL4379|Televisão|3|Luiza|Cabral|2/1/2018|Rio de Janeiro|2500|NaN|7500|
|549|3530|HL2714|Tablet|2|Adriane|Chagas|11/6/2018|Rio de Janeiro|1600|NaN|3200|
|550|3544|HL1918|iPhone|3|Lucas|Villanova|4/27/2018|Rio de Janeiro|5300|NaN|15900|
|551|3545|HL1918|iPhone|5|Caroline|Aquino|12/5/2018|Rio de Janeiro|5300|NaN|26500|
|552|3584|HL1918|iPhone|5|Sandy|Figueiredo|5/14/2018|Rio de Janeiro|5300|NaN|26500|
|553|3588|HL1918|iPhone|1|Jeferson|Costa|3/31/2018|Rio de Janeiro|5300|NaN|5300|
|554|3595|HL7348|SmartWatch|5|Leandro|Rodrigues|12/6/2018|Rio de Janeiro|1400|NaN|7000|
|555|3602|HL1918|iPhone|3|Luiza|Procaci|8/26/2018|Rio de Janeiro|5300|NaN|15900|
|556|3614|HL1148|Câmera|2|Gabrielle|Vasconcelos|5/23/2018|Rio de Janeiro|2100|NaN|4200|
|557|3617|HL4379|Televisão|5|Lázaro|Nascimento|8/10/2018|Rio de Janeiro|2500|NaN|12500|
|558|3626|HL7348|SmartWatch|2|Natalia|Andrade|1/4/2018|Rio de Janeiro|1400|NaN|2800|
|559|3627|HL7348|SmartWatch|3|Lara|Moreira|5/8/2018|Rio de Janeiro|1400|NaN|4200|
|560|3630|HL8851|Notebook|2|Mayara|Soares|5/25/2018|Rio de Janeiro|3500|NaN|7000|
|561|3639|HL4379|Televisão|1|Aline|Andrade|4/18/2018|Rio de Janeiro|2500|NaN|2500|
|562|3643|HL8851|Notebook|1|Alon|Pestana|8/20/2018|Rio de Janeiro|3500|NaN|3500|
|563|3644|HL1918|iPhone|4|Thainá|Binello|4/29/2018|Rio de Janeiro|5300|NaN|21200|
|564|3656|HL4379|Televisão|4|Carolina|Vasconcelos|12/30/2018|Rio de Janeiro|2500|NaN|10000|
|565|3660|HL9962|Android|2|Carlos|Assis|10/20/2018|Rio de Janeiro|3400|NaN|6800|
|566|3671|HL1918|iPhone|5|Rafael|Portela|11/6/2018|Rio de Janeiro|5300|NaN|26500|
|567|3675|HL7348|SmartWatch|5|Lucas|Destri|12/19/2018|Rio de Janeiro|1400|NaN|7000|
|568|3687|HL1918|iPhone|2|Patrick|Silva|3/31/2018|Rio de Janeiro|5300|NaN|10600|
|569|3688|HL4379|Televisão|1|Luis|Villanova|6/30/2018|Rio de Janeiro|2500|NaN|2500|
|570|3689|HL1148|Câmera|4|João|Monteiro|9/13/2018|Rio de Janeiro|2100|NaN|8400|
|571|3707|HL1918|iPhone|1|Luis|Souza|3/5/2018|Rio de Janeiro|5300|NaN|5300|
|572|3717|HL1148|Câmera|2|Guilherme|Merotto|12/1/2018|Rio de Janeiro|2100|NaN|4200|
|573|3725|HL8851|Notebook|2|Manuela|Ferreira|9/2/2018|Rio de Janeiro|3500|NaN|7000|
|574|3726|HL9962|Android|5|Lorena|Carvalho|10/28/2018|Rio de Janeiro|3400|NaN|17000|
|575|3731|HL9962|Android|4|Thiago|Nóbrega|6/23/2018|Rio de Janeiro|3400|NaN|13600|
|576|3737|HL9962|Android|5|Matheus|Miranda|12/15/2018|Rio de Janeiro|3400|NaN|17000|
|577|3740|HL1148|Câmera|4|Diego|Rodrigues|11/6/2018|Rio de Janeiro|2100|NaN|8400|
|578|3744|HL1918|iPhone|4|Rogério|Pereira|11/25/2018|Rio de Janeiro|5300|NaN|21200|
|579|3750|HL1148|Câmera|4|Daniel|Cardoso|12/19/2018|Rio de Janeiro|2100|NaN|8400|
|580|3752|HL8851|Notebook|1|Lucas|Araújo|12/27/2018|Rio de Janeiro|3500|NaN|3500|
|581|3795|HL1918|iPhone|2|Juliana|Pacheco|1/14/2018|Rio de Janeiro|5300|NaN|10600|
|582|3804|HL8851|Notebook|1|Isabel|Mesquita|11/17/2018|Rio de Janeiro|3500|NaN|3500|
|583|3808|HL7348|SmartWatch|3|Lucas|Coelho|6/29/2018|Rio de Janeiro|1400|NaN|4200|
|584|3816|HL1918|iPhone|4|Fernanda|Figueiredo|1/28/2018|Rio de Janeiro|5300|NaN|21200|
|585|3832|HL2714|Tablet|5|João|Fonseca|10/14/2018|Rio de Janeiro|1600|NaN|8000|
|586|3837|HL2714|Tablet|3|Jeferson|Sone|12/25/2018|Rio de Janeiro|1600|NaN|4800|
|587|3844|HL2714|Tablet|1|Matheus|Figueiredo|4/21/2018|Rio de Janeiro|1600|NaN|1600|
|588|3845|HL1918|iPhone|3|Julia|Leig|6/12/2018|Rio de Janeiro|5300|NaN|15900|
|589|3858|HL2714|Tablet|4|Carlos|Mesquita|12/9/2018|Rio de Janeiro|1600|NaN|6400|
|590|3863|HL1918|iPhone|3|João|Júnior|5/20/2018|Rio de Janeiro|5300|NaN|15900|
|591|3902|HL4379|Televisão|1|Eduardo|Vargas|8/27/2018|Rio de Janeiro|2500|NaN|2500|
|592|3903|HL1918|iPhone|5|Arthur|Souza|3/2/2018|Rio de Janeiro|5300|NaN|26500|
|593|3908|HL1918|iPhone|2|Carlos|Assis|12/2/2018|Rio de Janeiro|5300|NaN|10600|
|594|3912|HL1918|iPhone|5|Wendela|Veloso|12/7/2018|Rio de Janeiro|5300|NaN|26500|
|595|3918|HL1918|iPhone|2|Ana|Michetti|12/26/2018|Rio de Janeiro|5300|NaN|10600|
|596|3925|HL8851|Notebook|4|Karina|Camara|12/27/2018|Rio de Janeiro|3500|NaN|14000|
|597|3932|HL2714|Tablet|2|Danilo|Rubim|2/17/2018|Rio de Janeiro|1600|NaN|3200|
|598|3949|HL4379|Televisão|1|Victor|Oliveira|12/12/2018|Rio de Janeiro|2500|NaN|2500|
|599|3950|HL1148|Câmera|4|Caio|Affonso|12/3/2018|Rio de Janeiro|2100|NaN|8400|
|600|3960|HL1148|Câmera|3|Pedro|Ferrari|3/5/2018|Rio de Janeiro|2100|NaN|6300|
|601|3962|HL9962|Android|5|Guilherme|Castilho|2/14/2018|Rio de Janeiro|3400|NaN|17000|
|602|3965|HL1918|iPhone|4|Eduardo|Quindeler|8/31/2018|Rio de Janeiro|5300|NaN|21200|
|603|3971|HL1918|iPhone|2|Nicolas|Monteiro|5/29/2018|Rio de Janeiro|5300|NaN|10600|
|604|3980|HL4379|Televisão|4|Mônica|Rotolo|3/23/2018|Rio de Janeiro|2500|NaN|10000|
|605|3981|HL1918|iPhone|4|Natalia|Accioly|2/21/2018|Rio de Janeiro|5300|NaN|21200|
|606|3985|HL9962|Android|4|Stephanie|Novak|7/9/2018|Rio de Janeiro|3400|NaN|13600|
|607|3986|HL4379|Televisão|4|José|Vieira|10/2/2018|Rio de Janeiro|2500|NaN|10000|
|608|3993|HL4379|Televisão|5|Raphael|Filho|2/6/2018|Rio de Janeiro|2500|NaN|12500|
|609|4002|HL7348|SmartWatch|4|Nathalia|Ventura|8/27/2018|Rio de Janeiro|1400|NaN|5600|
|610|4008|HL1148|Câmera|3|Thays|Castro|9/14/2018|Rio de Janeiro|2100|NaN|6300|
|611|4010|HL1918|iPhone|3|Mayara|Soares|1/22/2018|Rio de Janeiro|5300|NaN|15900|
|612|4024|HL9962|Android|5|Lázaro|Nascimento|3/14/2018|Rio de Janeiro|3400|NaN|17000|
|613|4030|HL4379|Televisão|2|Willian|Albino|7/25/2018|Rio de Janeiro|2500|NaN|5000|
|614|4044|HL9962|Android|1|Lunna|Vannier|7/23/2018|Rio de Janeiro|3400|NaN|3400|
|615|4048|HL1918|iPhone|4|Breno|Farias|9/15/2018|Rio de Janeiro|5300|NaN|21200|
|616|4062|HL8851|Notebook|2|Audir|Franco|10/22/2018|Rio de Janeiro|3500|NaN|7000|
|617|4077|HL1918|iPhone|2|Carlos|Cardoso|8/2/2018|Rio de Janeiro|5300|NaN|10600|
|618|4079|HL1918|iPhone|5|Yasser|Calbucci|11/29/2018|Rio de Janeiro|5300|NaN|26500|
|619|4086|HL1918|iPhone|4|Thales|Santos|5/27/2018|Rio de Janeiro|5300|NaN|21200|
|620|4091|HL1918|iPhone|4|Lívia|Marques|6/11/2018|Rio de Janeiro|5300|NaN|21200|
|621|4104|HL4379|Televisão|4|Antonio|Manhães|6/17/2018|Rio de Janeiro|2500|NaN|10000|
|622|4106|HL1918|iPhone|3|Matheus|Silva|7/8/2018|Rio de Janeiro|5300|NaN|15900|
|623|4109|HL1918|iPhone|4|Bruna|Ramos|7/20/2018|Rio de Janeiro|5300|NaN|21200|
|624|4111|HL7348|SmartWatch|2|Victor|Magalhães|6/27/2018|Rio de Janeiro|1400|NaN|2800|
|625|4123|HL9962|Android|3|Paulo|Campos|1/19/2018|Rio de Janeiro|3400|NaN|10200|
|626|4128|HL7348|SmartWatch|5|Jéssica|Stefanelli|3/20/2018|Rio de Janeiro|1400|NaN|7000|
|627|4133|HL1918|iPhone|4|Matheus|Gomes|2/21/2018|Rio de Janeiro|5300|NaN|21200|
|628|4138|HL1918|iPhone|1|Silvio|Fahrnholz|12/15/2018|Rio de Janeiro|5300|NaN|5300|
|629|4143|HL9962|Android|5|Sandy|Ribeiro|4/6/2018|Rio de Janeiro|3400|NaN|17000|
|630|4149|HL2714|Tablet|1|Marina|Marins|5/3/2018|Rio de Janeiro|1600|NaN|1600|
|631|4155|HL9962|Android|4|Guilherme|Monteiro|9/28/2018|Rio de Janeiro|3400|NaN|13600|
|632|4170|HL1918|iPhone|2|Yasmim|Bittencourt|1/12/2018|Rio de Janeiro|5300|NaN|10600|
|633|4175|HL4379|Televisão|3|Lucas|Machado|3/28/2018|Rio de Janeiro|2500|NaN|7500|
|634|4180|HL4379|Televisão|5|Thiago|Veiga|1/4/2018|Rio de Janeiro|2500|NaN|12500|
|635|4183|HL4379|Televisão|5|Samara|Pinto|5/13/2018|Rio de Janeiro|2500|NaN|12500|
|636|4190|HL7348|SmartWatch|3|Kimberly|Sad|9/29/2018|Rio de Janeiro|1400|NaN|4200|
|637|4197|HL2714|Tablet|2|Bianca|Procaci|10/30/2018|Rio de Janeiro|1600|NaN|3200|
|638|4200|HL1918|iPhone|4|Jessica|Cordovil|2/7/2018|Rio de Janeiro|5300|NaN|21200|
|639|4202|HL1918|iPhone|4|Marcela|Gasperi|5/10/2018|Rio de Janeiro|5300|NaN|21200|
|640|4213|HL7348|SmartWatch|5|Marina|Mesquita|9/16/2018|Rio de Janeiro|1400|NaN|7000|
|641|4215|HL1918|iPhone|3|Juliana|Pacheco|7/13/2018|Rio de Janeiro|5300|NaN|15900|
|642|4219|HL1918|iPhone|2|Julie|Ferreira|6/22/2018|Rio de Janeiro|5300|NaN|10600|
|643|4226|HL4379|Televisão|5|Kimberly|Sad|3/3/2018|Rio de Janeiro|2500|NaN|12500|
|644|4236|HL9962|Android|4|Amanda|Braga|5/21/2018|Rio de Janeiro|3400|NaN|13600|
|645|4240|HL4379|Televisão|3|Cícero|Lima|1/12/2018|Rio de Janeiro|2500|NaN|7500|
|646|4249|HL1918|iPhone|4|Carolina|Brum|8/23/2018|Rio de Janeiro|5300|NaN|21200|
|647|4256|HL1918|iPhone|2|Maria|Moita|2/23/2018|Rio de Janeiro|5300|NaN|10600|
|648|4257|HL1918|iPhone|1|Gustavo|Azevedo|3/14/2018|Rio de Janeiro|5300|NaN|5300|
|649|4261|HL1918|iPhone|5|Fabio|Boccaletti|7/15/2018|Rio de Janeiro|5300|NaN|26500|
|650|4265|HL1918|iPhone|1|Danilo|Rubim|6/4/2018|Rio de Janeiro|5300|NaN|5300|
|651|4267|HL8851|Notebook|3|Luis|Garcia|3/15/2018|Rio de Janeiro|3500|NaN|10500|
|652|4279|HL1918|iPhone|3|Isabela|Teixeira|12/20/2018|Rio de Janeiro|5300|NaN|15900|
|653|4289|HL1918|iPhone|4|Victoria|Mazza|3/7/2018|Rio de Janeiro|5300|NaN|21200|
|654|4290|HL9962|Android|1|Roberta|Nogueira|5/1/2018|Rio de Janeiro|3400|NaN|3400|
|655|4304|HL1918|iPhone|3|Carlos|Portela|2/2/2018|Rio de Janeiro|5300|NaN|15900|
|656|4311|HL4379|Televisão|1|Ulisses|Filho|9/9/2018|Rio de Janeiro|2500|NaN|2500|
|657|4313|HL1918|iPhone|2|Natalia|Accioly|9/7/2018|Rio de Janeiro|5300|NaN|10600|
|658|4325|HL7348|SmartWatch|2|Joana|Calmon|10/27/2018|Rio de Janeiro|1400|NaN|2800|
|659|4327|HL1148|Câmera|3|Matheus|Afonso|10/21/2018|Rio de Janeiro|2100|NaN|6300|
|660|4330|HL7348|SmartWatch|1|Juan|Barbosa|11/8/2018|Rio de Janeiro|1400|NaN|1400|
|661|4333|HL1918|iPhone|4|Felipe|Freitas|4/12/2018|Rio de Janeiro|5300|NaN|21200|
|662|4341|HL4379|Televisão|2|Eduardo|Soares|5/27/2018|Rio de Janeiro|2500|NaN|5000|
|663|4350|HL4379|Televisão|2|Isabela|Chagas|6/8/2018|Rio de Janeiro|2500|NaN|5000|
|664|4355|HL1918|iPhone|3|Raul|Junqueira|10/6/2018|Rio de Janeiro|5300|NaN|15900|
|665|4362|HL4379|Televisão|1|Gabriel|Thoni|4/6/2018|Rio de Janeiro|2500|NaN|2500|
|666|4373|HL7348|SmartWatch|4|Eduardo|Vargas|4/4/2018|Rio de Janeiro|1400|NaN|5600|
|667|4374|HL4379|Televisão|5|Vitor|Campos|12/9/2018|Rio de Janeiro|2500|NaN|12500|
|668|4377|HL8851|Notebook|4|Rebeca|Manhães|3/20/2018|Rio de Janeiro|3500|NaN|14000|
|669|4383|HL2714|Tablet|1|Tadeu|Sousa|4/18/2018|Rio de Janeiro|1600|NaN|1600|
|670|4384|HL1148|Câmera|3|Deysiane|Bach|12/2/2018|Rio de Janeiro|2100|NaN|6300|
|671|4392|HL1918|iPhone|1|Alon|Pestana|3/31/2018|Rio de Janeiro|5300|NaN|5300|
|672|4396|HL9962|Android|4|Renan|Ventura|3/11/2018|Rio de Janeiro|3400|NaN|13600|
|673|4400|HL1918|iPhone|5|Breno|Varella|11/26/2018|Rio de Janeiro|5300|NaN|26500|
|674|4402|HL9962|Android|4|Raissa|Negrelli|6/26/2018|Rio de Janeiro|3400|NaN|13600|
|675|4412|HL9962|Android|1|Bianca|Paz|8/25/2018|Rio de Janeiro|3400|NaN|3400|
|676|4413|HL1918|iPhone|5|Silvio|Provenzano|9/15/2018|Rio de Janeiro|5300|NaN|26500|
|677|4417|HL2714|Tablet|5|Ulisses|Arruda|5/12/2018|Rio de Janeiro|1600|NaN|8000|
|678|4430|HL7348|SmartWatch|3|Daniel|Sousa|4/26/2018|Rio de Janeiro|1400|NaN|4200|
|679|4434|HL4379|Televisão|3|Luiza|Procaci|4/7/2018|Rio de Janeiro|2500|NaN|7500|
|680|4436|HL1918|iPhone|4|Luiza|Cavalcanti|1/13/2018|Rio de Janeiro|5300|NaN|21200|
|681|4440|HL1918|iPhone|3|Vittorio|Freitas|11/11/2018|Rio de Janeiro|5300|NaN|15900|
|682|4441|HL7348|SmartWatch|4|Joana|Calmon|8/18/2018|Rio de Janeiro|1400|NaN|5600|
|683|4447|HL7348|SmartWatch|4|Pedro|Jorge|11/3/2018|Rio de Janeiro|1400|NaN|5600|
|684|4458|HL1918|iPhone|5|Patrícia|Fernandes|6/9/2018|Rio de Janeiro|5300|NaN|26500|
|685|4465|HL4379|Televisão|3|Juliana|Souza|1/9/2018|Rio de Janeiro|2500|NaN|7500|
|686|4470|HL1148|Câmera|2|Gabriel|Azevedo|11/22/2018|Rio de Janeiro|2100|NaN|4200|
|687|4480|HL1918|iPhone|1|Fabio|Ramos|1/5/2018|Rio de Janeiro|5300|NaN|5300|
|688|4485|HL7348|SmartWatch|3|Alon|Guedes|5/22/2018|Rio de Janeiro|1400|NaN|4200|
|689|4499|HL8851|Notebook|4|Anderson|Cavalcanti|9/23/2018|Rio de Janeiro|3500|NaN|14000|
|690|4511|HL1918|iPhone|2|Carlos|Azevedo|6/21/2018|Rio de Janeiro|5300|NaN|10600|
|691|4513|HL9962|Android|2|José|Carvalho|6/26/2018|Rio de Janeiro|3400|NaN|6800|
|692|4522|HL7348|SmartWatch|4|Victor|Lira|3/12/2018|Rio de Janeiro|1400|NaN|5600|
|693|4523|HL7348|SmartWatch|5|Debora|Silva|1/1/2018|Rio de Janeiro|1400|NaN|7000|
|694|4560|HL1918|iPhone|5|Julia|Teixeira|11/21/2018|Rio de Janeiro|5300|NaN|26500|
|695|4561|HL1918|iPhone|3|Mariana|Miranda|12/20/2018|Rio de Janeiro|5300|NaN|15900|
|696|4572|HL1148|Câmera|1|Breno|Farias|4/8/2018|Rio de Janeiro|2100|NaN|2100|
|697|4584|HL1918|iPhone|3|Vinícius|Antunes|1/19/2018|Rio de Janeiro|5300|NaN|15900|
|698|4594|HL1918|iPhone|4|Marina|Gama|1/25/2018|Rio de Janeiro|5300|NaN|21200|
|699|4596|HL4379|Televisão|4|Ruan|Gonçalves|12/23/2018|Rio de Janeiro|2500|NaN|10000|
|700|4599|HL1918|iPhone|4|Rubens|Netto|11/4/2018|Rio de Janeiro|5300|NaN|21200|
|701|4606|HL4379|Televisão|3|Wilson|Farias|7/19/2018|Rio de Janeiro|2500|NaN|7500|
|702|4609|HL4379|Televisão|4|Sandy|Ribeiro|7/9/2018|Rio de Janeiro|2500|NaN|10000|
|703|4629|HL1918|iPhone|2|Juliana|Barreira|5/3/2018|Rio de Janeiro|5300|NaN|10600|
|704|4634|HL7348|SmartWatch|2|Bianca|Tatsch|11/21/2018|Rio de Janeiro|1400|NaN|2800|
|705|4638|HL2714|Tablet|5|Ana|Felippe|6/17/2018|Rio de Janeiro|1600|NaN|8000|
|706|4644|HL1918|iPhone|5|Mariana|Sousa|6/10/2018|Rio de Janeiro|5300|NaN|26500|
|707|4666|HL9962|Android|2|Priscila|Suzano|12/30/2018|Rio de Janeiro|3400|NaN|6800|
|708|4677|HL1148|Câmera|4|Raíssa|Oros|4/29/2018|Rio de Janeiro|2100|NaN|8400|
|709|4687|HL7348|SmartWatch|1|José|Jesus|9/28/2018|Rio de Janeiro|1400|NaN|1400|
|710|4697|HL1918|iPhone|2|Jonatas|Passos|9/16/2018|Rio de Janeiro|5300|NaN|10600|
|711|4698|HL2714|Tablet|3|Gabriel|Pereira|8/9/2018|Rio de Janeiro|1600|NaN|4800|
|712|4710|HL1148|Câmera|3|Matheus|Miranda|2/16/2018|Rio de Janeiro|2100|NaN|6300|
|713|4718|HL2714|Tablet|5|Raul|Junqueira|9/23/2018|Rio de Janeiro|1600|NaN|8000|
|714|4731|HL9962|Android|4|Carlos|Azevedo|8/16/2018|Rio de Janeiro|3400|NaN|13600|
|715|4732|HL4379|Televisão|1|Pedro|Dalforne|9/26/2018|Rio de Janeiro|2500|NaN|2500|
|716|4733|HL2714|Tablet|4|Caio|Silva|11/25/2018|Rio de Janeiro|1600|NaN|6400|
|717|4738|HL1918|iPhone|5|Priscila|Suzano|4/6/2018|Rio de Janeiro|5300|NaN|26500|
|718|4742|HL1918|iPhone|4|Guilherme|Lima|2/5/2018|Rio de Janeiro|5300|NaN|21200|
|719|4746|HL1918|iPhone|4|Marcelo|Magalhães|11/29/2018|Rio de Janeiro|5300|NaN|21200|
|720|4759|HL1918|iPhone|4|Pedro|Ferrari|11/13/2018|Rio de Janeiro|5300|NaN|21200|
|721|4763|HL1148|Câmera|4|Marina|Aragão|7/16/2018|Rio de Janeiro|2100|NaN|8400|
|722|4767|HL1918|iPhone|2|Iuri|Neto|10/24/2018|Rio de Janeiro|5300|NaN|10600|
|723|4781|HL4379|Televisão|3|Alberto|Silveira|10/28/2018|Rio de Janeiro|2500|NaN|7500|
|724|4782|HL4379|Televisão|4|Lara|Moreira|2/24/2018|Rio de Janeiro|2500|NaN|10000|
|725|4784|HL1918|iPhone|1|Luíza|Garcia|9/14/2018|Rio de Janeiro|5300|NaN|5300|
|726|4796|HL4379|Televisão|1|Carolina|Rachide|9/14/2018|Rio de Janeiro|2500|NaN|2500|
|727|4810|HL1918|iPhone|3|Alexandre|Dantas|12/23/2018|Rio de Janeiro|5300|NaN|15900|
|728|4814|HL1918|iPhone|3|Gabriella|Lopes|12/22/2018|Rio de Janeiro|5300|NaN|15900|
|729|4819|HL1918|iPhone|5|Luiza|Cabral|8/15/2018|Rio de Janeiro|5300|NaN|26500|
|730|4821|HL2714|Tablet|4|Isabella|Rodrigues|9/15/2018|Rio de Janeiro|1600|NaN|6400|
|731|4822|HL7348|SmartWatch|3|Cassio|Faria|9/9/2018|Rio de Janeiro|1400|NaN|4200|
|732|4839|HL4379|Televisão|4|Adriane|Chagas|3/16/2018|Rio de Janeiro|2500|NaN|10000|
|733|4842|HL1918|iPhone|5|Fernanda|Silva|2/22/2018|Rio de Janeiro|5300|NaN|26500|
|734|4844|HL4379|Televisão|3|Júlia|Almeida|4/28/2018|Rio de Janeiro|2500|NaN|7500|
|735|4849|HL1918|iPhone|1|Breno|Varella|1/15/2018|Rio de Janeiro|5300|NaN|5300|
|736|4853|HL4379|Televisão|3|Caio|Silva|12/15/2018|Rio de Janeiro|2500|NaN|7500|
|737|4862|HL9962|Android|5|Bernardo|Nauenberg|5/6/2018|Rio de Janeiro|3400|NaN|17000|
|738|4875|HL4379|Televisão|3|Rogério|Pereira|5/23/2018|Rio de Janeiro|2500|NaN|7500|
|739|4877|HL4379|Televisão|3|Adrielle|Gabriel|12/30/2018|Rio de Janeiro|2500|NaN|7500|
|740|4893|HL1918|iPhone|4|Bernardo|Ribeiro|6/30/2018|Rio de Janeiro|5300|NaN|21200|
|741|4899|HL2714|Tablet|1|Luiz|Campista|12/7/2018|Rio de Janeiro|1600|NaN|1600|
|742|4924|HL1918|iPhone|4|Miguel|Carneiro|10/18/2018|Rio de Janeiro|5300|NaN|21200|
|743|4925|HL7348|SmartWatch|1|Camila|Sobral|7/2/2018|Rio de Janeiro|1400|NaN|1400|
|744|4927|HL1918|iPhone|5|Arthur|Pereira|10/29/2018|Rio de Janeiro|5300|NaN|26500|
|745|4946|HL1918|iPhone|2|Eduardo|Peluzo|2/13/2018|Rio de Janeiro|5300|NaN|10600|
|746|4955|HL2714|Tablet|2|Yasmim|Verly|10/19/2018|Rio de Janeiro|1600|NaN|3200|
|747|4966|HL1918|iPhone|1|Isabella|Scalabrin|1/26/2018|Rio de Janeiro|5300|NaN|5300|
|748|4969|HL1918|iPhone|2|Felipe|Cavalcanti|6/23/2018|Rio de Janeiro|5300|NaN|10600|
|749|4981|HL1918|iPhone|5|Juliana|Guimarães|4/5/2018|Rio de Janeiro|5300|NaN|26500|
|750|4983|HL9962|Android|3|Julia|Silva|1/31/2018|Rio de Janeiro|3400|NaN|10200|
|751|4985|HL1918|iPhone|4|Erick|Soares|12/31/2018|Rio de Janeiro|5300|NaN|21200|
|752|4986|HL1918|iPhone|1|Myllena|Corrêa|5/31/2018|Rio de Janeiro|5300|NaN|5300|
|753|4991|HL9962|Android|3|Paula|Calbucci|9/10/2018|Rio de Janeiro|3400|NaN|10200|
|754|4996|HL4379|Televisão|1|Rebeca|Manhães|3/24/2018|Rio de Janeiro|2500|NaN|2500|
|755|5000|HL1918|iPhone|1|João|Pedrazza|9/19/2018|Rio de Janeiro|5300|NaN|5300|
|756|5004|HL4379|Televisão|2|Rafael|Guimarães|6/17/2018|Rio de Janeiro|2500|NaN|5000|
|757|5014|HL4379|Televisão|4|Giovanna|Santos|12/26/2018|Rio de Janeiro|2500|NaN|10000|
|758|5021|HL1918|iPhone|3|Julia|Aliani|11/15/2018|Rio de Janeiro|5300|NaN|15900|
|759|5024|HL8851|Notebook|1|Maria|Motta|6/5/2018|Rio de Janeiro|3500|NaN|3500|
|760|5025|HL9962|Android|1|Matheus|Santos|2/23/2018|Rio de Janeiro|3400|NaN|3400|
|761|5042|HL4379|Televisão|3|Juliana|Goes|2/23/2018|Rio de Janeiro|2500|NaN|7500|
|762|5076|HL1918|iPhone|1|Marcelo|Pereira|6/23/2018|Rio de Janeiro|5300|NaN|5300|
|763|5086|HL1918|iPhone|5|Ulisses|Filho|2/20/2018|Rio de Janeiro|5300|NaN|26500|
|764|5092|HL2714|Tablet|2|Victor|Gomes|11/19/2018|Rio de Janeiro|1600|NaN|3200|
|765|5102|HL1918|iPhone|4|Lucas|Villanova|6/25/2018|Rio de Janeiro|5300|NaN|21200|
|766|5109|HL8851|Notebook|3|Ana|Felippe|10/21/2018|Rio de Janeiro|3500|NaN|10500|
|767|5117|HL7348|SmartWatch|3|Paloma|Sperandei|8/17/2018|Rio de Janeiro|1400|NaN|4200|
|768|5119|HL1918|iPhone|3|Juliana|Hollander|7/6/2018|Rio de Janeiro|5300|NaN|15900|
|769|5123|HL1148|Câmera|3|Stefan|Nunes|7/29/2018|Rio de Janeiro|2100|NaN|6300|
|770|5135|HL8851|Notebook|5|Willian|Albino|9/21/2018|Rio de Janeiro|3500|NaN|17500|
|771|5142|HL1918|iPhone|4|Alberto|Silveira|5/12/2018|Rio de Janeiro|5300|NaN|21200|
|772|5159|HL1918|iPhone|5|Thales|Gouvêa|7/21/2018|Rio de Janeiro|5300|NaN|26500|
|773|5164|HL4379|Televisão|3|Felipe|Cavalcanti|8/11/2018|Rio de Janeiro|2500|NaN|7500|
|774|5166|HL2714|Tablet|3|Raissa|Negrelli|12/27/2018|Rio de Janeiro|1600|NaN|4800|
|775|5167|HL4379|Televisão|5|Guilherme|Seixas|1/31/2018|Rio de Janeiro|2500|NaN|12500|
|776|5178|HL2714|Tablet|1|Cláudio|Aragão|1/31/2018|Rio de Janeiro|1600|NaN|1600|
|777|5181|HL1918|iPhone|5|Caroline|Cavalcanti|10/17/2018|Rio de Janeiro|5300|NaN|26500|
|778|5187|HL4379|Televisão|5|Amanda|Braga|5/18/2018|Rio de Janeiro|2500|NaN|12500|
|779|5194|HL1918|iPhone|2|Breno|Caputo|1/1/2018|Rio de Janeiro|5300|NaN|10600|
|780|5202|HL1918|iPhone|5|Anderson|Martins|5/25/2018|Rio de Janeiro|5300|NaN|26500|
|781|5204|HL1918|iPhone|3|Letícia|Araujo|9/9/2018|Rio de Janeiro|5300|NaN|15900|
|782|5212|HL1918|iPhone|3|Fernanda|Coutinho|7/5/2018|Rio de Janeiro|5300|NaN|15900|
|783|5214|HL9962|Android|3|Marcela|Gasperi|5/2/2018|Rio de Janeiro|3400|NaN|10200|
|784|5221|HL4379|Televisão|4|Luiza|Cavalcanti|2/17/2018|Rio de Janeiro|2500|NaN|10000|
|785|5224|HL9962|Android|2|Anderson|Cavalcanti|1/27/2018|Rio de Janeiro|3400|NaN|6800|
|786|5227|HL4379|Televisão|1|Vanessa|Bach|6/25/2018|Rio de Janeiro|2500|NaN|2500|
|787|5232|HL7348|SmartWatch|3|Adrielle|Vieira|3/2/2018|Rio de Janeiro|1400|NaN|4200|
|788|5235|HL1148|Câmera|5|Thales|Andrade|6/30/2018|Rio de Janeiro|2100|NaN|10500|
|789|5236|HL2714|Tablet|1|Nina|Magalhães|12/11/2018|Rio de Janeiro|1600|NaN|1600|
|790|5238|HL7348|SmartWatch|1|Lara|Moreira|9/11/2018|Rio de Janeiro|1400|NaN|1400|
|791|5250|HL4379|Televisão|5|Victor|Corrêa|12/28/2018|Rio de Janeiro|2500|NaN|12500|
|792|5255|HL1918|iPhone|5|Juan|Barbosa|10/26/2018|Rio de Janeiro|5300|NaN|26500|
|793|5273|HL8851|Notebook|5|Ana|Soledade|7/5/2018|Rio de Janeiro|3500|NaN|17500|
|794|5283|HL9962|Android|2|Maria|Correa|7/26/2018|Rio de Janeiro|3400|NaN|6800|
|795|5287|HL1918|iPhone|3|Raissa|Pinheiro|4/25/2018|Rio de Janeiro|5300|NaN|15900|
|796|5298|HL1148|Câmera|1|Caio|Cardoso|2/28/2018|Rio de Janeiro|2100|NaN|2100|
|797|5301|HL7348|SmartWatch|4|Lázaro|Villanova|6/9/2018|Rio de Janeiro|1400|NaN|5600|
|798|5302|HL1918|iPhone|5|Carolina|Figueiredo|5/2/2018|Rio de Janeiro|5300|NaN|26500|
|799|5308|HL1918|iPhone|4|Milena|Pereira|1/28/2018|Rio de Janeiro|5300|NaN|21200|
|800|5309|HL4379|Televisão|5|Thainá|Binello|2/6/2018|Rio de Janeiro|2500|NaN|12500|
|801|5315|HL7348|SmartWatch|4|Camilla|Cardeman|11/20/2018|Rio de Janeiro|1400|NaN|5600|
|802|5317|HL1918|iPhone|2|Alon|Fahrnholz|2/21/2018|Rio de Janeiro|5300|NaN|10600|
|803|5323|HL9962|Android|5|Fernanda|Figueiredo|6/2/2018|Rio de Janeiro|3400|NaN|17000|
|804|5333|HL7348|SmartWatch|2|Camilla|Cardeman|7/8/2018|Rio de Janeiro|1400|NaN|2800|
|805|5368|HL4379|Televisão|5|Pedro|Oliveira|5/10/2018|Rio de Janeiro|2500|NaN|12500|
|806|5392|HL7348|SmartWatch|3|Fernanda|Figueiredo|4/23/2018|Rio de Janeiro|1400|NaN|4200|
|807|5394|HL1148|Câmera|3|Pedro|Conceição|11/28/2018|Rio de Janeiro|2100|NaN|6300|
|808|5396|HL1918|iPhone|3|Ramon|Araujo|2/14/2018|Rio de Janeiro|5300|NaN|15900|
|809|5403|HL1918|iPhone|2|Nina|Magalhães|10/14/2018|Rio de Janeiro|5300|NaN|10600|
|810|5409|HL2714|Tablet|1|Sarah|Souza|3/16/2018|Rio de Janeiro|1600|NaN|1600|
|811|5429|HL8851|Notebook|5|Juliana|Guimarães|2/18/2018|Rio de Janeiro|3500|NaN|17500|
|812|5430|HL4379|Televisão|2|Raphael|Kurtz|3/30/2018|Rio de Janeiro|2500|NaN|5000|
|813|5445|HL1148|Câmera|3|Milena|Pereira|7/16/2018|Rio de Janeiro|2100|NaN|6300|
|814|5451|HL4379|Televisão|2|Beatriz|Perdomo|2/13/2018|Rio de Janeiro|2500|NaN|5000|
|815|5454|HL1918|iPhone|5|Raphael|Machado|5/11/2018|Rio de Janeiro|5300|NaN|26500|
|816|5463|HL8851|Notebook|2|Juliana|Souza|6/14/2018|Rio de Janeiro|3500|NaN|7000|
|817|5476|HL1918|iPhone|5|Gabriel|Rubim|6/9/2018|Rio de Janeiro|5300|NaN|26500|
|818|5480|HL1918|iPhone|3|Vivianne|Rodrigues|10/13/2018|Rio de Janeiro|5300|NaN|15900|
|819|5485|HL2714|Tablet|4|Pedro|Bitencourt|11/18/2018|Rio de Janeiro|1600|NaN|6400|
|820|5486|HL1148|Câmera|3|Rafaela|Gonçalves|12/26/2018|Rio de Janeiro|2100|NaN|6300|
|821|5490|HL2714|Tablet|1|Letícia|Rodrigues|11/8/2018|Rio de Janeiro|1600|NaN|1600|
|822|5494|HL1918|iPhone|3|Adriana|Carneiro|11/24/2018|Rio de Janeiro|5300|NaN|15900|
|823|5496|HL8851|Notebook|4|Thayane|Resende|1/21/2018|Rio de Janeiro|3500|NaN|14000|
|824|5503|HL4379|Televisão|5|Luíza|Garcia|8/31/2018|Rio de Janeiro|2500|NaN|12500|
|825|5504|HL9962|Android|3|Thiago|Costa|5/17/2018|Rio de Janeiro|3400|NaN|10200|
|826|5505|HL1918|iPhone|3|Rilson|Guedes|7/1/2018|Rio de Janeiro|5300|NaN|15900|
|827|5516|HL1918|iPhone|3|Anízio|Carvalho|12/6/2018|Rio de Janeiro|5300|NaN|15900|
|828|5521|HL4379|Televisão|2|Lívia|Tanaka|3/27/2018|Rio de Janeiro|2500|NaN|5000|
|829|5527|HL2714|Tablet|4|Felipe|Júnior|2/24/2018|Rio de Janeiro|1600|NaN|6400|
|830|5542|HL4379|Televisão|3|Thaís|Ribeiro|8/4/2018|Rio de Janeiro|2500|NaN|7500|
|831|5544|HL7348|SmartWatch|3|Felipe|Cavalcanti|3/31/2018|Rio de Janeiro|1400|NaN|4200|
|832|5545|HL2714|Tablet|3|Gabriel|Pereira|8/5/2018|Rio de Janeiro|1600|NaN|4800|
|833|5546|HL1148|Câmera|5|Lucas|Lacerda|8/9/2018|Rio de Janeiro|2100|NaN|10500|
|834|5548|HL8851|Notebook|3|Caio|Caldas|1/13/2018|Rio de Janeiro|3500|NaN|10500|
|835|5554|HL1918|iPhone|2|Daniel|Ortiz|6/6/2018|Rio de Janeiro|5300|NaN|10600|
|836|5560|HL1918|iPhone|2|Marcelo|Borges|8/30/2018|Rio de Janeiro|5300|NaN|10600|
|837|5566|HL1148|Câmera|3|Paula|Cavalcanti|7/2/2018|Rio de Janeiro|2100|NaN|6300|
|838|5579|HL1918|iPhone|4|Lucas|Baptista|4/6/2018|Rio de Janeiro|5300|NaN|21200|
|839|5580|HL4379|Televisão|2|Ana|Soledade|11/23/2018|Rio de Janeiro|2500|NaN|5000|
|840|5594|HL1918|iPhone|2|Jonatas|Passos|5/4/2018|Rio de Janeiro|5300|NaN|10600|
|841|5595|HL1148|Câmera|3|Ana|Campos|3/19/2018|Rio de Janeiro|2100|NaN|6300|
|842|5596|HL1918|iPhone|5|Vitor|Arruda|8/6/2018|Rio de Janeiro|5300|NaN|26500|
|843|5604|HL1148|Câmera|2|Guilherme|Monteiro|5/28/2018|Rio de Janeiro|2100|NaN|4200|
|844|5619|HL1148|Câmera|4|Guilherme|Lima|4/29/2018|Rio de Janeiro|2100|NaN|8400|
|845|5632|HL2714|Tablet|1|Marcelo|Pereira|6/21/2018|Rio de Janeiro|1600|NaN|1600|
|846|5634|HL1918|iPhone|1|Bernardo|Ribeiro|1/2/2018|Rio de Janeiro|5300|NaN|5300|
|847|5635|HL4379|Televisão|3|Thaís|Pereira|7/15/2018|Rio de Janeiro|2500|NaN|7500|
|848|5646|HL1918|iPhone|1|Lucas|Lacerda|7/12/2018|Rio de Janeiro|5300|NaN|5300|
|849|5654|HL7348|SmartWatch|5|Luiza|Cabral|7/8/2018|Rio de Janeiro|1400|NaN|7000|
|850|5661|HL8851|Notebook|3|Luana|Santana|5/17/2018|Rio de Janeiro|3500|NaN|10500|
|851|5662|HL2714|Tablet|2|Luiza|Ribeiro|9/8/2018|Rio de Janeiro|1600|NaN|3200|
|852|5663|HL1918|iPhone|4|Juliana|Huon|1/24/2018|Rio de Janeiro|5300|NaN|21200|
|853|5679|HL7348|SmartWatch|3|Joyce|Souza|11/24/2018|Rio de Janeiro|1400|NaN|4200|
|854|5685|HL2714|Tablet|2|Antonio|Manhães|10/28/2018|Rio de Janeiro|1600|NaN|3200|
|855|5688|HL2714|Tablet|4|Gabriel|Azevedo|9/3/2018|Rio de Janeiro|1600|NaN|6400|
|856|5689|HL1918|iPhone|5|Daniel|Ortiz|6/15/2018|Rio de Janeiro|5300|NaN|26500|
|857|5697|HL1918|iPhone|1|Beatriz|Silva|3/16/2018|Rio de Janeiro|5300|NaN|5300|
|858|5705|HL1918|iPhone|3|Guilherme|Merotto|3/23/2018|Rio de Janeiro|5300|NaN|15900|
|859|5707|HL1918|iPhone|3|João|Araujo|12/13/2018|Rio de Janeiro|5300|NaN|15900|
|860|5709|HL8851|Notebook|1|Débora|Lopes|12/22/2018|Rio de Janeiro|3500|NaN|3500|
|861|5712|HL1918|iPhone|2|Thales|Andrade|9/6/2018|Rio de Janeiro|5300|NaN|10600|
|862|5714|HL7348|SmartWatch|4|Beatriz|Rocha|5/18/2018|Rio de Janeiro|1400|NaN|5600|
|863|5717|HL8851|Notebook|1|Danilo|Alves|3/29/2018|Rio de Janeiro|3500|NaN|3500|
|864|5721|HL1148|Câmera|2|Rebeca|Manhães|6/24/2018|Rio de Janeiro|2100|NaN|4200|
|865|5724|HL2714|Tablet|5|Bruna|Rangel|1/12/2018|Rio de Janeiro|1600|NaN|8000|
|866|5726|HL2714|Tablet|3|Lorena|Kohn|7/27/2018|Rio de Janeiro|1600|NaN|4800|
|867|5729|HL1918|iPhone|3|João|Ribeiro|8/8/2018|Rio de Janeiro|5300|NaN|15900|
|868|5730|HL1918|iPhone|4|Raissa|Pinheiro|11/14/2018|Rio de Janeiro|5300|NaN|21200|
|869|5732|HL8851|Notebook|3|Thomáz|Rodriguez|6/6/2018|Rio de Janeiro|3500|NaN|10500|
|870|5744|HL8851|Notebook|2|Gabrielle|Silva|8/16/2018|Rio de Janeiro|3500|NaN|7000|
|871|5745|HL4379|Televisão|2|Gabriel|Rubim|7/26/2018|Rio de Janeiro|2500|NaN|5000|
|872|5766|HL1918|iPhone|3|Marina|Cormack|7/28/2018|Rio de Janeiro|5300|NaN|15900|
|873|5773|HL9962|Android|5|Renan|Firmino|5/15/2018|Rio de Janeiro|3400|NaN|17000|
|874|5777|HL4379|Televisão|3|Caio|Ferreira|8/21/2018|Rio de Janeiro|2500|NaN|7500|
|875|5778|HL8851|Notebook|2|Matheus|Delgado|2/28/2018|Rio de Janeiro|3500|NaN|7000|
|876|5798|HL1918|iPhone|1|Mariana|Rotava|4/2/2018|Rio de Janeiro|5300|NaN|5300|
|877|5800|HL4379|Televisão|2|Alberto|Silveira|4/20/2018|Rio de Janeiro|2500|NaN|5000|
|878|5812|HL2714|Tablet|2|Adriana|Passos|5/9/2018|Rio de Janeiro|1600|NaN|3200|
|879|5827|HL9962|Android|5|Breno|Godoy|8/15/2018|Rio de Janeiro|3400|NaN|17000|
|880|5831|HL1918|iPhone|1|Luísa|Fonseca|5/15/2018|Rio de Janeiro|5300|NaN|5300|
|881|5838|HL8851|Notebook|3|Leandro|Rodrigues|7/19/2018|Rio de Janeiro|3500|NaN|10500|
|882|5867|HL8851|Notebook|3|Juliana|Guimarães|9/6/2018|Rio de Janeiro|3500|NaN|10500|
|883|5871|HL4379|Televisão|5|Matheus|Santos|2/25/2018|Rio de Janeiro|2500|NaN|12500|
|884|5880|HL1918|iPhone|4|Anna|Figueiredo|9/19/2018|Rio de Janeiro|5300|NaN|21200|
|885|5882|HL4379|Televisão|5|Henrique|Lencastre|11/26/2018|Rio de Janeiro|2500|NaN|12500|
|886|5889|HL1918|iPhone|2|Camila|Bastazini|12/28/2018|Rio de Janeiro|5300|NaN|10600|
|887|5890|HL1148|Câmera|3|Mariana|Freire|4/5/2018|Rio de Janeiro|2100|NaN|6300|
|888|5901|HL1918|iPhone|2|Daniel|Cardoso|10/15/2018|Rio de Janeiro|5300|NaN|10600|
|889|5916|HL2714|Tablet|4|Bruno|Mota|2/16/2018|Rio de Janeiro|1600|NaN|6400|
|890|5925|HL9962|Android|4|Matheus|Afonso|4/25/2018|Rio de Janeiro|3400|NaN|13600|
|891|5933|HL1918|iPhone|3|Henrique|Lencastre|3/17/2018|Rio de Janeiro|5300|NaN|15900|
|892|5945|HL1918|iPhone|2|Viviane|Cunha|12/8/2018|Rio de Janeiro|5300|NaN|10600|
|893|5965|HL1918|iPhone|5|Giulia|Lopes|10/31/2018|Rio de Janeiro|5300|NaN|26500|
|894|5971|HL4379|Televisão|4|Hygor|Essaber|7/19/2018|Rio de Janeiro|2500|NaN|10000|
|895|5977|HL8851|Notebook|2|Daniel|Monteiro|9/29/2018|Rio de Janeiro|3500|NaN|7000|
|896|5997|HL1148|Câmera|4|Matheus|Delgado|11/29/2018|Rio de Janeiro|2100|NaN|8400|
|897|5998|HL4379|Televisão|5|Caroline|Delgado|1/25/2018|Rio de Janeiro|2500|NaN|12500|
|898|6000|HL8851|Notebook|4|Alvaro|Kranz|10/11/2018|Rio de Janeiro|3500|NaN|14000|
|899|6007|HL9962|Android|2|Renan|Cunha|7/20/2018|Rio de Janeiro|3400|NaN|6800|
|900|6009|HL8851|Notebook|1|Jeferson|Sone|10/29/2018|Rio de Janeiro|3500|NaN|3500|
|901|6021|HL1148|Câmera|3|Paulo|Campos|2/5/2018|Rio de Janeiro|2100|NaN|6300|
|902|6024|HL9962|Android|5|Jessica|Cordovil|11/21/2018|Rio de Janeiro|3400|NaN|17000|
|903|6032|HL2714|Tablet|1|Ives|Pinheiro|10/29/2018|Rio de Janeiro|1600|NaN|1600|
|904|6035|HL2714|Tablet|2|Gabrielle|Silva|9/19/2018|Rio de Janeiro|1600|NaN|3200|
|905|6038|HL1918|iPhone|2|Lucas|Chagas|1/28/2018|Rio de Janeiro|5300|NaN|10600|
|906|6044|HL4379|Televisão|4|Gustavo|Azevedo|3/18/2018|Rio de Janeiro|2500|NaN|10000|
|907|6064|HL9962|Android|4|Breno|Britto|12/27/2018|Rio de Janeiro|3400|NaN|13600|
|908|6065|HL1918|iPhone|1|Larissa|Jesus|2/3/2018|Rio de Janeiro|5300|NaN|5300|
|909|6072|HL2714|Tablet|5|Isabelle|Gonçalves|6/18/2018|Rio de Janeiro|1600|NaN|8000|
|910|6073|HL7348|SmartWatch|5|Bruna|Londero|12/18/2018|Rio de Janeiro|1400|NaN|7000|
|911|6081|HL7348|SmartWatch|3|Mariane|Racy|7/31/2018|Rio de Janeiro|1400|NaN|4200|
|912|6110|HL1918|iPhone|2|Desirée|Heimlich|6/4/2018|Rio de Janeiro|5300|NaN|10600|
|913|6112|HL1918|iPhone|3|Pedro|Xavier|8/18/2018|Rio de Janeiro|5300|NaN|15900|
|914|6115|HL7348|SmartWatch|1|João|Pedrazza|2/26/2018|Rio de Janeiro|1400|NaN|1400|
|915|6124|HL7348|SmartWatch|2|Carlos|Azevedo|6/18/2018|Rio de Janeiro|1400|NaN|2800|
|916|6131|HL2714|Tablet|4|Thaís|Moura|6/10/2018|Rio de Janeiro|1600|NaN|6400|
|917|6133|HL1148|Câmera|1|Priscila|Carvalho|5/5/2018|Rio de Janeiro|2100|NaN|2100|
|918|6135|HL1918|iPhone|2|Marina|Cormack|11/5/2018|Rio de Janeiro|5300|NaN|10600|
|919|6153|HL8851|Notebook|2|Katharina|Barros|5/26/2018|Rio de Janeiro|3500|NaN|7000|
|920|6154|HL9962|Android|3|Thaís|Pereira|2/23/2018|Rio de Janeiro|3400|NaN|10200|
|921|6161|HL9962|Android|3|Raul|Silveira|3/22/2018|Rio de Janeiro|3400|NaN|10200|
|922|6163|HL1918|iPhone|5|Carolina|Rocha|4/20/2018|Rio de Janeiro|5300|NaN|26500|
|923|6165|HL7348|SmartWatch|2|Bruna|Brandao|3/10/2018|Rio de Janeiro|1400|NaN|2800|
|924|6166|HL1918|iPhone|2|Lázaro|Villanova|6/23/2018|Rio de Janeiro|5300|NaN|10600|
|925|6169|HL9962|Android|3|Raul|Silveira|2/7/2018|Rio de Janeiro|3400|NaN|10200|
|926|6179|HL8851|Notebook|1|Mariane|Ferreira|6/26/2018|Rio de Janeiro|3500|NaN|3500|
|927|6198|HL1918|iPhone|1|Rafael|Guimarães|4/23/2018|Rio de Janeiro|5300|NaN|5300|
|928|6208|HL7348|SmartWatch|2|Pedro|Oliveira|6/3/2018|Rio de Janeiro|1400|NaN|2800|
|929|6217|HL4379|Televisão|1|Felipe|Freitas|12/11/2018|Rio de Janeiro|2500|NaN|2500|
|930|6222|HL1918|iPhone|2|Thiago|Lima|11/18/2018|Rio de Janeiro|5300|NaN|10600|
|931|6229|HL4379|Televisão|5|Lucas|Reis|7/6/2018|Rio de Janeiro|2500|NaN|12500|
|932|6231|HL4379|Televisão|2|Juliana|Hollander|3/9/2018|Rio de Janeiro|2500|NaN|5000|
|933|6235|HL7348|SmartWatch|4|Deysiane|Bach|2/13/2018|Rio de Janeiro|1400|NaN|5600|
|934|6244|HL1148|Câmera|5|Renan|Nascimento|2/15/2018|Rio de Janeiro|2100|NaN|10500|
|935|6247|HL9962|Android|3|Victor|Magalhães|7/21/2018|Rio de Janeiro|3400|NaN|10200|
|936|6248|HL9962|Android|5|Raphael|Machado|3/8/2018|Rio de Janeiro|3400|NaN|17000|
|937|6273|HL1918|iPhone|2|Ana|Miura|11/29/2018|Rio de Janeiro|5300|NaN|10600|
|938|6278|HL1918|iPhone|3|Raíssa|Nimer|5/17/2018|Rio de Janeiro|5300|NaN|15900|
|939|6288|HL1148|Câmera|1|Bianca|Procaci|3/29/2018|Rio de Janeiro|2100|NaN|2100|
|940|6290|HL8851|Notebook|2|Milena|Pereira|10/16/2018|Rio de Janeiro|3500|NaN|7000|
|941|6292|HL2714|Tablet|2|Carolina|Brum|8/30/2018|Rio de Janeiro|1600|NaN|3200|
|942|6298|HL4379|Televisão|2|Norman|Jimbo|2/13/2018|Rio de Janeiro|2500|NaN|5000|
|943|6304|HL9962|Android|1|Thainá|Binello|7/17/2018|Rio de Janeiro|3400|NaN|3400|
|944|6308|HL4379|Televisão|1|Lucas|Machado|5/16/2018|Rio de Janeiro|2500|NaN|2500|
|945|6313|HL1918|iPhone|5|Ana|Felippe|6/10/2018|Rio de Janeiro|5300|NaN|26500|
|946|6319|HL4379|Televisão|3|Diego|Marchesi|3/29/2018|Rio de Janeiro|2500|NaN|7500|
|947|6322|HL2714|Tablet|4|Igor|Azevedo|4/7/2018|Rio de Janeiro|1600|NaN|6400|
|948|6323|HL7348|SmartWatch|1|Bruna|Rosa|2/22/2018|Rio de Janeiro|1400|NaN|1400|
|949|6327|HL1918|iPhone|3|José|Carvalho|11/3/2018|Rio de Janeiro|5300|NaN|15900|
|950|6330|HL1918|iPhone|2|Caio|Ferreira|6/14/2018|Rio de Janeiro|5300|NaN|10600|
|951|6332|HL1918|iPhone|2|Wilson|Vianna|5/5/2018|Rio de Janeiro|5300|NaN|10600|
|952|6333|HL8851|Notebook|1|Miguel|Carneiro|12/4/2018|Rio de Janeiro|3500|NaN|3500|
|953|6334|HL1918|iPhone|5|Ana|Fioretti|1/1/2018|Rio de Janeiro|5300|NaN|26500|
|954|6345|HL8851|Notebook|3|Victor|Magalhães|3/30/2018|Rio de Janeiro|3500|NaN|10500|
|955|6359|HL1918|iPhone|2|Mariana|Baptista|9/22/2018|Rio de Janeiro|5300|NaN|10600|
|956|6361|HL8851|Notebook|4|Isaac|Santos|8/3/2018|Rio de Janeiro|3500|NaN|14000|
|957|6364|HL1148|Câmera|1|Felipe|Jorge|9/20/2018|Rio de Janeiro|2100|NaN|2100|
|958|6369|HL1918|iPhone|1|Maria|Junior|6/1/2018|Rio de Janeiro|5300|NaN|5300|
|959|6374|HL1148|Câmera|2|Maria|Moita|9/25/2018|Rio de Janeiro|2100|NaN|4200|
|960|6382|HL1918|iPhone|4|Breno|Varella|6/22/2018|Rio de Janeiro|5300|NaN|21200|
|961|6398|HL8851|Notebook|3|Maria|Gasperi|9/11/2018|Rio de Janeiro|3500|NaN|10500|
|962|6400|HL1918|iPhone|2|Ana|Felippe|9/19/2018|Rio de Janeiro|5300|NaN|10600|
|963|6403|HL4379|Televisão|3|Alexandre|Dantas|9/10/2018|Rio de Janeiro|2500|NaN|7500|
|964|6406|HL8851|Notebook|3|Kimberly|Sad|8/17/2018|Rio de Janeiro|3500|NaN|10500|
|965|6408|HL9962|Android|3|Ana|Gomes|12/25/2018|Rio de Janeiro|3400|NaN|10200|
|966|6422|HL2714|Tablet|1|Gabriela|Mello|4/3/2018|Rio de Janeiro|1600|NaN|1600|
|967|6427|HL4379|Televisão|2|Thiago|Veiga|6/16/2018|Rio de Janeiro|2500|NaN|5000|
|968|6437|HL4379|Televisão|2|Carlos|Barbosa|12/22/2018|Rio de Janeiro|2500|NaN|5000|
|969|6452|HL4379|Televisão|1|Gabrielle|Costa|6/19/2018|Rio de Janeiro|2500|NaN|2500|
|970|6453|HL4379|Televisão|1|Carolina|Santos|8/30/2018|Rio de Janeiro|2500|NaN|2500|
|971|6459|HL1918|iPhone|4|Isabelle|Gonçalves|2/16/2018|Rio de Janeiro|5300|NaN|21200|
|972|6463|HL9962|Android|3|Gabrielle|Wanderley|5/9/2018|Rio de Janeiro|3400|NaN|10200|
|973|6465|HL1148|Câmera|2|Rodrigo|Silva|6/2/2018|Rio de Janeiro|2100|NaN|4200|
|974|6468|HL1918|iPhone|4|Felipe|Freitas|10/16/2018|Rio de Janeiro|5300|NaN|21200|
|975|6477|HL1918|iPhone|4|Deysiane|Medronho|2/20/2018|Rio de Janeiro|5300|NaN|21200|
|976|6481|HL1918|iPhone|1|Caroline|Pinto|12/4/2018|Rio de Janeiro|5300|NaN|5300|
|977|6484|HL1918|iPhone|5|Stephanie|Novak|7/4/2018|Rio de Janeiro|5300|NaN|26500|
|978|6490|HL1918|iPhone|1|Marcos|Nucci|6/27/2018|Rio de Janeiro|5300|NaN|5300|
|979|6505|HL1918|iPhone|3|Paloma|Sperandei|3/23/2018|Rio de Janeiro|5300|NaN|15900|
|980|6515|HL4379|Televisão|2|Caroline|Delgado|3/9/2018|Rio de Janeiro|2500|NaN|5000|
|981|6528|HL1918|iPhone|5|Pedro|Lyra|3/31/2018|Rio de Janeiro|5300|NaN|26500|
|982|6530|HL1918|iPhone|3|Matheus|Miranda|9/8/2018|Rio de Janeiro|5300|NaN|15900|
|983|6537|HL1148|Câmera|5|Bruno|Barcessat|6/27/2018|Rio de Janeiro|2100|NaN|10500|
|984|6539|HL1918|iPhone|1|Jéssica|Netto|2/21/2018|Rio de Janeiro|5300|NaN|5300|
|985|6543|HL1918|iPhone|3|João|Ribeiro|1/22/2018|Rio de Janeiro|5300|NaN|15900|
|986|6561|HL8851|Notebook|5|Wen|Santos|2/8/2018|Rio de Janeiro|3500|NaN|17500|
|987|6563|HL9962|Android|2|Maria|Gasperi|8/3/2018|Rio de Janeiro|3400|NaN|6800|
|988|6564|HL1918|iPhone|1|Victor|Gomes|9/5/2018|Rio de Janeiro|5300|NaN|5300|
|989|6573|HL1918|iPhone|2|Carlos|Araujo|7/28/2018|Rio de Janeiro|5300|NaN|10600|
|990|6575|HL4379|Televisão|2|Viviane|Souza|12/11/2018|Rio de Janeiro|2500|NaN|5000|
|991|6578|HL1918|iPhone|5|Bruna|Soares|3/23/2018|Rio de Janeiro|5300|NaN|26500|
|992|6596|HL9962|Android|1|Renan|Melo|11/28/2018|Rio de Janeiro|3400|NaN|3400|
|993|6603|HL7348|SmartWatch|3|William|Mendonça|11/25/2018|Rio de Janeiro|1400|NaN|4200|
|994|6605|HL9962|Android|5|Ana|Gonzaga|5/17/2018|Rio de Janeiro|3400|NaN|17000|
|995|6607|HL2714|Tablet|5|Elaine|Santos|11/2/2018|Rio de Janeiro|1600|NaN|8000|
|996|6611|HL4379|Televisão|4|Mateus|Polastri|9/6/2018|Rio de Janeiro|2500|NaN|10000|
|997|6616|HL8851|Notebook|5|Juliana|Hollander|7/24/2018|Rio de Janeiro|3500|NaN|17500|
|998|6619|HL9962|Android|2|Larissa|Jesus|2/15/2018|Rio de Janeiro|3400|NaN|6800|
|999|6620|HL2714|Tablet|5|Gabriel|Pereira|2/19/2018|Rio de Janeiro|1600|NaN|8000|
|1000|6621|HL1918|iPhone|2|Roberta|Nogueira|1/11/2018|Rio de Janeiro|5300|NaN|10600|
|1001|6625|HL1148|Câmera|2|Juliana|Souza|1/22/2018|Rio de Janeiro|2100|NaN|4200|
|1002|6626|HL2714|Tablet|2|Larissa|Vasconcellos|8/15/2018|Rio de Janeiro|1600|NaN|3200|
|1003|6635|HL1918|iPhone|4|Giuseppe|Bhering|11/15/2018|Rio de Janeiro|5300|NaN|21200|
|1004|6642|HL1918|iPhone|4|Renan|Firmino|4/4/2018|Rio de Janeiro|5300|NaN|21200|
|1005|6650|HL1918|iPhone|1|Matheus|Souza|7/4/2018|Rio de Janeiro|5300|NaN|5300|
|1006|6652|HL4379|Televisão|3|Lucas|Wanderley|4/8/2018|Rio de Janeiro|2500|NaN|7500|
|1007|6675|HL8851|Notebook|4|Dykson|Silva|7/7/2018|Rio de Janeiro|3500|NaN|14000|
|1008|6683|HL9962|Android|2|Thais|Rodrigues|5/6/2018|Rio de Janeiro|3400|NaN|6800|
|1009|6685|HL4379|Televisão|4|Julia|Teixeira|6/12/2018|Rio de Janeiro|2500|NaN|10000|
|1010|6695|HL7348|SmartWatch|3|Felipe|Mello|3/7/2018|Rio de Janeiro|1400|NaN|4200|
|1011|6709|HL8851|Notebook|3|Lucas|Destri|1/23/2018|Rio de Janeiro|3500|NaN|10500|
|1012|6715|HL4379|Televisão|5|Isabella|Scalabrin|2/20/2018|Rio de Janeiro|2500|NaN|12500|
|1013|6735|HL1148|Câmera|3|Ives|Teixeira|4/21/2018|Rio de Janeiro|2100|NaN|6300|
|1014|6746|HL1148|Câmera|5|Breno|Caputo|12/6/2018|Rio de Janeiro|2100|NaN|10500|
|1015|6751|HL8851|Notebook|2|Ulisses|Quinto|7/18/2018|Rio de Janeiro|3500|NaN|7000|
|1016|6753|HL8851|Notebook|1|Nina|Magalhães|7/10/2018|Rio de Janeiro|3500|NaN|3500|
|1017|6757|HL1918|iPhone|2|Julia|Figueiredo|3/31/2018|Rio de Janeiro|5300|NaN|10600|
|1018|6762|HL1918|iPhone|2|Aline|Mello|2/23/2018|Rio de Janeiro|5300|NaN|10600|
|1019|6811|HL7348|SmartWatch|4|João|Castilho|1/27/2018|Rio de Janeiro|1400|NaN|5600|
|1020|6819|HL8851|Notebook|2|Lucas|Reis|1/7/2018|Rio de Janeiro|3500|NaN|7000|
|1021|6835|HL1918|iPhone|2|Pedro|Xavier|8/30/2018|Rio de Janeiro|5300|NaN|10600|
|1022|6840|HL7348|SmartWatch|3|João|Menezes|6/19/2018|Rio de Janeiro|1400|NaN|4200|
|1023|6843|HL7348|SmartWatch|3|José|Fonseca|2/20/2018|Rio de Janeiro|1400|NaN|4200|
|1024|6845|HL1918|iPhone|5|Caio|Silva|11/24/2018|Rio de Janeiro|5300|NaN|26500|
|1025|6847|HL2714|Tablet|1|Diego|Rodrigues|6/6/2018|Rio de Janeiro|1600|NaN|1600|
|1026|6849|HL2714|Tablet|3|Juliana|Guimarães|5/12/2018|Rio de Janeiro|1600|NaN|4800|
|1027|6855|HL4379|Televisão|5|Matheus|Miranda|2/13/2018|Rio de Janeiro|2500|NaN|12500|
|1028|6859|HL2714|Tablet|2|Maria|Moita|11/5/2018|Rio de Janeiro|1600|NaN|3200|
|1029|6863|HL4379|Televisão|2|Beatriz|Santos|11/29/2018|Rio de Janeiro|2500|NaN|5000|
|1030|6871|HL9962|Android|5|Camilla|Cardeman|11/20/2018|Rio de Janeiro|3400|NaN|17000|
|1031|6872|HL9962|Android|1|Guilherme|Castilho|2/17/2018|Rio de Janeiro|3400|NaN|3400|
|1032|6873|HL1918|iPhone|5|Jeferson|Costa|2/14/2018|Rio de Janeiro|5300|NaN|26500|
|1033|6877|HL2714|Tablet|2|Gabrielle|Silva|10/26/2018|Rio de Janeiro|1600|NaN|3200|
|1034|6932|HL8851|Notebook|4|Daniel|Felippe|10/4/2018|Rio de Janeiro|3500|NaN|14000|
|1035|6942|HL4379|Televisão|5|Lucas|Freitas|11/11/2018|Rio de Janeiro|2500|NaN|12500|
|1036|6947|HL8851|Notebook|2|Myllena|Carneiro|9/10/2018|Rio de Janeiro|3500|NaN|7000|
|1037|6950|HL1148|Câmera|3|Juliana|Goes|4/15/2018|Rio de Janeiro|2100|NaN|6300|
|1038|6956|HL9962|Android|2|Guilherme|Merotto|8/15/2018|Rio de Janeiro|3400|NaN|6800|
|1039|6964|HL7348|SmartWatch|5|Sylvio|Bernhardt|2/21/2018|Rio de Janeiro|1400|NaN|7000|
|1040|6970|HL9962|Android|5|Carlos|Galvão|9/17/2018|Rio de Janeiro|3400|NaN|17000|
|1041|6990|HL4379|Televisão|5|Guilherme|Seixas|7/23/2018|Rio de Janeiro|2500|NaN|12500|
|1042|6992|HL1148|Câmera|2|Itai|Puntel|12/30/2018|Rio de Janeiro|2100|NaN|4200|
|1043|7012|HL1918|iPhone|1|Ramon|Araujo|9/11/2018|Rio de Janeiro|5300|NaN|5300|
|1044|7013|HL1918|iPhone|3|João|Capitulo|10/10/2018|Rio de Janeiro|5300|NaN|15900|
|1045|7014|HL1918|iPhone|1|Pedro|Costa|11/30/2018|Rio de Janeiro|5300|NaN|5300|
|1046|7016|HL9962|Android|1|Isabelle|Firmino|3/6/2018|Rio de Janeiro|3400|NaN|3400|
|1047|7036|HL1918|iPhone|1|Igor|Azevedo|5/8/2018|Rio de Janeiro|5300|NaN|5300|
|1048|7040|HL9962|Android|4|Pedro|Jorge|1/24/2018|Rio de Janeiro|3400|NaN|13600|
|1049|7044|HL9962|Android|1|Myllena|Carneiro|12/30/2018|Rio de Janeiro|3400|NaN|3400|
|1050|7059|HL4379|Televisão|2|Gabrielle|Costa|10/11/2018|Rio de Janeiro|2500|NaN|5000|
|1051|7073|HL2714|Tablet|3|Caroline|Delgado|12/31/2018|Rio de Janeiro|1600|NaN|4800|
|1052|7076|HL2714|Tablet|4|Bruno|Barcessat|3/31/2018|Rio de Janeiro|1600|NaN|6400|
|1053|7078|HL1148|Câmera|2|Lara|Moreira|5/18/2018|Rio de Janeiro|2100|NaN|4200|
|1054|7091|HL8851|Notebook|4|Raissa|Maia|6/30/2018|Rio de Janeiro|3500|NaN|14000|
|1055|7099|HL1918|iPhone|1|Wilson|Brandão|3/20/2018|Rio de Janeiro|5300|NaN|5300|
|1056|7106|HL9962|Android|1|Matheus|Figueiredo|10/24/2018|Rio de Janeiro|3400|NaN|3400|
|1057|7110|HL4379|Televisão|1|Guilherme|Castilho|1/25/2018|Rio de Janeiro|2500|NaN|2500|
|1058|7113|HL9962|Android|4|Rogério|Gentile|10/21/2018|Rio de Janeiro|3400|NaN|13600|
|1059|7120|HL1918|iPhone|2|Débora|Lopes|3/15/2018|Rio de Janeiro|5300|NaN|10600|
|1060|7130|HL1148|Câmera|3|Carlos|Mesquita|12/6/2018|Rio de Janeiro|2100|NaN|6300|
|1061|7134|HL4379|Televisão|3|Brenno|Santos|11/16/2018|Rio de Janeiro|2500|NaN|7500|
|1062|7138|HL1148|Câmera|2|Patrícia|Amaral|9/8/2018|Rio de Janeiro|2100|NaN|4200|
|1063|7152|HL1918|iPhone|1|Jéssica|Teixeira|4/28/2018|Rio de Janeiro|5300|NaN|5300|
|1064|7160|HL7348|SmartWatch|4|Beatriz|Cavalcanti|12/26/2018|Rio de Janeiro|1400|NaN|5600|
|1065|7162|HL1918|iPhone|3|Amanda|Roberto|1/8/2018|Rio de Janeiro|5300|NaN|15900|
|1066|7164|HL4379|Televisão|1|Cícero|Ramos|1/4/2018|Rio de Janeiro|2500|NaN|2500|
|1067|7175|HL1918|iPhone|1|Felipe|Freitas|7/3/2018|Rio de Janeiro|5300|NaN|5300|
|1068|7181|HL4379|Televisão|3|João|Júnior|2/21/2018|Rio de Janeiro|2500|NaN|7500|
|1069|7197|HL1918|iPhone|3|Rodrigo|Bruno|8/26/2018|Rio de Janeiro|5300|NaN|15900|
|1070|7210|HL1918|iPhone|1|Paola|Abreu|2/19/2018|Rio de Janeiro|5300|NaN|5300|
|1071|7212|HL4379|Televisão|2|Anna|Silva|7/2/2018|Rio de Janeiro|2500|NaN|5000|
|1072|7214|HL8851|Notebook|3|Lucas|Almeida|3/6/2018|Rio de Janeiro|3500|NaN|10500|
|1073|7217|HL7348|SmartWatch|3|Bruna|Rosa|1/24/2018|Rio de Janeiro|1400|NaN|4200|
|1074|7221|HL8851|Notebook|4|Pedro|Bitencourt|3/14/2018|Rio de Janeiro|3500|NaN|14000|
|1075|7226|HL1918|iPhone|3|Matheus|Miranda|12/11/2018|Rio de Janeiro|5300|NaN|15900|
|1076|7254|HL7348|SmartWatch|2|Lorena|Carvalho|11/20/2018|Rio de Janeiro|1400|NaN|2800|
|1077|7265|HL1148|Câmera|3|Lucas|Baptista|7/15/2018|Rio de Janeiro|2100|NaN|6300|
|1078|7280|HL1918|iPhone|3|Bárbara|Cavalcante|4/3/2018|Rio de Janeiro|5300|NaN|15900|
|1079|7288|HL4379|Televisão|2|Fillipe|Almeida|5/22/2018|Rio de Janeiro|2500|NaN|5000|
|1080|7294|HL7348|SmartWatch|5|Carlos|Araujo|4/25/2018|Rio de Janeiro|1400|NaN|7000|
|1081|7314|HL8851|Notebook|3|Daniel|Felippe|11/15/2018|Rio de Janeiro|3500|NaN|10500|
|1082|7317|HL7348|SmartWatch|1|Lucas|Rodrigues|8/29/2018|Rio de Janeiro|1400|NaN|1400|
|1083|7346|HL4379|Televisão|2|Guido|Monteiro|10/10/2018|Rio de Janeiro|2500|NaN|5000|
|1084|7350|HL1918|iPhone|2|João|Pedrazza|3/19/2018|Rio de Janeiro|5300|NaN|10600|
|1085|7351|HL4379|Televisão|5|Gabrielle|Figueiredo|1/10/2018|Rio de Janeiro|2500|NaN|12500|
|1086|7365|HL1918|iPhone|4|Lorena|Carvalho|8/31/2018|Rio de Janeiro|5300|NaN|21200|
|1087|7369|HL9962|Android|5|Carolina|Abrahão|1/27/2018|Rio de Janeiro|3400|NaN|17000|
|1088|7371|HL7348|SmartWatch|2|Arthur|Rocha|3/16/2018|Rio de Janeiro|1400|NaN|2800|
|1089|7373|HL1918|iPhone|1|David|Campelo|2/20/2018|Rio de Janeiro|5300|NaN|5300|
|1090|7378|HL9962|Android|4|Felipe|Cavalcanti|7/4/2018|Rio de Janeiro|3400|NaN|13600|
|1091|7384|HL1918|iPhone|1|Yasser|Calbucci|11/29/2018|Rio de Janeiro|5300|NaN|5300|
|1092|7385|HL4379|Televisão|2|Carlos|Portela|3/16/2018|Rio de Janeiro|2500|NaN|5000|
|1093|7388|HL2714|Tablet|2|Norman|Jimbo|10/21/2018|Rio de Janeiro|1600|NaN|3200|
|1094|7389|HL1148|Câmera|1|Rafael|Guimarães|3/5/2018|Rio de Janeiro|2100|NaN|2100|
|1095|7396|HL1918|iPhone|5|Stefan|Nunes|1/21/2018|Rio de Janeiro|5300|NaN|26500|
|1096|7399|HL1918|iPhone|1|Tainah|Nogueira|11/14/2018|Rio de Janeiro|5300|NaN|5300|
|1097|7407|HL4379|Televisão|4|Morgana|Correa|4/4/2018|Rio de Janeiro|2500|NaN|10000|
|1098|7410|HL7348|SmartWatch|5|Roger|Rosa|1/20/2018|Rio de Janeiro|1400|NaN|7000|
|1099|7433|HL4379|Televisão|1|Adriano|Silva|6/15/2018|Rio de Janeiro|2500|NaN|2500|
|1100|7456|HL4379|Televisão|5|Lucas|Villanova|1/30/2018|Rio de Janeiro|2500|NaN|12500|
|1101|7470|HL4379|Televisão|5|Laura|Araujo|6/16/2018|Rio de Janeiro|2500|NaN|12500|
|1102|7479|HL4379|Televisão|1|Caio|Ferreira|7/14/2018|Rio de Janeiro|2500|NaN|2500|
|1103|7480|HL2714|Tablet|4|Henrique|Silva|8/26/2018|Rio de Janeiro|1600|NaN|6400|
|1104|7486|HL4379|Televisão|4|Ylana|Teraoka|12/1/2018|Rio de Janeiro|2500|NaN|10000|
|1105|7493|HL9962|Android|4|Matheus|Miranda|7/22/2018|Rio de Janeiro|3400|NaN|13600|
|1106|7500|HL1148|Câmera|4|Milena|Alcoforado|2/21/2018|Rio de Janeiro|2100|NaN|8400|
|1107|7504|HL4379|Televisão|1|Lucas|Freitas|10/15/2018|Rio de Janeiro|2500|NaN|2500|
|1108|7510|HL8851|Notebook|5|Carolina|Siqueira|11/24/2018|Rio de Janeiro|3500|NaN|17500|
|1109|7517|HL1148|Câmera|3|João|Costa|8/25/2018|Rio de Janeiro|2100|NaN|6300|
|1110|7519|HL1918|iPhone|4|Gustavo|Azevedo|2/22/2018|Rio de Janeiro|5300|NaN|21200|
|1111|7532|HL1918|iPhone|1|Thiago|Miura|8/30/2018|Rio de Janeiro|5300|NaN|5300|
|1112|7540|HL4379|Televisão|5|Rogério|Pereira|2/16/2018|Rio de Janeiro|2500|NaN|12500|
|1113|7542|HL7348|SmartWatch|4|Julie|Ferreira|7/14/2018|Rio de Janeiro|1400|NaN|5600|
|1114|7549|HL1918|iPhone|5|Lucas|Lima|8/30/2018|Rio de Janeiro|5300|NaN|26500|
|1115|7565|HL1918|iPhone|4|Jonas|Gomes|10/21/2018|Rio de Janeiro|5300|NaN|21200|
|1116|7566|HL4379|Televisão|4|Rodrigo|Silva|7/5/2018|Rio de Janeiro|2500|NaN|10000|
|1117|7567|HL4379|Televisão|3|Rafael|Ramos|12/2/2018|Rio de Janeiro|2500|NaN|7500|
|1118|7578|HL4379|Televisão|3|Henrique|Villanova|1/21/2018|Rio de Janeiro|2500|NaN|7500|
|1119|7589|HL1918|iPhone|2|Raissa|Sales|3/22/2018|Rio de Janeiro|5300|NaN|10600|
|1120|7595|HL4379|Televisão|3|Pedro|Ayres|1/30/2018|Rio de Janeiro|2500|NaN|7500|
|1121|7617|HL1148|Câmera|2|Luiza|Cavalcanti|12/28/2018|Rio de Janeiro|2100|NaN|4200|
|1122|7619|HL2714|Tablet|2|Julia|Figueiredo|4/1/2018|Rio de Janeiro|1600|NaN|3200|
|1123|7621|HL1918|iPhone|4|Mateus|Polastri|8/9/2018|Rio de Janeiro|5300|NaN|21200|
|1124|7624|HL8851|Notebook|4|Jeferson|Costa|3/23/2018|Rio de Janeiro|3500|NaN|14000|
|1125|7626|HL1918|iPhone|2|Luã|Sá|2/5/2018|Rio de Janeiro|5300|NaN|10600|
|1126|7632|HL1918|iPhone|1|Daniel|Monteiro|6/17/2018|Rio de Janeiro|5300|NaN|5300|
|1127|7644|HL1148|Câmera|2|David|Assumpção|8/23/2018|Rio de Janeiro|2100|NaN|4200|
|1128|7647|HL1918|iPhone|2|Natalia|Andrade|10/5/2018|Rio de Janeiro|5300|NaN|10600|
|1129|7653|HL4379|Televisão|2|Gabrielle|Porto|3/18/2018|Rio de Janeiro|2500|NaN|5000|
|1130|7655|HL4379|Televisão|4|Eduardo|Lopes|1/9/2018|Rio de Janeiro|2500|NaN|10000|
|1131|7660|HL1148|Câmera|1|Barbara|Procaci|6/4/2018|Rio de Janeiro|2100|NaN|2100|
|1132|7661|HL1918|iPhone|4|Pedro|Ronfini|12/29/2018|Rio de Janeiro|5300|NaN|21200|
|1133|7665|HL8851|Notebook|1|Ana|Fioretti|10/11/2018|Rio de Janeiro|3500|NaN|3500|
|1134|7670|HL1148|Câmera|4|Brenno|Miranda|11/29/2018|Rio de Janeiro|2100|NaN|8400|
|1135|7677|HL1918|iPhone|2|Diego|Mello|12/6/2018|Rio de Janeiro|5300|NaN|10600|
|1136|7678|HL1918|iPhone|3|Roberta|Pimenta|12/8/2018|Rio de Janeiro|5300|NaN|15900|
|1137|7686|HL1148|Câmera|4|Carolina|Abrahão|6/26/2018|Rio de Janeiro|2100|NaN|8400|
|1138|7694|HL1918|iPhone|2|Gabriel|Silva|7/21/2018|Rio de Janeiro|5300|NaN|10600|
|1139|7697|HL1918|iPhone|5|Cláudio|Aragão|9/3/2018|Rio de Janeiro|5300|NaN|26500|
|1140|7703|HL4379|Televisão|5|Anna|Silva|3/31/2018|Rio de Janeiro|2500|NaN|12500|
|1141|7705|HL4379|Televisão|5|Caio|Vianna|9/11/2018|Rio de Janeiro|2500|NaN|12500|
|1142|7713|HL1918|iPhone|4|Gabriela|Mello|4/12/2018|Rio de Janeiro|5300|NaN|21200|
|1143|7718|HL9962|Android|5|Luíza|Melo|11/7/2018|Rio de Janeiro|3400|NaN|17000|
|1144|7719|HL1918|iPhone|1|Guilherme|Lima|9/25/2018|Rio de Janeiro|5300|NaN|5300|
|1145|7720|HL9962|Android|4|Carlos|Assis|8/22/2018|Rio de Janeiro|3400|NaN|13600|
|1146|7762|HL1918|iPhone|4|Pedro|Ferrari|3/19/2018|Rio de Janeiro|5300|NaN|21200|
|1147|7766|HL9962|Android|4|Marina|Marins|6/26/2018|Rio de Janeiro|3400|NaN|13600|
|1148|7796|HL1918|iPhone|4|Milena|Alcoforado|3/27/2018|Rio de Janeiro|5300|NaN|21200|
|1149|7820|HL2714|Tablet|3|Daniel|Valente|2/8/2018|Rio de Janeiro|1600|NaN|4800|
|1150|7825|HL1918|iPhone|1|Thales|Gouvêa|5/20/2018|Rio de Janeiro|5300|NaN|5300|
|1151|7828|HL2714|Tablet|4|Raissa|Maia|2/22/2018|Rio de Janeiro|1600|NaN|6400|
|1152|7829|HL1148|Câmera|4|Thales|Santos|8/24/2018|Rio de Janeiro|2100|NaN|8400|
|1153|7831|HL1918|iPhone|5|Pedro|Ferrari|6/14/2018|Rio de Janeiro|5300|NaN|26500|
|1154|7839|HL1148|Câmera|3|Bárbara|Cavalcante|1/29/2018|Rio de Janeiro|2100|NaN|6300|
|1155|7847|HL7348|SmartWatch|1|Júlia|Almeida|10/28/2018|Rio de Janeiro|1400|NaN|1400|
|1156|7850|HL1148|Câmera|5|Gabriel|Puntel|3/27/2018|Rio de Janeiro|2100|NaN|10500|
|1157|7860|HL1918|iPhone|2|Debora|Silva|5/4/2018|Rio de Janeiro|5300|NaN|10600|
|1158|7863|HL4379|Televisão|2|Marcela|Johnson|4/23/2018|Rio de Janeiro|2500|NaN|5000|
|1159|7880|HL4379|Televisão|2|Raíza|Lopes|9/29/2018|Rio de Janeiro|2500|NaN|5000|
|1160|7881|HL1918|iPhone|2|Victor|Gomes|6/30/2018|Rio de Janeiro|5300|NaN|10600|
|1161|7889|HL1918|iPhone|1|Helena|Chafin|4/5/2018|Rio de Janeiro|5300|NaN|5300|
|1162|7892|HL7348|SmartWatch|2|Isaac|Santos|4/13/2018|Rio de Janeiro|1400|NaN|2800|
|1163|7904|HL1918|iPhone|4|Alberto|Silveira|2/5/2018|Rio de Janeiro|5300|NaN|21200|
|1164|7932|HL1918|iPhone|2|Alexandre|Dantas|12/9/2018|Rio de Janeiro|5300|NaN|10600|
|1165|7933|HL1918|iPhone|4|Gabriella|Lopes|8/23/2018|Rio de Janeiro|5300|NaN|21200|
|1166|7937|HL2714|Tablet|3|Victor|Franco|11/4/2018|Rio de Janeiro|1600|NaN|4800|
|1167|7943|HL1148|Câmera|3|Henrique|Silva|3/15/2018|Rio de Janeiro|2100|NaN|6300|
|1168|7952|HL2714|Tablet|3|Anderson|Cavalcanti|6/8/2018|Rio de Janeiro|1600|NaN|4800|
|1169|7956|HL2714|Tablet|4|Mateus|Duque|11/16/2018|Rio de Janeiro|1600|NaN|6400|
|1170|7959|HL1148|Câmera|3|Fabio|Ramos|10/8/2018|Rio de Janeiro|2100|NaN|6300|
|1171|7960|HL9962|Android|3|Bruno|Salomão|5/21/2018|Rio de Janeiro|3400|NaN|10200|
|1172|7962|HL7348|SmartWatch|3|Brenno|Santos|6/1/2018|Rio de Janeiro|1400|NaN|4200|
|1173|7989|HL1148|Câmera|3|Felipe|Cavalcanti|6/25/2018|Rio de Janeiro|2100|NaN|6300|
|1174|7993|HL4379|Televisão|1|Yasmim|Bittencourt|1/11/2018|Rio de Janeiro|2500|NaN|2500|
|1175|7995|HL4379|Televisão|5|Patrícia|Amaral|12/31/2018|Rio de Janeiro|2500|NaN|12500|
|1176|8004|HL9962|Android|3|Arthur|Souza|6/15/2018|Rio de Janeiro|3400|NaN|10200|
|1177|8032|HL1918|iPhone|5|João|Araujo|9/8/2018|Rio de Janeiro|5300|NaN|26500|
|1178|8040|HL1918|iPhone|1|Raíssa|Nimer|11/18/2018|Rio de Janeiro|5300|NaN|5300|
|1179|8047|HL4379|Televisão|5|Jeferson|Sone|2/5/2018|Rio de Janeiro|2500|NaN|12500|
|1180|8052|HL1918|iPhone|1|Renan|Nascimento|1/7/2018|Rio de Janeiro|5300|NaN|5300|
|1181|8055|HL8851|Notebook|5|Jonatas|Essaber|5/8/2018|Rio de Janeiro|3500|NaN|17500|
|1182|8057|HL1918|iPhone|3|Pedro|Pereira|7/15/2018|Rio de Janeiro|5300|NaN|15900|
|1183|8063|HL7348|SmartWatch|5|Gabriel|Puntel|11/12/2018|Rio de Janeiro|1400|NaN|7000|
|1184|8065|HL9962|Android|4|Anna|Figueiredo|4/17/2018|Rio de Janeiro|3400|NaN|13600|
|1185|8073|HL1918|iPhone|5|Gabrielle|Costa|2/22/2018|Rio de Janeiro|5300|NaN|26500|
|1186|8092|HL4379|Televisão|4|Thales|Fanara|11/18/2018|Rio de Janeiro|2500|NaN|10000|
|1187|8119|HL9962|Android|2|Mayara|Soares|12/24/2018|Rio de Janeiro|3400|NaN|6800|
|1188|8121|HL2714|Tablet|4|Izabel|Miura|6/27/2018|Rio de Janeiro|1600|NaN|6400|
|1189|8126|HL8851|Notebook|1|Fabio|Sepúlveda|12/16/2018|Rio de Janeiro|3500|NaN|3500|
|1190|8127|HL9962|Android|1|Lucas|Rocha|9/6/2018|Rio de Janeiro|3400|NaN|3400|
|1191|8130|HL8851|Notebook|5|Letícia|Leal|12/27/2018|Rio de Janeiro|3500|NaN|17500|
|1192|8146|HL7348|SmartWatch|3|Thiago|Veloso|7/11/2018|Rio de Janeiro|1400|NaN|4200|
|1193|8148|HL1148|Câmera|2|Katharina|Barros|6/22/2018|Rio de Janeiro|2100|NaN|4200|
|1194|8153|HL7348|SmartWatch|5|Carlos|Galvão|12/22/2018|Rio de Janeiro|1400|NaN|7000|
|1195|8154|HL8851|Notebook|1|Ana|Júnior|1/18/2018|Rio de Janeiro|3500|NaN|3500|
|1196|8167|HL2714|Tablet|3|Carolina|Carneiro|4/1/2018|Rio de Janeiro|1600|NaN|4800|
|1197|8170|HL1918|iPhone|4|Luiz|Almeida|11/20/2018|Rio de Janeiro|5300|NaN|21200|
|1198|8184|HL8851|Notebook|4|Rafaela|Gonçalves|4/1/2018|Rio de Janeiro|3500|NaN|14000|
|1199|8188|HL9962|Android|5|Mariana|Rotava|11/7/2018|Rio de Janeiro|3400|NaN|17000|
|1200|8196|HL1918|iPhone|2|Ana|Gomes|8/19/2018|Rio de Janeiro|5300|NaN|10600|
|1201|8202|HL1918|iPhone|5|Jônatas|Tanaka|12/20/2018|Rio de Janeiro|5300|NaN|26500|
|1202|8204|HL4379|Televisão|4|Bernardo|Soares|2/20/2018|Rio de Janeiro|2500|NaN|10000|
|1203|8206|HL7348|SmartWatch|1|Itai|Puntel|8/10/2018|Rio de Janeiro|1400|NaN|1400|
|1204|8212|HL4379|Televisão|3|Matheus|Ramos|9/24/2018|Rio de Janeiro|2500|NaN|7500|
|1205|8216|HL4379|Televisão|3|Matheus|Delgado|8/19/2018|Rio de Janeiro|2500|NaN|7500|
|1206|8232|HL9962|Android|4|Ana|Júnior|6/10/2018|Rio de Janeiro|3400|NaN|13600|
|1207|8243|HL2714|Tablet|1|Gustavo|Guimarães|10/4/2018|Rio de Janeiro|1600|NaN|1600|
|1208|8244|HL2714|Tablet|3|Luana|Santana|10/23/2018|Rio de Janeiro|1600|NaN|4800|
|1209|8247|HL7348|SmartWatch|1|Katharina|Barros|6/17/2018|Rio de Janeiro|1400|NaN|1400|
|1210|8260|HL7348|SmartWatch|3|Milena|Alcoforado|9/6/2018|Rio de Janeiro|1400|NaN|4200|
|1211|8261|HL2714|Tablet|2|Bianca|Ferezin|1/25/2018|Rio de Janeiro|1600|NaN|3200|
|1212|8264|HL1918|iPhone|2|Luísa|Fonseca|1/8/2018|Rio de Janeiro|5300|NaN|10600|
|1213|8278|HL4379|Televisão|1|Carolina|Siqueira|6/10/2018|Rio de Janeiro|2500|NaN|2500|
|1214|8285|HL8851|Notebook|5|Bernardo|Nauenberg|10/9/2018|Rio de Janeiro|3500|NaN|17500|
|1215|8291|HL4379|Televisão|5|Natali|Rangel|4/6/2018|Rio de Janeiro|2500|NaN|12500|
|1216|8293|HL9962|Android|3|Alberto|Silveira|6/17/2018|Rio de Janeiro|3400|NaN|10200|
|1217|8302|HL1918|iPhone|3|Victoria|Tavares|8/24/2018|Rio de Janeiro|5300|NaN|15900|
|1218|8308|HL8851|Notebook|1|Fabio|Boccaletti|8/16/2018|Rio de Janeiro|3500|NaN|3500|
|1219|8335|HL8851|Notebook|3|Matheus|Silva|10/28/2018|Rio de Janeiro|3500|NaN|10500|
|1220|8336|HL9962|Android|4|Juan|Barbosa|1/12/2018|Rio de Janeiro|3400|NaN|13600|
|1221|8352|HL1148|Câmera|5|Marcos|Nucci|8/4/2018|Rio de Janeiro|2100|NaN|10500|
|1222|8358|HL1148|Câmera|4|Diego|Mello|5/23/2018|Rio de Janeiro|2100|NaN|8400|
|1223|8365|HL4379|Televisão|3|Carlos|Galvão|2/17/2018|Rio de Janeiro|2500|NaN|7500|
|1224|8368|HL1918|iPhone|2|Victor|Corrêa|8/6/2018|Rio de Janeiro|5300|NaN|10600|
|1225|8374|HL2714|Tablet|3|Juliana|Barreira|11/19/2018|Rio de Janeiro|1600|NaN|4800|
|1226|8387|HL1918|iPhone|2|Rachel|Silva|3/1/2018|Rio de Janeiro|5300|NaN|10600|
|1227|8404|HL1918|iPhone|5|Thiago|Veiga|11/6/2018|Rio de Janeiro|5300|NaN|26500|
|1228|8406|HL1918|iPhone|2|Milena|Alcoforado|9/4/2018|Rio de Janeiro|5300|NaN|10600|
|1229|8410|HL1918|iPhone|2|Mariane|Ferreira|1/3/2018|Rio de Janeiro|5300|NaN|10600|
|1230|8418|HL2714|Tablet|2|Juliana|Correa|8/31/2018|Rio de Janeiro|1600|NaN|3200|
|1231|8419|HL1918|iPhone|4|Luiz|Freire|1/11/2018|Rio de Janeiro|5300|NaN|21200|
|1232|8436|HL8851|Notebook|3|Gabrielle|Porto|8/18/2018|Rio de Janeiro|3500|NaN|10500|
|1233|8437|HL1148|Câmera|1|Diego|Barros|9/10/2018|Rio de Janeiro|2100|NaN|2100|
|1234|8440|HL4379|Televisão|2|Marina|Aragão|2/8/2018|Rio de Janeiro|2500|NaN|5000|
|1235|8446|HL8851|Notebook|3|Priscila|Garcia|4/9/2018|Rio de Janeiro|3500|NaN|10500|
|1236|8450|HL4379|Televisão|5|Rilson|Dias|12/22/2018|Rio de Janeiro|2500|NaN|12500|
|1237|8462|HL1918|iPhone|5|Julia|Leite|9/8/2018|Rio de Janeiro|5300|NaN|26500|
|1238|8465|HL4379|Televisão|4|Leandro|Melo|1/27/2018|Rio de Janeiro|2500|NaN|10000|
|1239|8482|HL2714|Tablet|5|Renan|Firmino|4/11/2018|Rio de Janeiro|1600|NaN|8000|
|1240|8488|HL2714|Tablet|5|Nina|Magalhães|5/7/2018|Rio de Janeiro|1600|NaN|8000|
|1241|8490|HL1918|iPhone|3|Bruno|Mota|4/14/2018|Rio de Janeiro|5300|NaN|15900|
|1242|8491|HL7348|SmartWatch|1|Diego|Rodrigues|7/17/2018|Rio de Janeiro|1400|NaN|1400|
|1243|8494|HL1148|Câmera|1|Gabrielle|Costa|7/26/2018|Rio de Janeiro|2100|NaN|2100|
|1244|8504|HL9962|Android|1|Marcela|Medeiros|3/26/2018|Rio de Janeiro|3400|NaN|3400|
|1245|8505|HL8851|Notebook|1|Pedro|Bitencourt|10/5/2018|Rio de Janeiro|3500|NaN|3500|
|1246|8507|HL1148|Câmera|4|Victor|Soares|12/7/2018|Rio de Janeiro|2100|NaN|8400|
|1247|8509|HL4379|Televisão|3|Jessica|Cordovil|10/24/2018|Rio de Janeiro|2500|NaN|7500|
|1248|8517|HL8851|Notebook|1|Thiago|Veiga|3/10/2018|Rio de Janeiro|3500|NaN|3500|
|1249|8531|HL1148|Câmera|4|Thiago|Veiga|8/22/2018|Rio de Janeiro|2100|NaN|8400|
|1250|8532|HL8851|Notebook|2|Livia|Corrêa|4/7/2018|Rio de Janeiro|3500|NaN|7000|
|1251|8544|HL4379|Televisão|3|Clara|Bruno|10/27/2018|Rio de Janeiro|2500|NaN|7500|
|1252|8545|HL8851|Notebook|3|Luana|Santos|10/19/2018|Rio de Janeiro|3500|NaN|10500|
|1253|8550|HL2714|Tablet|1|Maria|Mello|1/3/2018|Rio de Janeiro|1600|NaN|1600|
|1254|8556|HL8851|Notebook|2|Glenda|Santos|2/4/2018|Rio de Janeiro|3500|NaN|7000|
|1255|8558|HL1918|iPhone|1|Guilherme|Merotto|2/15/2018|Rio de Janeiro|5300|NaN|5300|
|1256|8574|HL4379|Televisão|3|Bruno|Temporal|12/28/2018|Rio de Janeiro|2500|NaN|7500|
|1257|8575|HL7348|SmartWatch|1|Andre|Sampaio|2/27/2018|Rio de Janeiro|1400|NaN|1400|
|1258|8582|HL7348|SmartWatch|2|Carolina|Motta|7/29/2018|Rio de Janeiro|1400|NaN|2800|
|1259|8591|HL8851|Notebook|2|Carlos|Azevedo|5/24/2018|Rio de Janeiro|3500|NaN|7000|
|1260|8598|HL4379|Televisão|3|Wilson|Brandão|2/21/2018|Rio de Janeiro|2500|NaN|7500|
|1261|8608|HL9962|Android|4|Rafael|Portela|8/30/2018|Rio de Janeiro|3400|NaN|13600|
|1262|8617|HL4379|Televisão|3|Gustavo|Erthal|6/3/2018|Rio de Janeiro|2500|NaN|7500|
|1263|8622|HL4379|Televisão|1|Ulisses|Arruda|9/25/2018|Rio de Janeiro|2500|NaN|2500|
|1264|8632|HL4379|Televisão|4|Izabel|Lopes|3/10/2018|Rio de Janeiro|2500|NaN|10000|
|1265|8651|HL9962|Android|1|Natali|Rangel|1/31/2018|Rio de Janeiro|3400|NaN|3400|
|1266|8664|HL2714|Tablet|1|Lara|Moreira|5/7/2018|Rio de Janeiro|1600|NaN|1600|
|1267|8672|HL9962|Android|2|Julia|Figueiredo|4/29/2018|Rio de Janeiro|3400|NaN|6800|
|1268|8678|HL1148|Câmera|4|Kim|Ferreira|4/16/2018|Rio de Janeiro|2100|NaN|8400|
|1269|8682|HL1918|iPhone|1|Alberto|Silveira|1/29/2018|Rio de Janeiro|5300|NaN|5300|
|1270|8695|HL1148|Câmera|5|Bernardo|Ribeiro|12/29/2018|Rio de Janeiro|2100|NaN|10500|
|1271|8697|HL1918|iPhone|4|Roberto|Nogueira|12/3/2018|Rio de Janeiro|5300|NaN|21200|
|1272|8701|HL1918|iPhone|5|Gabrielle|Porto|2/11/2018|Rio de Janeiro|5300|NaN|26500|
|1273|8708|HL4379|Televisão|4|Breno|Quinto|8/2/2018|Rio de Janeiro|2500|NaN|10000|
|1274|8733|HL4379|Televisão|1|Lucas|Rodrigues|10/13/2018|Rio de Janeiro|2500|NaN|2500|
|1275|8740|HL8851|Notebook|5|Joana|Calmon|6/26/2018|Rio de Janeiro|3500|NaN|17500|
|1276|8775|HL9962|Android|4|Camila|Sobral|3/18/2018|Rio de Janeiro|3400|NaN|13600|
|1277|8782|HL8851|Notebook|5|Deysiane|Medronho|9/22/2018|Rio de Janeiro|3500|NaN|17500|
|1278|8792|HL1918|iPhone|5|Lucas|Lacerda|11/14/2018|Rio de Janeiro|5300|NaN|26500|
|1279|8798|HL1918|iPhone|3|Luiza|Farias|8/19/2018|Rio de Janeiro|5300|NaN|15900|
|1280|8803|HL1918|iPhone|2|Michelle|Figueiredo|6/21/2018|Rio de Janeiro|5300|NaN|10600|
|1281|8804|HL4379|Televisão|3|Lucas|Costa|2/16/2018|Rio de Janeiro|2500|NaN|7500|
|1282|8809|HL1148|Câmera|2|Raul|Silveira|9/10/2018|Rio de Janeiro|2100|NaN|4200|
|1283|8832|HL1148|Câmera|3|Rogério|Pereira|6/13/2018|Rio de Janeiro|2100|NaN|6300|
|1284|8835|HL1918|iPhone|1|Diego|Barros|12/24/2018|Rio de Janeiro|5300|NaN|5300|
|1285|8837|HL1148|Câmera|1|Gustavo|Accardo|5/22/2018|Rio de Janeiro|2100|NaN|2100|
|1286|8841|HL2714|Tablet|3|Myllena|Carneiro|9/25/2018|Rio de Janeiro|1600|NaN|4800|
|1287|8844|HL1918|iPhone|1|Tiago|Pereira|7/6/2018|Rio de Janeiro|5300|NaN|5300|
|1288|8846|HL1918|iPhone|2|Livia|Codeceira|11/20/2018|Rio de Janeiro|5300|NaN|10600|
|1289|8875|HL2714|Tablet|1|Larissa|Jesus|9/9/2018|Rio de Janeiro|1600|NaN|1600|
|1290|8885|HL1918|iPhone|4|Isabel|Lacerda|6/1/2018|Rio de Janeiro|5300|NaN|21200|
|1291|8895|HL8851|Notebook|5|Danilo|Alves|5/18/2018|Rio de Janeiro|3500|NaN|17500|
|1292|8896|HL4379|Televisão|4|Mariana|Miranda|6/15/2018|Rio de Janeiro|2500|NaN|10000|
|1293|8912|HL2714|Tablet|5|Caio|Silva|4/30/2018|Rio de Janeiro|1600|NaN|8000|
|1294|8919|HL1918|iPhone|5|Mariana|Rotava|3/12/2018|Rio de Janeiro|5300|NaN|26500|
|1295|8928|HL8851|Notebook|4|Hygor|Essaber|5/19/2018|Rio de Janeiro|3500|NaN|14000|
|1296|8929|HL4379|Televisão|5|Luis|Villanova|7/13/2018|Rio de Janeiro|2500|NaN|12500|
|1297|8939|HL1918|iPhone|5|Antônio|Oliveira|9/20/2018|Rio de Janeiro|5300|NaN|26500|
|1298|8965|HL1918|iPhone|1|Felipe|Paulo|9/7/2018|Rio de Janeiro|5300|NaN|5300|
|1299|8976|HL9962|Android|3|João|Ribeiro|10/24/2018|Rio de Janeiro|3400|NaN|10200|
|1300|8991|HL1918|iPhone|3|Laís|Oliveira|3/23/2018|Rio de Janeiro|5300|NaN|15900|
|1301|8994|HL7348|SmartWatch|2|Daniel|Nauenberg|1/13/2018|Rio de Janeiro|1400|NaN|2800|
|1302|9000|HL4379|Televisão|5|Hanna|Fonseca|6/6/2018|Rio de Janeiro|2500|NaN|12500|
|1303|9002|HL9962|Android|5|João|Rodrigues|4/15/2018|Rio de Janeiro|3400|NaN|17000|
|1304|9048|HL4379|Televisão|1|Gabriella|Lopes|2/10/2018|Rio de Janeiro|2500|NaN|2500|
|1305|9053|HL1918|iPhone|3|Eduardo|Ferreira|2/3/2018|Rio de Janeiro|5300|NaN|15900|
|1306|9061|HL1918|iPhone|3|Arthur|Pereira|4/15/2018|Rio de Janeiro|5300|NaN|15900|
|1307|9063|HL4379|Televisão|4|Clarissa|Santos|4/8/2018|Rio de Janeiro|2500|NaN|10000|
|1308|9072|HL1918|iPhone|1|Priscila|Garcia|12/16/2018|Rio de Janeiro|5300|NaN|5300|
|1309|9076|HL9962|Android|1|Renan|Nascimento|8/16/2018|Rio de Janeiro|3400|NaN|3400|
|1310|9080|HL1918|iPhone|5|Pedro|Cardoso|11/17/2018|Rio de Janeiro|5300|NaN|26500|
|1311|9086|HL1918|iPhone|3|Adriane|Gomes|5/14/2018|Rio de Janeiro|5300|NaN|15900|
|1312|9088|HL1918|iPhone|5|Gabriel|Rubim|9/13/2018|Rio de Janeiro|5300|NaN|26500|
|1313|9095|HL8851|Notebook|4|Carolina|Santos|6/21/2018|Rio de Janeiro|3500|NaN|14000|
|1314|9105|HL4379|Televisão|4|Rachel|Silva|2/17/2018|Rio de Janeiro|2500|NaN|10000|
|1315|9113|HL1918|iPhone|5|Ana|Silva|11/5/2018|Rio de Janeiro|5300|NaN|26500|
|1316|9115|HL1148|Câmera|4|Hygor|Essaber|11/30/2018|Rio de Janeiro|2100|NaN|8400|
|1317|9126|HL9962|Android|3|Adriane|Gomes|7/26/2018|Rio de Janeiro|3400|NaN|10200|
|1318|9138|HL8851|Notebook|4|Priscila|Garcia|2/1/2018|Rio de Janeiro|3500|NaN|14000|
|1319|9141|HL2714|Tablet|4|Amanda|Delgado|6/3/2018|Rio de Janeiro|1600|NaN|6400|
|1320|9150|HL1918|iPhone|1|Luis|Villanova|9/9/2018|Rio de Janeiro|5300|NaN|5300|
|1321|9157|HL7348|SmartWatch|3|Rachel|Silva|1/14/2018|Rio de Janeiro|1400|NaN|4200|
|1322|9161|HL1918|iPhone|1|Lucas|Lima|7/19/2018|Rio de Janeiro|5300|NaN|5300|
|1323|9164|HL8851|Notebook|5|Bruna|Rosa|7/29/2018|Rio de Janeiro|3500|NaN|17500|
|1324|9165|HL2714|Tablet|2|Juan|Fernandes|12/4/2018|Rio de Janeiro|1600|NaN|3200|
|1325|9166|HL2714|Tablet|2|Danilo|Alves|4/16/2018|Rio de Janeiro|1600|NaN|3200|
|1326|9167|HL1918|iPhone|1|Mateus|Polastri|3/3/2018|Rio de Janeiro|5300|NaN|5300|
|1327|9175|HL2714|Tablet|3|Lázaro|Nascimento|2/22/2018|Rio de Janeiro|1600|NaN|4800|
|1328|9176|HL1918|iPhone|4|Fillipe|Almeida|4/29/2018|Rio de Janeiro|5300|NaN|21200|
|1329|9186|HL8851|Notebook|3|Tadeu|Sousa|5/25/2018|Rio de Janeiro|3500|NaN|10500|
|1330|9190|HL2714|Tablet|2|Giovanna|Santos|10/11/2018|Rio de Janeiro|1600|NaN|3200|
|1331|9193|HL4379|Televisão|1|Ana|Leite|8/17/2018|Rio de Janeiro|2500|NaN|2500|
|1332|9195|HL1918|iPhone|5|Carolina|Rocha|11/21/2018|Rio de Janeiro|5300|NaN|26500|
|1333|9198|HL1918|iPhone|3|Rafael|Wajnsztok|3/10/2018|Rio de Janeiro|5300|NaN|15900|
|1334|9199|HL7348|SmartWatch|2|Alex|Fernandes|12/13/2018|Rio de Janeiro|1400|NaN|2800|
|1335|9202|HL2714|Tablet|5|Caio|Silva|3/1/2018|Rio de Janeiro|1600|NaN|8000|
|1336|9208|HL1918|iPhone|5|Cícero|Lima|6/11/2018|Rio de Janeiro|5300|NaN|26500|
|1337|9210|HL1918|iPhone|4|Victor|Gomes|12/1/2018|Rio de Janeiro|5300|NaN|21200|
|1338|9213|HL1918|iPhone|4|José|Fonseca|7/26/2018|Rio de Janeiro|5300|NaN|21200|
|1339|9216|HL4379|Televisão|1|Raul|Junqueira|6/16/2018|Rio de Janeiro|2500|NaN|2500|
|1340|9217|HL1918|iPhone|3|Caroline|Aquino|3/4/2018|Rio de Janeiro|5300|NaN|15900|
|1341|9226|HL1148|Câmera|2|Igor|Lima|9/20/2018|Rio de Janeiro|2100|NaN|4200|
|1342|9230|HL1918|iPhone|2|Camilla|Guimarães|2/8/2018|Rio de Janeiro|5300|NaN|10600|
|1343|9234|HL9962|Android|5|João|Monteiro|9/19/2018|Rio de Janeiro|3400|NaN|17000|
|1344|9240|HL4379|Televisão|1|Manuela|Merege|1/7/2018|Rio de Janeiro|2500|NaN|2500|
|1345|9256|HL1918|iPhone|3|Rafael|Carneiro|5/16/2018|Rio de Janeiro|5300|NaN|15900|
|1346|9262|HL4379|Televisão|3|Matheus|Ramos|5/3/2018|Rio de Janeiro|2500|NaN|7500|
|1347|9265|HL1148|Câmera|3|Gabriel|Thoni|9/13/2018|Rio de Janeiro|2100|NaN|6300|
|1348|9272|HL8851|Notebook|2|Eduardo|Pacheco|12/1/2018|Rio de Janeiro|3500|NaN|7000|
|1349|9275|HL4379|Televisão|2|José|Marques|11/12/2018|Rio de Janeiro|2500|NaN|5000|
|1350|9278|HL8851|Notebook|5|Andressa|Nóbrega|5/20/2018|Rio de Janeiro|3500|NaN|17500|
|1351|9285|HL1148|Câmera|3|Erick|Soares|1/24/2018|Rio de Janeiro|2100|NaN|6300|
|1352|9298|HL2714|Tablet|5|William|Mendonça|12/13/2018|Rio de Janeiro|1600|NaN|8000|
|1353|9303|HL1918|iPhone|2|David|Campelo|12/26/2018|Rio de Janeiro|5300|NaN|10600|
|1354|9304|HL1918|iPhone|1|Thomáz|Vannier|10/28/2018|Rio de Janeiro|5300|NaN|5300|
|1355|9313|HL9962|Android|1|João|Rodrigues|9/20/2018|Rio de Janeiro|3400|NaN|3400|
|1356|9318|HL1918|iPhone|4|Giuseppe|Bhering|1/7/2018|Rio de Janeiro|5300|NaN|21200|
|1357|9320|HL2714|Tablet|1|Raissa|Sales|12/20/2018|Rio de Janeiro|1600|NaN|1600|
|1358|9334|HL7348|SmartWatch|2|Dykson|Silva|11/30/2018|Rio de Janeiro|1400|NaN|2800|
|1359|9343|HL9962|Android|2|Jeferson|Sone|8/10/2018|Rio de Janeiro|3400|NaN|6800|
|1360|9345|HL2714|Tablet|2|Bruno|Salomão|9/5/2018|Rio de Janeiro|1600|NaN|3200|
|1361|9348|HL9962|Android|5|Camille|Silva|9/2/2018|Rio de Janeiro|3400|NaN|17000|
|1362|9371|HL4379|Televisão|1|João|Tabet|9/10/2018|Rio de Janeiro|2500|NaN|2500|
|1363|9377|HL1918|iPhone|4|Karina|Camara|7/2/2018|Rio de Janeiro|5300|NaN|21200|
|1364|9378|HL1918|iPhone|3|Matheus|Sapir|3/2/2018|Rio de Janeiro|5300|NaN|15900|
|1365|9389|HL1918|iPhone|4|Carolina|Rachide|5/11/2018|Rio de Janeiro|5300|NaN|21200|
|1366|9390|HL9962|Android|3|Gabrielle|Viríssimo|5/29/2018|Rio de Janeiro|3400|NaN|10200|
|1367|9396|HL2714|Tablet|5|Carolina|Costa|3/25/2018|Rio de Janeiro|1600|NaN|8000|
|1368|9397|HL8851|Notebook|1|Vinícius|Antunes|5/28/2018|Rio de Janeiro|3500|NaN|3500|
|1369|9399|HL4379|Televisão|4|Paola|Abreu|4/3/2018|Rio de Janeiro|2500|NaN|10000|
|1370|9400|HL4379|Televisão|2|Beatriz|Silva|1/19/2018|Rio de Janeiro|2500|NaN|5000|
|1371|9407|HL7348|SmartWatch|4|Giulia|Lopes|5/18/2018|Rio de Janeiro|1400|NaN|5600|
|1372|9408|HL1148|Câmera|4|João|Júnior|2/28/2018|Rio de Janeiro|2100|NaN|8400|
|1373|9409|HL1148|Câmera|1|Luiz|Campista|12/18/2018|Rio de Janeiro|2100|NaN|2100|
|1374|9412|HL8851|Notebook|4|Lucas|Rodrigues|2/12/2018|Rio de Janeiro|3500|NaN|14000|
|1375|9414|HL2714|Tablet|2|Fabio|Boccaletti|5/23/2018|Rio de Janeiro|1600|NaN|3200|
|1376|9415|HL1918|iPhone|4|Amanda|Braga|4/6/2018|Rio de Janeiro|5300|NaN|21200|
|1377|9416|HL1148|Câmera|3|Juan|Barbosa|8/19/2018|Rio de Janeiro|2100|NaN|6300|
|1378|9418|HL4379|Televisão|3|Deysiane|Medronho|12/20/2018|Rio de Janeiro|2500|NaN|7500|
|1379|9420|HL1918|iPhone|4|Letícia|Leal|12/14/2018|Rio de Janeiro|5300|NaN|21200|
|1380|9425|HL1148|Câmera|4|Breno|Quinto|1/7/2018|Rio de Janeiro|2100|NaN|8400|
|1381|9430|HL2714|Tablet|4|Daniel|Ortiz|3/20/2018|Rio de Janeiro|1600|NaN|6400|
|1382|9431|HL1918|iPhone|2|Thomáz|Rodriguez|2/8/2018|Rio de Janeiro|5300|NaN|10600|
|1383|9432|HL4379|Televisão|3|Luis|Silva|2/16/2018|Rio de Janeiro|2500|NaN|7500|
|1384|9433|HL1918|iPhone|4|Luiz|Almeida|2/7/2018|Rio de Janeiro|5300|NaN|21200|
|1385|9437|HL8851|Notebook|4|Lenon|Fernandes|3/27/2018|Rio de Janeiro|3500|NaN|14000|
|1386|9445|HL1918|iPhone|4|Gabrielle|Wanderley|1/17/2018|Rio de Janeiro|5300|NaN|21200|
|1387|9448|HL2714|Tablet|1|Carolina|Siqueira|2/26/2018|Rio de Janeiro|1600|NaN|1600|
|1388|9453|HL1918|iPhone|2|Adrielle|Vieira|10/5/2018|Rio de Janeiro|5300|NaN|10600|
|1389|9481|HL1918|iPhone|1|José|Carvalho|8/15/2018|Rio de Janeiro|5300|NaN|5300|
|1390|9494|HL7348|SmartWatch|4|Milena|Almeida|4/2/2018|Rio de Janeiro|1400|NaN|5600|
|1391|9504|HL1918|iPhone|2|Luana|Santos|9/12/2018|Rio de Janeiro|5300|NaN|10600|
|1392|9518|HL1918|iPhone|1|Pedro|Rodrigues|1/24/2018|Rio de Janeiro|5300|NaN|5300|
|1393|9519|HL4379|Televisão|4|Alon|Fahrnholz|8/21/2018|Rio de Janeiro|2500|NaN|10000|
|1394|9521|HL4379|Televisão|1|Caio|Caldas|3/20/2018|Rio de Janeiro|2500|NaN|2500|
|1395|9522|HL4379|Televisão|3|Victor|Lira|3/16/2018|Rio de Janeiro|2500|NaN|7500|
|1396|9538|HL9962|Android|2|Arthur|Souza|6/16/2018|Rio de Janeiro|3400|NaN|6800|
|1397|9539|HL9962|Android|1|Rebeca|Taylor|2/11/2018|Rio de Janeiro|3400|NaN|3400|
|1398|9542|HL1918|iPhone|1|Matheus|Sapir|6/6/2018|Rio de Janeiro|5300|NaN|5300|
|1399|9559|HL1918|iPhone|4|Lorena|Kohn|8/13/2018|Rio de Janeiro|5300|NaN|21200|
|1400|9560|HL1918|iPhone|1|João|Tabet|3/23/2018|Rio de Janeiro|5300|NaN|5300|
|1401|9562|HL8851|Notebook|2|Luiz|Almeida|2/12/2018|Rio de Janeiro|3500|NaN|7000|
|1402|9573|HL1918|iPhone|5|Natalia|Andrade|9/25/2018|Rio de Janeiro|5300|NaN|26500|
|1403|9576|HL1918|iPhone|5|Roberta|Pimenta|1/6/2018|Rio de Janeiro|5300|NaN|26500|
|1404|9582|HL7348|SmartWatch|1|João|Costa|3/16/2018|Rio de Janeiro|1400|NaN|1400|
|1405|9593|HL9962|Android|1|Douglas|Rodrigues|4/12/2018|Rio de Janeiro|3400|NaN|3400|
|1406|9595|HL1148|Câmera|5|João|Alves|7/25/2018|Rio de Janeiro|2100|NaN|10500|
|1407|9598|HL8851|Notebook|4|Isaac|Santos|2/8/2018|Rio de Janeiro|3500|NaN|14000|
|1408|9599|HL1918|iPhone|5|Daniel|Nauenberg|9/21/2018|Rio de Janeiro|5300|NaN|26500|
|1409|9625|HL1918|iPhone|2|Breno|Britto|1/25/2018|Rio de Janeiro|5300|NaN|10600|
|1410|9633|HL1918|iPhone|1|Carolina|Siqueira|8/14/2018|Rio de Janeiro|5300|NaN|5300|
|1411|9635|HL1148|Câmera|3|Bruno|Freitas|9/20/2018|Rio de Janeiro|2100|NaN|6300|
|1412|9638|HL2714|Tablet|5|Júlio|Fraga|5/25/2018|Rio de Janeiro|1600|NaN|8000|
|1413|9655|HL4379|Televisão|2|Ana|Miura|7/28/2018|Rio de Janeiro|2500|NaN|5000|
|1414|9656|HL7348|SmartWatch|2|Danilo|Rubim|7/31/2018|Rio de Janeiro|1400|NaN|2800|
|1415|9666|HL7348|SmartWatch|5|Breno|Godoy|8/14/2018|Rio de Janeiro|1400|NaN|7000|
|1416|9668|HL4379|Televisão|2|Letícia|Araujo|7/10/2018|Rio de Janeiro|2500|NaN|5000|
|1417|9675|HL2714|Tablet|2|Nathan|Cunha|6/13/2018|Rio de Janeiro|1600|NaN|3200|
|1418|9680|HL7348|SmartWatch|1|Ana|Carvalho|5/3/2018|Rio de Janeiro|1400|NaN|1400|
|1419|9691|HL1918|iPhone|4|Guilherme|Lima|2/18/2018|Rio de Janeiro|5300|NaN|21200|
|1420|9694|HL9962|Android|2|Tiago|Pereira|7/5/2018|Rio de Janeiro|3400|NaN|6800|
|1421|9697|HL1918|iPhone|4|Victor|Lira|9/18/2018|Rio de Janeiro|5300|NaN|21200|
|1422|9701|HL1918|iPhone|5|Guilherme|Castilho|9/25/2018|Rio de Janeiro|5300|NaN|26500|
|1423|9702|HL4379|Televisão|2|Breno|Caputo|6/27/2018|Rio de Janeiro|2500|NaN|5000|
|1424|9708|HL4379|Televisão|2|Victoria|Mazza|1/28/2018|Rio de Janeiro|2500|NaN|5000|
|1425|9723|HL9962|Android|3|Laís|Oliveira|9/10/2018|Rio de Janeiro|3400|NaN|10200|
|1426|9728|HL2714|Tablet|4|Pedro|Oliveira|10/27/2018|Rio de Janeiro|1600|NaN|6400|
|1427|9730|HL4379|Televisão|4|Myllena|Corrêa|6/3/2018|Rio de Janeiro|2500|NaN|10000|
|1428|9732|HL7348|SmartWatch|4|Gustavo|Junior|8/10/2018|Rio de Janeiro|1400|NaN|5600|
|1429|9736|HL1918|iPhone|5|Brenno|Miranda|5/25/2018|Rio de Janeiro|5300|NaN|26500|
|1430|9737|HL1918|iPhone|4|Marcela|Johnson|8/13/2018|Rio de Janeiro|5300|NaN|21200|
|1431|9740|HL8851|Notebook|5|Bernardo|Nauenberg|4/1/2018|Rio de Janeiro|3500|NaN|17500|
|1432|9745|HL9962|Android|5|Jéssica|Netto|9/24/2018|Rio de Janeiro|3400|NaN|17000|
|1433|9752|HL2714|Tablet|2|Gabrielle|Wanderley|7/30/2018|Rio de Janeiro|1600|NaN|3200|
|1434|9763|HL9962|Android|5|Beatriz|Nogueira|1/12/2018|Rio de Janeiro|3400|NaN|17000|
|1435|9764|HL1918|iPhone|4|Vivianne|Rodrigues|6/6/2018|Rio de Janeiro|5300|NaN|21200|
|1436|9785|HL1148|Câmera|5|Carolina|Carneiro|8/3/2018|Rio de Janeiro|2100|NaN|10500|
|1437|9788|HL1918|iPhone|3|Vivianne|Rodrigues|7/29/2018|Rio de Janeiro|5300|NaN|15900|
|1438|9803|HL8851|Notebook|5|Roger|Rosa|6/8/2018|Rio de Janeiro|3500|NaN|17500|
|1439|9806|HL1918|iPhone|3|Isabella|Santos|2/7/2018|Rio de Janeiro|5300|NaN|15900|
|1440|9809|HL1918|iPhone|3|Lucas|Aragão|1/15/2018|Rio de Janeiro|5300|NaN|15900|
|1441|9816|HL4379|Televisão|3|Wendela|Veloso|5/9/2018|Rio de Janeiro|2500|NaN|7500|
|1442|9828|HL9962|Android|1|Gabriel|Almeida|2/22/2018|Rio de Janeiro|3400|NaN|3400|
|1443|9858|HL1918|iPhone|4|Luã|Sá|11/25/2018|Rio de Janeiro|5300|NaN|21200|
|1444|9877|HL1918|iPhone|3|Yasser|Calbucci|5/19/2018|Rio de Janeiro|5300|NaN|15900|
|1445|9891|HL1918|iPhone|2|Rafael|Guimarães|4/25/2018|Rio de Janeiro|5300|NaN|10600|
|1446|9899|HL7348|SmartWatch|3|Carlos|Assis|3/23/2018|Rio de Janeiro|1400|NaN|4200|
|1447|9902|HL4379|Televisão|4|Ana|Silva|11/7/2018|Rio de Janeiro|2500|NaN|10000|
|1448|9904|HL7348|SmartWatch|3|Gabriel|Brito|7/19/2018|Rio de Janeiro|1400|NaN|4200|
|1449|9906|HL1918|iPhone|5|Samara|Pinto|1/10/2018|Rio de Janeiro|5300|NaN|26500|
|1450|9907|HL1918|iPhone|1|Matheus|Sapir|8/15/2018|Rio de Janeiro|5300|NaN|5300|
|1451|9911|HL2714|Tablet|1|Maria|Moita|5/8/2018|Rio de Janeiro|1600|NaN|1600|
|1452|9926|HL1918|iPhone|5|Nina|Magalhães|11/9/2018|Rio de Janeiro|5300|NaN|26500|
|1453|9935|HL4379|Televisão|2|Maria|Correa|11/4/2018|Rio de Janeiro|2500|NaN|5000|
|1454|9946|HL1148|Câmera|2|Henrique|Silva|12/14/2018|Rio de Janeiro|2100|NaN|4200|
|1455|9948|HL4379|Televisão|3|Mariana|Barrozo|11/24/2018|Rio de Janeiro|2500|NaN|7500|
|1456|9951|HL1918|iPhone|5|Ana|Almeida|10/20/2018|Rio de Janeiro|5300|NaN|26500|
|1457|9952|HL4379|Televisão|4|Rubens|Netto|3/26/2018|Rio de Janeiro|2500|NaN|10000|
|1458|9955|HL1918|iPhone|1|Bruno|Oliveira|5/4/2018|Rio de Janeiro|5300|NaN|5300|
|1459|9960|HL7348|SmartWatch|3|Chan|Santos|7/1/2018|Rio de Janeiro|1400|NaN|4200|
|1460|9961|HL2714|Tablet|2|Eduardo|Peluzo|2/19/2018|Rio de Janeiro|1600|NaN|3200|
|1461|9966|HL1918|iPhone|2|João|Pedrazza|9/20/2018|Rio de Janeiro|5300|NaN|10600|
|1462|9971|HL1918|iPhone|4|Isaac|Santos|12/3/2018|Rio de Janeiro|5300|NaN|21200|
|1463|9976|HL9962|Android|2|Andreza|Ramos|12/17/2018|Rio de Janeiro|3400|NaN|6800|
|1464|9982|HL4379|Televisão|3|Leticia|Mesquita|5/22/2018|Rio de Janeiro|2500|NaN|7500|
|1465|9987|HL1918|iPhone|5|Manuela|Merege|9/12/2018|Rio de Janeiro|5300|NaN|26500|
|1466|9989|HL1918|iPhone|5|Rafael|Carneiro|2/28/2018|Rio de Janeiro|5300|NaN|26500|
|0|13|HL4379|Televisão|1|Daniel|Monteiro|5/23/2018|Goiás|2500|NaN|2500|
|1|19|HL9962|Android|4|Elaine|Santos|7/5/2018|Goiás|3400|NaN|13600|
|2|45|HL1918|iPhone|5|Lenon|Fernandes|3/31/2018|Goiás|5300|NaN|26500|
|3|50|HL7348|SmartWatch|1|Vivianne|Rodrigues|8/11/2018|Goiás|1400|NaN|1400|
|4|97|HL7348|SmartWatch|2|Pedro|Rodrigues|7/26/2018|Goiás|1400|NaN|2800|
|5|116|HL2714|Tablet|3|Caio|Cardoso|6/18/2018|Goiás|1600|NaN|4800|
|6|123|HL2714|Tablet|4|Lucas|Freire|1/13/2018|Goiás|1600|NaN|6400|
|7|130|HL9962|Android|5|Caio|Fernandes|7/25/2018|Goiás|3400|NaN|17000|
|8|133|HL1918|iPhone|4|Kim|Ferreira|5/11/2018|Goiás|5300|NaN|21200|
|9|135|HL4379|Televisão|4|Beatriz|Rocha|10/23/2018|Goiás|2500|NaN|10000|
|10|139|HL4379|Televisão|2|Leandro|Ferreira|1/25/2018|Goiás|2500|NaN|5000|
|11|146|HL1918|iPhone|1|Thomáz|Bôas|7/22/2018|Goiás|5300|NaN|5300|
|12|159|HL9962|Android|4|Philipe|Morete|10/18/2018|Goiás|3400|NaN|13600|
|13|164|HL4379|Televisão|3|Felipe|Jorge|7/10/2018|Goiás|2500|NaN|7500|
|14|181|HL9962|Android|2|João|Junior|1/11/2018|Goiás|3400|NaN|6800|
|15|187|HL1918|iPhone|4|Marina|Gama|7/20/2018|Goiás|5300|NaN|21200|
|16|197|HL4379|Televisão|4|Rilson|Guedes|3/15/2018|Goiás|2500|NaN|10000|
|17|205|HL1918|iPhone|4|Felipe|Mello|3/13/2018|Goiás|5300|NaN|21200|
|18|228|HL8851|Notebook|3|Beatriz|Silva|9/21/2018|Goiás|3500|NaN|10500|
|19|233|HL7348|SmartWatch|3|Vanessa|Rodrigues|10/20/2018|Goiás|1400|NaN|4200|
|20|246|HL7348|SmartWatch|4|Camila|Bastazini|4/28/2018|Goiás|1400|NaN|5600|
|21|265|HL1918|iPhone|4|Julia|Teixeira|6/5/2018|Goiás|5300|NaN|21200|
|22|267|HL2714|Tablet|2|Raissa|Sales|9/21/2018|Goiás|1600|NaN|3200|
|23|281|HL1918|iPhone|1|Lorena|Carvalho|2/10/2018|Goiás|5300|NaN|5300|
|24|293|HL7348|SmartWatch|4|Beatriz|Biase|11/8/2018|Goiás|1400|NaN|5600|
|25|312|HL1148|Câmera|4|Juliana|Goes|8/19/2018|Goiás|2100|NaN|8400|
|26|355|HL1918|iPhone|5|Guilherme|Monteiro|11/9/2018|Goiás|5300|NaN|26500|
|27|356|HL1918|iPhone|4|Rafaela|Gomes|3/26/2018|Goiás|5300|NaN|21200|
|28|395|HL4379|Televisão|2|William|Mendonça|3/27/2018|Goiás|2500|NaN|5000|
|29|421|HL8851|Notebook|2|Clara|Silveira|9/16/2018|Goiás|3500|NaN|7000|
|30|441|HL4379|Televisão|2|David|Assumpção|10/25/2018|Goiás|2500|NaN|5000|
|31|447|HL4379|Televisão|5|Camilla|Cardeman|11/20/2018|Goiás|2500|NaN|12500|
|32|450|HL4379|Televisão|1|Julie|Ferreira|4/19/2018|Goiás|2500|NaN|2500|
|33|479|HL8851|Notebook|5|Myllena|Carneiro|4/4/2018|Goiás|3500|NaN|17500|
|34|498|HL1918|iPhone|1|Izabel|Miura|5/12/2018|Goiás|5300|NaN|5300|
|35|504|HL1918|iPhone|5|Rojane|Lima|9/24/2018|Goiás|5300|NaN|26500|
|36|512|HL1918|iPhone|4|Luiza|Procaci|4/19/2018|Goiás|5300|NaN|21200|
|37|525|HL8851|Notebook|1|Lucas|Neto|5/2/2018|Goiás|3500|NaN|3500|
|38|541|HL9962|Android|3|Beatriz|Li|9/20/2018|Goiás|3400|NaN|10200|
|39|556|HL8851|Notebook|5|Arthur|Pereira|4/13/2018|Goiás|3500|NaN|17500|
|40|560|HL4379|Televisão|2|Mateus|Maia|7/9/2018|Goiás|2500|NaN|5000|
|41|572|HL2714|Tablet|5|Thaís|Ribeiro|10/29/2018|Goiás|1600|NaN|8000|
|42|588|HL1918|iPhone|3|Nicolas|Monteiro|12/14/2018|Goiás|5300|NaN|15900|
|43|597|HL4379|Televisão|1|Amanda|Braga|9/15/2018|Goiás|2500|NaN|2500|
|44|615|HL9962|Android|4|Carolina|Santos|6/11/2018|Goiás|3400|NaN|13600|
|45|636|HL1918|iPhone|1|Raíssa|Oros|12/31/2018|Goiás|5300|NaN|5300|
|46|637|HL7348|SmartWatch|5|Rodrigo|Bruno|2/9/2018|Goiás|1400|NaN|7000|
|47|655|HL4379|Televisão|1|Eduardo|Soares|10/31/2018|Goiás|2500|NaN|2500|
|48|668|HL1918|iPhone|2|Rebeca|Reis|9/12/2018|Goiás|5300|NaN|10600|
|49|670|HL4379|Televisão|5|Gabriel|Rubim|2/6/2018|Goiás|2500|NaN|12500|
|50|716|HL1148|Câmera|1|Diego|Rodrigues|10/17/2018|Goiás|2100|NaN|2100|
|51|728|HL7348|SmartWatch|3|Danilo|Rubim|3/21/2018|Goiás|1400|NaN|4200|
|52|754|HL9962|Android|5|Fabio|Boccaletti|11/22/2018|Goiás|3400|NaN|17000|
|53|755|HL1148|Câmera|1|Samara|Pinto|3/26/2018|Goiás|2100|NaN|2100|
|54|770|HL1918|iPhone|5|Desirée|Heimlich|11/6/2018|Goiás|5300|NaN|26500|
|55|774|HL9962|Android|2|Lucas|Freitas|10/28/2018|Goiás|3400|NaN|6800|
|56|776|HL4379|Televisão|1|Pedro|Macckione|9/19/2018|Goiás|2500|NaN|2500|
|57|786|HL9962|Android|2|Lunna|Vannier|12/22/2018|Goiás|3400|NaN|6800|
|58|805|HL9962|Android|4|João|Capitulo|11/14/2018|Goiás|3400|NaN|13600|
|59|810|HL4379|Televisão|4|Lucas|Rodrigues|7/7/2018|Goiás|2500|NaN|10000|
|60|826|HL4379|Televisão|1|João|Capitulo|11/16/2018|Goiás|2500|NaN|2500|
|61|829|HL1148|Câmera|1|Victor|Zakhm|11/15/2018|Goiás|2100|NaN|2100|
|62|841|HL4379|Televisão|5|Lucas|Neto|9/29/2018|Goiás|2500|NaN|12500|
|63|865|HL1918|iPhone|4|Gabriel|Rocha|3/19/2018|Goiás|5300|NaN|21200|
|64|884|HL4379|Televisão|5|Anna|Maia|8/13/2018|Goiás|2500|NaN|12500|
|65|892|HL1918|iPhone|5|Patrícia|Amaral|8/21/2018|Goiás|5300|NaN|26500|
|66|907|HL1918|iPhone|3|Helena|Chafin|5/25/2018|Goiás|5300|NaN|15900|
|67|920|HL4379|Televisão|5|Andre|Nóbrega|10/16/2018|Goiás|2500|NaN|12500|
|68|924|HL1148|Câmera|4|Bianca|Piero|10/11/2018|Goiás|2100|NaN|8400|
|69|939|HL1918|iPhone|4|Matheus|Ramos|12/4/2018|Goiás|5300|NaN|21200|
|70|951|HL4379|Televisão|1|Dykson|Silva|5/26/2018|Goiás|2500|NaN|2500|
|71|989|HL9962|Android|5|Rafaela|Rodrigues|9/4/2018|Goiás|3400|NaN|17000|
|72|1011|HL1148|Câmera|2|Amanda|Procaci|2/15/2018|Goiás|2100|NaN|4200|
|73|1034|HL1918|iPhone|2|Larissa|Jesus|3/21/2018|Goiás|5300|NaN|10600|
|74|1035|HL1918|iPhone|3|Carolina|Vasconcelos|3/3/2018|Goiás|5300|NaN|15900|
|75|1040|HL4379|Televisão|1|Bianca|Piero|2/12/2018|Goiás|2500|NaN|2500|
|76|1051|HL9962|Android|2|Andressa|Chou|1/4/2018|Goiás|3400|NaN|6800|
|77|1055|HL1918|iPhone|5|Anízio|Carvalho|12/5/2018|Goiás|5300|NaN|26500|
|78|1086|HL1918|iPhone|2|Lucas|Monte|6/6/2018|Goiás|5300|NaN|10600|
|79|1116|HL4379|Televisão|5|Victor|Magalhães|8/14/2018|Goiás|2500|NaN|12500|
|80|1142|HL4379|Televisão|4|Raul|Junqueira|2/3/2018|Goiás|2500|NaN|10000|
|81|1149|HL9962|Android|2|Karina|Camara|9/17/2018|Goiás|3400|NaN|6800|
|82|1150|HL1918|iPhone|5|Larissa|Vasconcellos|1/9/2018|Goiás|5300|NaN|26500|
|83|1163|HL1918|iPhone|1|Audir|Franco|2/25/2018|Goiás|5300|NaN|5300|
|84|1165|HL9962|Android|5|Thiago|Miura|11/21/2018|Goiás|3400|NaN|17000|
|85|1182|HL8851|Notebook|4|Adriana|Passos|10/11/2018|Goiás|3500|NaN|14000|
|86|1199|HL8851|Notebook|3|Lucas|Monte|11/27/2018|Goiás|3500|NaN|10500|
|87|1234|HL4379|Televisão|5|Roberta|Pimenta|4/13/2018|Goiás|2500|NaN|12500|
|88|1263|HL4379|Televisão|3|Henrique|Lencastre|7/17/2018|Goiás|2500|NaN|7500|
|89|1272|HL1148|Câmera|4|Guilherme|Lima|11/6/2018|Goiás|2100|NaN|8400|
|90|1299|HL8851|Notebook|4|Lívia|Tanaka|3/9/2018|Goiás|3500|NaN|14000|
|91|1309|HL7348|SmartWatch|2|Pedro|Costa|9/26/2018|Goiás|1400|NaN|2800|
|92|1328|HL4379|Televisão|2|Victor|Gomes|12/5/2018|Goiás|2500|NaN|5000|
|93|1335|HL2714|Tablet|4|Rilson|Guedes|1/2/2018|Goiás|1600|NaN|6400|
|94|1345|HL7348|SmartWatch|5|Pedro|Martins|6/22/2018|Goiás|1400|NaN|7000|
|95|1386|HL4379|Televisão|5|Caroline|Cavalcanti|12/10/2018|Goiás|2500|NaN|12500|
|96|1403|HL4379|Televisão|4|Gabriel|Brito|1/27/2018|Goiás|2500|NaN|10000|
|97|1407|HL4379|Televisão|1|Thomáz|Rodriguez|2/14/2018|Goiás|2500|NaN|2500|
|98|1416|HL8851|Notebook|4|Elena|Barreto|4/5/2018|Goiás|3500|NaN|14000|
|99|1419|HL1918|iPhone|2|Lorena|Carvalho|11/19/2018|Goiás|5300|NaN|10600|
|100|1435|HL8851|Notebook|4|Pedro|Macckione|5/19/2018|Goiás|3500|NaN|14000|
|101|1437|HL1918|iPhone|5|Carolina|Rachide|10/8/2018|Goiás|5300|NaN|26500|
|102|1448|HL7348|SmartWatch|3|Felipe|Paulo|4/22/2018|Goiás|1400|NaN|4200|
|103|1456|HL7348|SmartWatch|3|Lenon|Fernandes|7/8/2018|Goiás|1400|NaN|4200|
|104|1463|HL7348|SmartWatch|3|Eduardo|Pacheco|7/28/2018|Goiás|1400|NaN|4200|
|105|1464|HL4379|Televisão|4|Allan|Candido|9/18/2018|Goiás|2500|NaN|10000|
|106|1465|HL1918|iPhone|1|Daniel|Sousa|11/19/2018|Goiás|5300|NaN|5300|
|107|1469|HL4379|Televisão|3|Luiz|Campista|4/16/2018|Goiás|2500|NaN|7500|
|108|1492|HL1918|iPhone|3|Raíssa|Oliveira|3/11/2018|Goiás|5300|NaN|15900|
|109|1494|HL4379|Televisão|4|Rafael|Guimarães|8/19/2018|Goiás|2500|NaN|10000|
|110|1506|HL1918|iPhone|1|Jackson|Derossi|1/16/2018|Goiás|5300|NaN|5300|
|111|1508|HL4379|Televisão|1|Marina|Correa|8/29/2018|Goiás|2500|NaN|2500|
|112|1510|HL4379|Televisão|3|Maria|Junior|5/2/2018|Goiás|2500|NaN|7500|
|113|1539|HL2714|Tablet|5|Raissa|Sales|1/9/2018|Goiás|1600|NaN|8000|
|114|1543|HL7348|SmartWatch|3|Julia|Aliani|5/2/2018|Goiás|1400|NaN|4200|
|115|1556|HL1918|iPhone|5|Lívia|Marques|4/5/2018|Goiás|5300|NaN|26500|
|116|1574|HL1918|iPhone|1|Carlos|Mesquita|4/14/2018|Goiás|5300|NaN|5300|
|117|1579|HL9962|Android|3|Gabrielle|Costa|8/22/2018|Goiás|3400|NaN|10200|
|118|1598|HL9962|Android|3|Larissa|Jesus|12/20/2018|Goiás|3400|NaN|10200|
|119|1604|HL8851|Notebook|3|Bianca|Tatsch|7/6/2018|Goiás|3500|NaN|10500|
|120|1618|HL2714|Tablet|2|Raíssa|Oros|3/21/2018|Goiás|1600|NaN|3200|
|121|1644|HL1918|iPhone|4|Ana|Carvalho|12/30/2018|Goiás|5300|NaN|21200|
|122|1645|HL4379|Televisão|4|Nathan|Morelli|11/8/2018|Goiás|2500|NaN|10000|
|123|1647|HL2714|Tablet|4|Thiago|Costa|7/13/2018|Goiás|1600|NaN|6400|
|124|1655|HL1918|iPhone|2|Caroline|Cavalcanti|2/19/2018|Goiás|5300|NaN|10600|
|125|1690|HL1918|iPhone|3|Sarah|Souza|7/8/2018|Goiás|5300|NaN|15900|
|126|1733|HL2714|Tablet|5|Antônio|Soares|12/21/2018|Goiás|1600|NaN|8000|
|127|1734|HL1918|iPhone|2|Igor|Lima|8/31/2018|Goiás|5300|NaN|10600|
|128|1736|HL1918|iPhone|1|Paloma|Sperandei|12/2/2018|Goiás|5300|NaN|5300|
|129|1742|HL1918|iPhone|3|Raissa|Sales|4/26/2018|Goiás|5300|NaN|15900|
|130|1755|HL8851|Notebook|4|Wilson|Miranda|1/31/2018|Goiás|3500|NaN|14000|
|131|1767|HL1918|iPhone|4|Gabrielle|Wanderley|11/19/2018|Goiás|5300|NaN|21200|
|132|1772|HL1148|Câmera|1|Raissa|Maia|8/25/2018|Goiás|2100|NaN|2100|
|133|1779|HL1918|iPhone|4|Lucas|Wanderley|6/4/2018|Goiás|5300|NaN|21200|
|134|1780|HL7348|SmartWatch|4|Michelle|Miura|3/9/2018|Goiás|1400|NaN|5600|
|135|1796|HL4379|Televisão|2|Gabriela|Mello|11/10/2018|Goiás|2500|NaN|5000|
|136|1801|HL9962|Android|1|Isabel|Leite|11/10/2018|Goiás|3400|NaN|3400|
|137|1808|HL1918|iPhone|3|João|Monteiro|10/4/2018|Goiás|5300|NaN|15900|
|138|1816|HL8851|Notebook|2|Isabella|Santos|10/10/2018|Goiás|3500|NaN|7000|
|139|1820|HL1148|Câmera|2|Miguel|Carneiro|10/5/2018|Goiás|2100|NaN|4200|
|140|1823|HL9962|Android|3|Marina|Miranda|1/22/2018|Goiás|3400|NaN|10200|
|141|1844|HL1918|iPhone|2|Isabella|Montanholi|4/5/2018|Goiás|5300|NaN|10600|
|142|1859|HL1918|iPhone|5|Manuela|Ferreira|1/21/2018|Goiás|5300|NaN|26500|
|143|1862|HL2714|Tablet|5|Ana|Felippe|3/4/2018|Goiás|1600|NaN|8000|
|144|1866|HL1918|iPhone|2|Maria|Gasperi|3/29/2018|Goiás|5300|NaN|10600|
|145|1868|HL1918|iPhone|3|Cézar|Santos|2/10/2018|Goiás|5300|NaN|15900|
|146|1870|HL4379|Televisão|4|Paula|Cavalcanti|11/30/2018|Goiás|2500|NaN|10000|
|147|1879|HL4379|Televisão|3|Lucas|Machado|1/5/2018|Goiás|2500|NaN|7500|
|148|1882|HL4379|Televisão|1|Raul|Junqueira|1/20/2018|Goiás|2500|NaN|2500|
|149|1890|HL4379|Televisão|3|José|Fonseca|1/29/2018|Goiás|2500|NaN|7500|
|150|1974|HL1918|iPhone|5|Cézar|Santos|3/19/2018|Goiás|5300|NaN|26500|
|151|1979|HL7348|SmartWatch|3|Hygor|Essaber|9/13/2018|Goiás|1400|NaN|4200|
|152|2018|HL7348|SmartWatch|1|Norman|Jimbo|12/25/2018|Goiás|1400|NaN|1400|
|153|2040|HL4379|Televisão|3|Isabella|Rodrigues|5/13/2018|Goiás|2500|NaN|7500|
|154|2064|HL4379|Televisão|5|Arthur|Fernandes|6/9/2018|Goiás|2500|NaN|12500|
|155|2117|HL9962|Android|3|Vanessa|Neves|3/21/2018|Goiás|3400|NaN|10200|
|156|2156|HL1918|iPhone|3|Cícero|Lima|9/22/2018|Goiás|5300|NaN|15900|
|157|2162|HL4379|Televisão|3|Luíza|Garcia|3/15/2018|Goiás|2500|NaN|7500|
|158|2165|HL8851|Notebook|2|Rebeca|Manhães|4/23/2018|Goiás|3500|NaN|7000|
|159|2179|HL9962|Android|5|Carlos|Melo|4/8/2018|Goiás|3400|NaN|17000|
|160|2182|HL1918|iPhone|5|Rafaela|Rodrigues|5/1/2018|Goiás|5300|NaN|26500|
|161|2192|HL1918|iPhone|2|Guilherme|Lima|11/15/2018|Goiás|5300|NaN|10600|
|162|2195|HL1918|iPhone|2|Daniel|Nauenberg|2/21/2018|Goiás|5300|NaN|10600|
|163|2207|HL1918|iPhone|3|João|Castilho|11/30/2018|Goiás|5300|NaN|15900|
|164|2217|HL4379|Televisão|1|Letícia|Rodrigues|9/12/2018|Goiás|2500|NaN|2500|
|165|2232|HL2714|Tablet|2|Leonardo|Faria|12/3/2018|Goiás|1600|NaN|3200|
|166|2242|HL2714|Tablet|4|Katharina|Barros|3/4/2018|Goiás|1600|NaN|6400|
|167|2246|HL2714|Tablet|4|Antonio|Manhães|7/10/2018|Goiás|1600|NaN|6400|
|168|2248|HL1918|iPhone|5|Thais|Rodrigues|2/3/2018|Goiás|5300|NaN|26500|
|169|2256|HL4379|Televisão|1|Adriane|Gomes|6/30/2018|Goiás|2500|NaN|2500|
|170|2262|HL4379|Televisão|5|Rafael|Wajnsztok|5/20/2018|Goiás|2500|NaN|12500|
|171|2277|HL8851|Notebook|4|Camilla|Cardeman|3/28/2018|Goiás|3500|NaN|14000|
|172|2286|HL4379|Televisão|4|Leonardo|Ferreira|8/29/2018|Goiás|2500|NaN|10000|
|173|2297|HL1918|iPhone|2|Marina|Marins|9/27/2018|Goiás|5300|NaN|10600|
|174|2303|HL9962|Android|2|Bianca|Allevato|8/25/2018|Goiás|3400|NaN|6800|
|175|2307|HL2714|Tablet|3|Julia|Figueiredo|3/10/2018|Goiás|1600|NaN|4800|
|176|2351|HL1918|iPhone|4|Juliana|Souza|9/2/2018|Goiás|5300|NaN|21200|
|177|2394|HL4379|Televisão|1|Helena|Chafin|12/25/2018|Goiás|2500|NaN|2500|
|178|2396|HL9962|Android|2|Anderson|Cavalcanti|9/29/2018|Goiás|3400|NaN|6800|
|179|2428|HL2714|Tablet|1|Rafaela|Ferreira|1/26/2018|Goiás|1600|NaN|1600|
|180|2429|HL9962|Android|4|Ananda|Dias|10/8/2018|Goiás|3400|NaN|13600|
|181|2456|HL7348|SmartWatch|5|Lucas|Almeida|12/22/2018|Goiás|1400|NaN|7000|
|182|2469|HL1918|iPhone|4|Julia|Teixeira|12/31/2018|Goiás|5300|NaN|21200|
|183|2486|HL1918|iPhone|3|Luíza|Melo|7/3/2018|Goiás|5300|NaN|15900|
|184|2535|HL1148|Câmera|3|João|Araujo|5/10/2018|Goiás|2100|NaN|6300|
|185|2541|HL1148|Câmera|4|Bruna|Gomes|7/22/2018|Goiás|2100|NaN|8400|
|186|2557|HL1918|iPhone|5|Daniela|Andrada|4/26/2018|Goiás|5300|NaN|26500|
|187|2582|HL1148|Câmera|1|Adrielle|Forte|5/20/2018|Goiás|2100|NaN|2100|
|188|2611|HL1918|iPhone|4|Thais|Rodrigues|9/25/2018|Goiás|5300|NaN|21200|
|189|2614|HL4379|Televisão|2|Elena|Barreto|5/21/2018|Goiás|2500|NaN|5000|
|190|2632|HL8851|Notebook|3|Marina|Marins|6/1/2018|Goiás|3500|NaN|10500|
|191|2634|HL1918|iPhone|5|Luiz|Campista|8/8/2018|Goiás|5300|NaN|26500|
|192|2653|HL1918|iPhone|4|João|Pedrazza|11/2/2018|Goiás|5300|NaN|21200|
|193|2672|HL1148|Câmera|4|Deysiane|Medronho|1/19/2018|Goiás|2100|NaN|8400|
|194|2695|HL1918|iPhone|5|Kimberly|Sad|9/30/2018|Goiás|5300|NaN|26500|
|195|2710|HL1918|iPhone|1|Arthur|Fernandes|8/5/2018|Goiás|5300|NaN|5300|
|196|2713|HL7348|SmartWatch|1|Isabel|Leite|9/3/2018|Goiás|1400|NaN|1400|
|197|2720|HL2714|Tablet|5|Juan|Fernandes|2/6/2018|Goiás|1600|NaN|8000|
|198|2721|HL9962|Android|4|João|Ribeiro|1/21/2018|Goiás|3400|NaN|13600|
|199|2735|HL8851|Notebook|4|Hércules|Moreira|12/22/2018|Goiás|3500|NaN|14000|
|200|2760|HL9962|Android|1|Victor|Ferreira|11/12/2018|Goiás|3400|NaN|3400|
|201|2775|HL9962|Android|2|Silvio|Fahrnholz|12/10/2018|Goiás|3400|NaN|6800|
|202|2779|HL9962|Android|5|Larissa|Jesus|1/11/2018|Goiás|3400|NaN|17000|
|203|2793|HL2714|Tablet|1|Henrique|Oliveira|9/9/2018|Goiás|1600|NaN|1600|
|204|2809|HL1148|Câmera|3|José|Jesus|6/20/2018|Goiás|2100|NaN|6300|
|205|2823|HL1918|iPhone|3|Isabella|Rodrigues|11/13/2018|Goiás|5300|NaN|15900|
|206|2835|HL1148|Câmera|3|Gabriel|Pereira|2/3/2018|Goiás|2100|NaN|6300|
|207|2855|HL1148|Câmera|2|Fillipe|Almeida|6/1/2018|Goiás|2100|NaN|4200|
|208|2862|HL7348|SmartWatch|1|Sandy|Moreira|6/9/2018|Goiás|1400|NaN|1400|
|209|2869|HL2714|Tablet|1|Fillipe|Almeida|10/3/2018|Goiás|1600|NaN|1600|
|210|2912|HL1918|iPhone|5|Luiz|Limp|10/13/2018|Goiás|5300|NaN|26500|
|211|2920|HL4379|Televisão|5|Daniel|Araujo|3/13/2018|Goiás|2500|NaN|12500|
|212|2932|HL4379|Televisão|5|Alexandre|Rodriguez|5/20/2018|Goiás|2500|NaN|12500|
|213|2942|HL1918|iPhone|3|Carolina|Silva|5/6/2018|Goiás|5300|NaN|15900|
|214|2962|HL9962|Android|1|Priscila|Garcia|7/29/2018|Goiás|3400|NaN|3400|
|215|2967|HL7348|SmartWatch|3|Guilherme|Seixas|1/11/2018|Goiás|1400|NaN|4200|
|216|2968|HL8851|Notebook|3|Arthur|Fernandes|9/9/2018|Goiás|3500|NaN|10500|
|217|2970|HL1918|iPhone|3|Mateus|Polastri|10/7/2018|Goiás|5300|NaN|15900|
|218|2985|HL1918|iPhone|3|Nicolas|Monteiro|5/10/2018|Goiás|5300|NaN|15900|
|219|2986|HL9962|Android|1|Lucas|Villanova|1/30/2018|Goiás|3400|NaN|3400|
|220|2992|HL1918|iPhone|4|Mateus|Duque|6/9/2018|Goiás|5300|NaN|21200|
|221|2995|HL1918|iPhone|4|Raphael|Machado|5/10/2018|Goiás|5300|NaN|21200|
|222|2999|HL1918|iPhone|1|Bruno|Mota|9/18/2018|Goiás|5300|NaN|5300|
|223|3011|HL4379|Televisão|2|Amanda|Machado|11/23/2018|Goiás|2500|NaN|5000|
|224|3033|HL2714|Tablet|2|Carlos|Barbosa|8/4/2018|Goiás|1600|NaN|3200|
|225|3055|HL4379|Televisão|3|Leandro|Rodrigues|4/21/2018|Goiás|2500|NaN|7500|
|226|3056|HL4379|Televisão|2|Roberto|Mattos|5/24/2018|Goiás|2500|NaN|5000|
|227|3078|HL4379|Televisão|3|Livia|Codeceira|11/7/2018|Goiás|2500|NaN|7500|
|228|3083|HL1918|iPhone|3|Danilo|Rubim|11/28/2018|Goiás|5300|NaN|15900|
|229|3111|HL9962|Android|3|Cícero|Lima|11/6/2018|Goiás|3400|NaN|10200|
|230|3114|HL1918|iPhone|5|Bruno|Silva|9/15/2018|Goiás|5300|NaN|26500|
|231|3139|HL1918|iPhone|1|João|Alves|2/9/2018|Goiás|5300|NaN|5300|
|232|3146|HL1918|iPhone|2|Cícero|Lima|12/18/2018|Goiás|5300|NaN|10600|
|233|3155|HL1918|iPhone|5|Mariana|Freire|6/24/2018|Goiás|5300|NaN|26500|
|234|3157|HL1918|iPhone|3|Kim|Ferreira|12/7/2018|Goiás|5300|NaN|15900|
|235|3166|HL1918|iPhone|1|Gabriel|Puntel|6/29/2018|Goiás|5300|NaN|5300|
|236|3170|HL1918|iPhone|2|Julia|Silva|5/24/2018|Goiás|5300|NaN|10600|
|237|3179|HL4379|Televisão|1|Julia|Leig|12/17/2018|Goiás|2500|NaN|2500|
|238|3202|HL1918|iPhone|3|Carlos|Melo|11/14/2018|Goiás|5300|NaN|15900|
|239|3204|HL1918|iPhone|3|Bruno|Mota|4/7/2018|Goiás|5300|NaN|15900|
|240|3220|HL1918|iPhone|3|Eduardo|Veiga|7/30/2018|Goiás|5300|NaN|15900|
|241|3233|HL4379|Televisão|4|Gabriel|Soares|3/2/2018|Goiás|2500|NaN|10000|
|242|3282|HL4379|Televisão|2|Eric|Júnior|10/9/2018|Goiás|2500|NaN|5000|
|243|3284|HL1918|iPhone|2|Matheus|Gomes|8/10/2018|Goiás|5300|NaN|10600|
|244|3285|HL8851|Notebook|4|Luísa|Fonseca|7/25/2018|Goiás|3500|NaN|14000|
|245|3291|HL8851|Notebook|4|Guilherme|Lima|2/13/2018|Goiás|3500|NaN|14000|
|246|3298|HL4379|Televisão|2|Livia|Corrêa|7/10/2018|Goiás|2500|NaN|5000|
|247|3312|HL1918|iPhone|4|Gabriel|Assis|9/16/2018|Goiás|5300|NaN|21200|
|248|3334|HL2714|Tablet|1|Ana|Carvalho|2/2/2018|Goiás|1600|NaN|1600|
|249|3336|HL9962|Android|2|Sandy|Figueiredo|3/7/2018|Goiás|3400|NaN|6800|
|250|3343|HL9962|Android|2|Carlos|Melo|2/22/2018|Goiás|3400|NaN|6800|
|251|3352|HL1148|Câmera|3|Adriano|Silva|8/1/2018|Goiás|2100|NaN|6300|
|252|3356|HL1918|iPhone|2|Bruno|Oliveira|2/6/2018|Goiás|5300|NaN|10600|
|253|3408|HL7348|SmartWatch|5|João|Monteiro|11/26/2018|Goiás|1400|NaN|7000|
|254|3424|HL7348|SmartWatch|4|Fernanda|Figueiredo|3/28/2018|Goiás|1400|NaN|5600|
|255|3431|HL9962|Android|3|Eduardo|Lopes|5/24/2018|Goiás|3400|NaN|10200|
|256|3434|HL4379|Televisão|4|Amanda|Gontijo|3/24/2018|Goiás|2500|NaN|10000|
|257|3449|HL9962|Android|4|Ana|Carvalho|8/31/2018|Goiás|3400|NaN|13600|
|258|3459|HL1918|iPhone|3|Luiza|Farias|3/27/2018|Goiás|5300|NaN|15900|
|259|3471|HL7348|SmartWatch|1|Bernard|Pedrosa|7/18/2018|Goiás|1400|NaN|1400|
|260|3511|HL1918|iPhone|5|Rafaela|Gomes|7/25/2018|Goiás|5300|NaN|26500|
|261|3521|HL1918|iPhone|3|Juan|Barbosa|4/15/2018|Goiás|5300|NaN|15900|
|262|3522|HL1148|Câmera|4|Wen|Braga|12/8/2018|Goiás|2100|NaN|8400|
|263|3539|HL1148|Câmera|4|Guilherme|Monteiro|12/17/2018|Goiás|2100|NaN|8400|
|264|3553|HL1918|iPhone|4|Mariane|Ferreira|11/12/2018|Goiás|5300|NaN|21200|
|265|3556|HL1918|iPhone|1|Sylvio|Bernhardt|1/14/2018|Goiás|5300|NaN|5300|
|266|3570|HL1148|Câmera|3|José|Jesus|8/30/2018|Goiás|2100|NaN|6300|
|267|3572|HL7348|SmartWatch|2|Luiza|Johnson|8/25/2018|Goiás|1400|NaN|2800|
|268|3579|HL1918|iPhone|3|Wendela|Veloso|5/4/2018|Goiás|5300|NaN|15900|
|269|3587|HL1918|iPhone|2|Melissa|Nucci|10/15/2018|Goiás|5300|NaN|10600|
|270|3593|HL1918|iPhone|3|Roberto|Nogueira|10/18/2018|Goiás|5300|NaN|15900|
|271|3600|HL1918|iPhone|5|Felipe|Cavalcanti|10/24/2018|Goiás|5300|NaN|26500|
|272|3605|HL1918|iPhone|4|Bruno|Barcessat|7/10/2018|Goiás|5300|NaN|21200|
|273|3612|HL4379|Televisão|1|Juliana|Pacheco|2/15/2018|Goiás|2500|NaN|2500|
|274|3628|HL9962|Android|5|Luiza|Cavalcanti|5/19/2018|Goiás|3400|NaN|17000|
|275|3651|HL4379|Televisão|4|Giulia|Lopes|11/22/2018|Goiás|2500|NaN|10000|
|276|3661|HL1148|Câmera|3|Norman|Jimbo|4/29/2018|Goiás|2100|NaN|6300|
|277|3670|HL1918|iPhone|2|Gabriella|Lopes|1/9/2018|Goiás|5300|NaN|10600|
|278|3674|HL7348|SmartWatch|4|Gabriella|Lopes|3/19/2018|Goiás|1400|NaN|5600|
|279|3677|HL9962|Android|2|Maria|Junior|5/6/2018|Goiás|3400|NaN|6800|
|280|3701|HL1918|iPhone|3|Ana|Felippe|1/20/2018|Goiás|5300|NaN|15900|
|281|3708|HL1918|iPhone|5|Isabel|Mesquita|12/5/2018|Goiás|5300|NaN|26500|
|282|3712|HL1918|iPhone|4|Bruna|Chein|3/17/2018|Goiás|5300|NaN|21200|
|283|3727|HL1918|iPhone|2|Raphael|Kurtz|7/15/2018|Goiás|5300|NaN|10600|
|284|3728|HL2714|Tablet|3|Pedro|Santos|8/16/2018|Goiás|1600|NaN|4800|
|285|3754|HL1918|iPhone|4|Andre|Nóbrega|12/26/2018|Goiás|5300|NaN|21200|
|286|3757|HL1918|iPhone|2|Henrique|Villanova|4/29/2018|Goiás|5300|NaN|10600|
|287|3758|HL1918|iPhone|3|Felipe|Cavalcanti|8/16/2018|Goiás|5300|NaN|15900|
|288|3775|HL4379|Televisão|5|Larissa|Cruz|6/30/2018|Goiás|2500|NaN|12500|
|289|3776|HL7348|SmartWatch|5|João|Monteiro|6/29/2018|Goiás|1400|NaN|7000|
|290|3783|HL7348|SmartWatch|5|Lenon|Fernandes|2/24/2018|Goiás|1400|NaN|7000|
|291|3786|HL4379|Televisão|2|Julia|Figueiredo|11/13/2018|Goiás|2500|NaN|5000|
|292|3792|HL4379|Televisão|1|Priscila|Carvalho|3/13/2018|Goiás|2500|NaN|2500|
|293|3813|HL9962|Android|2|Maria|Mello|7/20/2018|Goiás|3400|NaN|6800|
|294|3822|HL8851|Notebook|5|Kimberly|Sad|2/20/2018|Goiás|3500|NaN|17500|
|295|3836|HL4379|Televisão|5|Daniela|Pereira|12/2/2018|Goiás|2500|NaN|12500|
|296|3849|HL8851|Notebook|1|Guilherme|Merotto|11/6/2018|Goiás|3500|NaN|3500|
|297|3855|HL7348|SmartWatch|5|Audir|Franco|7/20/2018|Goiás|1400|NaN|7000|
|298|3883|HL1918|iPhone|2|Lucas|Almeida|6/13/2018|Goiás|5300|NaN|10600|
|299|3889|HL9962|Android|2|Jéssica|Stefanelli|3/16/2018|Goiás|3400|NaN|6800|
|300|3913|HL8851|Notebook|3|Daniel|Cardoso|7/9/2018|Goiás|3500|NaN|10500|
|301|3920|HL1918|iPhone|2|Ana|Miura|5/13/2018|Goiás|5300|NaN|10600|
|302|3959|HL1918|iPhone|2|Carolina|Carneiro|12/8/2018|Goiás|5300|NaN|10600|
|303|4006|HL8851|Notebook|5|Maria|Gasperi|9/19/2018|Goiás|3500|NaN|17500|
|304|4042|HL1918|iPhone|4|Thomáz|Vannier|5/13/2018|Goiás|5300|NaN|21200|
|305|4050|HL1148|Câmera|4|Rodrigo|Ramos|1/10/2018|Goiás|2100|NaN|8400|
|306|4053|HL7348|SmartWatch|1|Larissa|Nauenberg|5/25/2018|Goiás|1400|NaN|1400|
|307|4054|HL8851|Notebook|1|Victor|Lira|5/8/2018|Goiás|3500|NaN|3500|
|308|4055|HL2714|Tablet|2|Wilson|Brandão|8/26/2018|Goiás|1600|NaN|3200|
|309|4063|HL1918|iPhone|1|Wen|Braga|5/9/2018|Goiás|5300|NaN|5300|
|310|4078|HL2714|Tablet|1|Ives|Teixeira|6/29/2018|Goiás|1600|NaN|1600|
|311|4087|HL4379|Televisão|3|Ana|Leite|9/24/2018|Goiás|2500|NaN|7500|
|312|4115|HL4379|Televisão|2|Bruno|Velucci|7/12/2018|Goiás|2500|NaN|5000|
|313|4129|HL1918|iPhone|1|Arthur|Fernandes|10/6/2018|Goiás|5300|NaN|5300|
|314|4131|HL1918|iPhone|1|Vanessa|Bach|2/15/2018|Goiás|5300|NaN|5300|
|315|4136|HL7348|SmartWatch|2|Philipe|Morete|10/7/2018|Goiás|1400|NaN|2800|
|316|4140|HL4379|Televisão|2|Norman|Jimbo|6/7/2018|Goiás|2500|NaN|5000|
|317|4153|HL9962|Android|1|Priscila|Vogel|6/13/2018|Goiás|3400|NaN|3400|
|318|4198|HL2714|Tablet|3|Stephanie|Oliveira|5/3/2018|Goiás|1600|NaN|4800|
|319|4207|HL2714|Tablet|4|Milena|Alcoforado|1/6/2018|Goiás|1600|NaN|6400|
|320|4216|HL1918|iPhone|2|Rodrigo|Feijo|3/22/2018|Goiás|5300|NaN|10600|
|321|4229|HL4379|Televisão|5|Andre|Sampaio|12/4/2018|Goiás|2500|NaN|12500|
|322|4241|HL8851|Notebook|2|Diego|Marchesi|2/27/2018|Goiás|3500|NaN|7000|
|323|4245|HL7348|SmartWatch|1|Ana|Monte|5/6/2018|Goiás|1400|NaN|1400|
|324|4250|HL8851|Notebook|3|Beatriz|Cavalcanti|6/5/2018|Goiás|3500|NaN|10500|
|325|4258|HL9962|Android|1|Breno|Varella|1/23/2018|Goiás|3400|NaN|3400|
|326|4269|HL1148|Câmera|5|Amanda|Roberto|11/29/2018|Goiás|2100|NaN|10500|
|327|4314|HL1148|Câmera|1|Igor|Lima|6/14/2018|Goiás|2100|NaN|2100|
|328|4324|HL4379|Televisão|5|Bianca|Ferezin|8/1/2018|Goiás|2500|NaN|12500|
|329|4329|HL7348|SmartWatch|5|Renan|Melo|5/3/2018|Goiás|1400|NaN|7000|
|330|4349|HL7348|SmartWatch|3|Carolina|Siqueira|4/17/2018|Goiás|1400|NaN|4200|
|331|4358|HL4379|Televisão|5|Yasmim|Verly|12/10/2018|Goiás|2500|NaN|12500|
|332|4361|HL2714|Tablet|3|Fernanda|Coutinho|8/14/2018|Goiás|1600|NaN|4800|
|333|4381|HL8851|Notebook|1|Bruno|Oliveira|9/10/2018|Goiás|3500|NaN|3500|
|334|4386|HL9962|Android|2|Leandro|Ferreira|7/23/2018|Goiás|3400|NaN|6800|
|335|4395|HL1918|iPhone|3|Raul|Junqueira|10/28/2018|Goiás|5300|NaN|15900|
|336|4403|HL1918|iPhone|3|Stephanie|Gonçalves|4/27/2018|Goiás|5300|NaN|15900|
|337|4414|HL1918|iPhone|3|Victor|Soares|4/22/2018|Goiás|5300|NaN|15900|
|338|4415|HL1918|iPhone|5|Arthur|Rocha|2/5/2018|Goiás|5300|NaN|26500|
|339|4431|HL4379|Televisão|2|Priscila|Garcia|4/5/2018|Goiás|2500|NaN|5000|
|340|4452|HL1148|Câmera|5|Juliana|Silva|12/15/2018|Goiás|2100|NaN|10500|
|341|4461|HL4379|Televisão|4|Luana|Santos|2/23/2018|Goiás|2500|NaN|10000|
|342|4463|HL2714|Tablet|2|Caio|Moura|10/11/2018|Goiás|1600|NaN|3200|
|343|4486|HL9962|Android|5|Raíssa|Oliveira|8/26/2018|Goiás|3400|NaN|17000|
|344|4509|HL1918|iPhone|3|Guilherme|Rachide|7/16/2018|Goiás|5300|NaN|15900|
|345|4510|HL2714|Tablet|5|Lorena|Kohn|10/4/2018|Goiás|1600|NaN|8000|
|346|4520|HL4379|Televisão|1|Raphael|Coelho|8/26/2018|Goiás|2500|NaN|2500|
|347|4528|HL9962|Android|2|Maria|Junior|12/24/2018|Goiás|3400|NaN|6800|
|348|4534|HL1918|iPhone|1|Myllena|Corrêa|6/12/2018|Goiás|5300|NaN|5300|
|349|4545|HL4379|Televisão|1|Anna|Silva|9/15/2018|Goiás|2500|NaN|2500|
|350|4546|HL1148|Câmera|2|Bianca|Paz|9/7/2018|Goiás|2100|NaN|4200|
|351|4548|HL4379|Televisão|1|William|Mendonça|3/9/2018|Goiás|2500|NaN|2500|
|352|4563|HL7348|SmartWatch|3|Raíssa|Nimer|11/16/2018|Goiás|1400|NaN|4200|
|353|4581|HL2714|Tablet|1|Fernanda|Rubim|10/11/2018|Goiás|1600|NaN|1600|
|354|4625|HL1148|Câmera|1|Gabriela|Mello|12/1/2018|Goiás|2100|NaN|2100|
|355|4635|HL7348|SmartWatch|3|Anna|Figueiredo|4/13/2018|Goiás|1400|NaN|4200|
|356|4636|HL1918|iPhone|1|Fernanda|Rubim|1/4/2018|Goiás|5300|NaN|5300|
|357|4641|HL9962|Android|4|Gabriel|Soares|9/2/2018|Goiás|3400|NaN|13600|
|358|4649|HL7348|SmartWatch|1|Karina|Camara|11/18/2018|Goiás|1400|NaN|1400|
|359|4680|HL1918|iPhone|5|Lucas|Fontoura|7/20/2018|Goiás|5300|NaN|26500|
|360|4681|HL1918|iPhone|5|João|Júnior|9/3/2018|Goiás|5300|NaN|26500|
|361|4690|HL4379|Televisão|3|Deysiane|Bach|4/9/2018|Goiás|2500|NaN|7500|
|362|4707|HL9962|Android|4|Marina|Miranda|7/17/2018|Goiás|3400|NaN|13600|
|363|4721|HL1918|iPhone|1|Ylana|Teraoka|1/15/2018|Goiás|5300|NaN|5300|
|364|4771|HL8851|Notebook|2|Norman|Jimbo|5/4/2018|Goiás|3500|NaN|7000|
|365|4785|HL1918|iPhone|5|João|Costa|8/14/2018|Goiás|5300|NaN|26500|
|366|4787|HL7348|SmartWatch|3|Matheus|Delgado|7/19/2018|Goiás|1400|NaN|4200|
|367|4792|HL1918|iPhone|1|Pedro|Costa|3/28/2018|Goiás|5300|NaN|5300|
|368|4795|HL7348|SmartWatch|3|Fernanda|Silva|12/26/2018|Goiás|1400|NaN|4200|
|369|4835|HL8851|Notebook|4|Caio|Silva|11/8/2018|Goiás|3500|NaN|14000|
|370|4848|HL4379|Televisão|5|Sthefeson|Kohn|3/12/2018|Goiás|2500|NaN|12500|
|371|4864|HL1918|iPhone|5|Luiz|Conceição|12/19/2018|Goiás|5300|NaN|26500|
|372|4873|HL2714|Tablet|5|Alvaro|Kranz|4/6/2018|Goiás|1600|NaN|8000|
|373|4886|HL2714|Tablet|1|Hércules|Moreira|6/19/2018|Goiás|1600|NaN|1600|
|374|4887|HL9962|Android|5|Roberta|Nogueira|4/21/2018|Goiás|3400|NaN|17000|
|375|4891|HL4379|Televisão|5|Pedro|Costa|5/27/2018|Goiás|2500|NaN|12500|
|376|4902|HL1918|iPhone|2|Juliana|Goes|3/2/2018|Goiás|5300|NaN|10600|
|377|4909|HL8851|Notebook|3|Thales|Gouvêa|2/20/2018|Goiás|3500|NaN|10500|
|378|4916|HL2714|Tablet|3|Renan|Ventura|11/25/2018|Goiás|1600|NaN|4800|
|379|4919|HL4379|Televisão|2|Luis|Garcia|12/24/2018|Goiás|2500|NaN|5000|
|380|4937|HL7348|SmartWatch|4|João|Castilho|9/29/2018|Goiás|1400|NaN|5600|
|381|4979|HL8851|Notebook|4|Willian|Albino|12/6/2018|Goiás|3500|NaN|14000|
|382|5002|HL1148|Câmera|2|Thays|Castro|11/3/2018|Goiás|2100|NaN|4200|
|383|5006|HL4379|Televisão|3|Rafael|Rocha|10/6/2018|Goiás|2500|NaN|7500|
|384|5007|HL4379|Televisão|3|Priscila|Carvalho|12/20/2018|Goiás|2500|NaN|7500|
|385|5019|HL4379|Televisão|2|Luíza|Garcia|7/21/2018|Goiás|2500|NaN|5000|
|386|5034|HL4379|Televisão|3|Laís|Oliveira|8/6/2018|Goiás|2500|NaN|7500|
|387|5035|HL4379|Televisão|3|Danilo|Rubim|2/5/2018|Goiás|2500|NaN|7500|
|388|5036|HL4379|Televisão|5|Pedro|Santos|7/23/2018|Goiás|2500|NaN|12500|
|389|5037|HL1148|Câmera|5|Raphael|Filho|5/18/2018|Goiás|2100|NaN|10500|
|390|5070|HL4379|Televisão|3|Juliana|Pacheco|2/18/2018|Goiás|2500|NaN|7500|
|391|5090|HL7348|SmartWatch|3|Antonio|Manhães|7/7/2018|Goiás|1400|NaN|4200|
|392|5093|HL7348|SmartWatch|2|Eduardo|Vargas|1/8/2018|Goiás|1400|NaN|2800|
|393|5125|HL9962|Android|1|Felipe|Jorge|9/6/2018|Goiás|3400|NaN|3400|
|394|5161|HL1148|Câmera|3|Lais|Candido|7/19/2018|Goiás|2100|NaN|6300|
|395|5163|HL9962|Android|4|Mateus|Polastri|9/23/2018|Goiás|3400|NaN|13600|
|396|5170|HL1148|Câmera|3|Victor|Ferreira|9/19/2018|Goiás|2100|NaN|6300|
|397|5182|HL1918|iPhone|4|Matheus|Miranda|9/5/2018|Goiás|5300|NaN|21200|
|398|5203|HL1148|Câmera|2|Luíza|Melo|5/21/2018|Goiás|2100|NaN|4200|
|399|5207|HL1918|iPhone|1|Yasmim|Bittencourt|9/4/2018|Goiás|5300|NaN|5300|
|400|5226|HL1148|Câmera|4|Rodrigo|Feijo|3/9/2018|Goiás|2100|NaN|8400|
|401|5228|HL1918|iPhone|3|Caio|Moraes|10/22/2018|Goiás|5300|NaN|15900|
|402|5239|HL2714|Tablet|3|Eduardo|Quindeler|11/9/2018|Goiás|1600|NaN|4800|
|403|5252|HL2714|Tablet|5|Alexandre|Dantas|7/2/2018|Goiás|1600|NaN|8000|
|404|5254|HL8851|Notebook|2|Victor|Zakhm|7/27/2018|Goiás|3500|NaN|7000|
|405|5257|HL1148|Câmera|5|Wilson|Miranda|5/21/2018|Goiás|2100|NaN|10500|
|406|5260|HL8851|Notebook|2|Maria|Mello|4/9/2018|Goiás|3500|NaN|7000|
|407|5277|HL8851|Notebook|3|Raísa|Rodrigues|11/9/2018|Goiás|3500|NaN|10500|
|408|5291|HL4379|Televisão|3|Daniel|Monteiro|1/25/2018|Goiás|2500|NaN|7500|
|409|5293|HL7348|SmartWatch|2|Caio|Affonso|8/9/2018|Goiás|1400|NaN|2800|
|410|5295|HL1918|iPhone|3|Nina|Magalhães|8/14/2018|Goiás|5300|NaN|15900|
|411|5316|HL1148|Câmera|3|Isabela|Chagas|9/10/2018|Goiás|2100|NaN|6300|
|412|5352|HL1918|iPhone|1|Jéssica|Resinente|2/4/2018|Goiás|5300|NaN|5300|
|413|5360|HL1918|iPhone|5|Aline|Andrade|10/4/2018|Goiás|5300|NaN|26500|
|414|5361|HL2714|Tablet|3|Rachel|Restum|12/19/2018|Goiás|1600|NaN|4800|
|415|5375|HL1148|Câmera|4|João|Araujo|11/3/2018|Goiás|2100|NaN|8400|
|416|5376|HL8851|Notebook|4|Thayna|Martins|6/19/2018|Goiás|3500|NaN|14000|
|417|5377|HL9962|Android|3|Milena|Alcoforado|5/23/2018|Goiás|3400|NaN|10200|
|418|5398|HL1918|iPhone|4|Jônatas|Soares|4/16/2018|Goiás|5300|NaN|21200|
|419|5410|HL1918|iPhone|2|Daniel|Sousa|11/5/2018|Goiás|5300|NaN|10600|
|420|5411|HL1918|iPhone|5|Nina|Magalhães|9/19/2018|Goiás|5300|NaN|26500|
|421|5419|HL1918|iPhone|4|Leticia|Mesquita|1/2/2018|Goiás|5300|NaN|21200|
|422|5422|HL4379|Televisão|5|Pedro|Dalforne|1/28/2018|Goiás|2500|NaN|12500|
|423|5427|HL9962|Android|2|Anderson|Cavalcanti|11/19/2018|Goiás|3400|NaN|6800|
|424|5432|HL4379|Televisão|5|Miguel|Carneiro|1/8/2018|Goiás|2500|NaN|12500|
|425|5439|HL9962|Android|1|Henrique|Lencastre|4/16/2018|Goiás|3400|NaN|3400|
|426|5487|HL1148|Câmera|3|Luíza|Garcia|10/15/2018|Goiás|2100|NaN|6300|
|427|5515|HL1918|iPhone|4|Luíza|Goulart|2/14/2018|Goiás|5300|NaN|21200|
|428|5525|HL1918|iPhone|3|Rafaela|Gomes|6/20/2018|Goiás|5300|NaN|15900|
|429|5543|HL1918|iPhone|3|Bianca|Allevato|8/22/2018|Goiás|5300|NaN|15900|
|430|5553|HL1148|Câmera|3|Ana|Michetti|6/13/2018|Goiás|2100|NaN|6300|
|431|5578|HL1918|iPhone|5|Gabriella|Sagrillo|4/3/2018|Goiás|5300|NaN|26500|
|432|5599|HL4379|Televisão|4|Lara|Moreira|2/9/2018|Goiás|2500|NaN|10000|
|433|5605|HL7348|SmartWatch|1|Beatriz|Almeida|10/23/2018|Goiás|1400|NaN|1400|
|434|5609|HL7348|SmartWatch|2|Gabriela|Cavalcanti|6/8/2018|Goiás|1400|NaN|2800|
|435|5618|HL1148|Câmera|3|Camilla|Cardeman|3/27/2018|Goiás|2100|NaN|6300|
|436|5620|HL7348|SmartWatch|4|Luã|Sá|12/29/2018|Goiás|1400|NaN|5600|
|437|5622|HL4379|Televisão|2|Sthefeson|Pereira|1/5/2018|Goiás|2500|NaN|5000|
|438|5624|HL1148|Câmera|4|Lais|Candido|4/22/2018|Goiás|2100|NaN|8400|
|439|5644|HL7348|SmartWatch|3|Rilson|Dias|12/28/2018|Goiás|1400|NaN|4200|
|440|5649|HL8851|Notebook|5|Luiza|Procaci|5/19/2018|Goiás|3500|NaN|17500|
|441|5660|HL8851|Notebook|5|Sandy|Figueiredo|9/6/2018|Goiás|3500|NaN|17500|
|442|5680|HL4379|Televisão|1|Beatriz|Nogueira|9/28/2018|Goiás|2500|NaN|2500|
|443|5765|HL1148|Câmera|2|Breno|Varella|6/14/2018|Goiás|2100|NaN|4200|
|444|5809|HL1148|Câmera|1|Myllena|Corrêa|1/24/2018|Goiás|2100|NaN|2100|
|445|5855|HL4379|Televisão|2|Gabriel|Puntel|7/4/2018|Goiás|2500|NaN|5000|
|446|5875|HL8851|Notebook|4|Wilson|Farias|4/12/2018|Goiás|3500|NaN|14000|
|447|5894|HL9962|Android|4|Marcelo|Guadagnino|5/6/2018|Goiás|3400|NaN|13600|
|448|5919|HL1148|Câmera|1|Michelle|Miura|10/12/2018|Goiás|2100|NaN|2100|
|449|5928|HL1918|iPhone|4|Gustavo|Thome|6/13/2018|Goiás|5300|NaN|21200|
|450|5942|HL7348|SmartWatch|1|Roberta|Teixeira|8/6/2018|Goiás|1400|NaN|1400|
|451|5961|HL8851|Notebook|1|Marcelo|Pereira|6/9/2018|Goiás|3500|NaN|3500|
|452|5973|HL9962|Android|3|Arthur|Rocha|3/21/2018|Goiás|3400|NaN|10200|
|453|5979|HL1148|Câmera|5|Beatriz|Almeida|1/3/2018|Goiás|2100|NaN|10500|
|454|6010|HL1918|iPhone|5|Carolina|Abrahão|10/29/2018|Goiás|5300|NaN|26500|
|455|6031|HL4379|Televisão|4|Caroll|Johnson|1/16/2018|Goiás|2500|NaN|10000|
|456|6062|HL1918|iPhone|4|Thales|Gouvêa|5/11/2018|Goiás|5300|NaN|21200|
|457|6080|HL1918|iPhone|3|João|Júnior|12/19/2018|Goiás|5300|NaN|15900|
|458|6092|HL1918|iPhone|2|Diego|Marchesi|3/1/2018|Goiás|5300|NaN|10600|
|459|6116|HL4379|Televisão|2|Raul|Junqueira|12/23/2018|Goiás|2500|NaN|5000|
|460|6120|HL4379|Televisão|2|Jônatas|Soares|5/22/2018|Goiás|2500|NaN|5000|
|461|6139|HL1148|Câmera|1|João|Menezes|1/31/2018|Goiás|2100|NaN|2100|
|462|6144|HL2714|Tablet|5|Anderson|Cavalcanti|4/8/2018|Goiás|1600|NaN|8000|
|463|6159|HL1918|iPhone|5|Thiago|Lima|9/16/2018|Goiás|5300|NaN|26500|
|464|6177|HL4379|Televisão|1|Beatriz|Silva|4/14/2018|Goiás|2500|NaN|2500|
|465|6202|HL1918|iPhone|2|Isabela|Rodrigues|9/8/2018|Goiás|5300|NaN|10600|
|466|6219|HL1918|iPhone|4|Mônica|Rotolo|1/15/2018|Goiás|5300|NaN|21200|
|467|6242|HL7348|SmartWatch|5|Jeferson|Costa|3/20/2018|Goiás|1400|NaN|7000|
|468|6274|HL1918|iPhone|4|Lucas|Villanova|3/27/2018|Goiás|5300|NaN|21200|
|469|6275|HL4379|Televisão|5|Lucas|Monte|8/11/2018|Goiás|2500|NaN|12500|
|470|6284|HL9962|Android|1|Ana|Silva|10/5/2018|Goiás|3400|NaN|3400|
|471|6295|HL4379|Televisão|1|Lívia|Tanaka|6/12/2018|Goiás|2500|NaN|2500|
|472|6302|HL4379|Televisão|3|Lucas|Freitas|6/30/2018|Goiás|2500|NaN|7500|
|473|6326|HL4379|Televisão|4|Pedro|Conceição|5/14/2018|Goiás|2500|NaN|10000|
|474|6336|HL7348|SmartWatch|5|Debora|Silva|6/12/2018|Goiás|1400|NaN|7000|
|475|6341|HL1148|Câmera|4|Rodrigo|Mendes|7/20/2018|Goiás|2100|NaN|8400|
|476|6366|HL9962|Android|5|Stefan|Nunes|11/12/2018|Goiás|3400|NaN|17000|
|477|6370|HL4379|Televisão|1|Daniela|Rosa|1/13/2018|Goiás|2500|NaN|2500|
|478|6373|HL4379|Televisão|4|Breno|Costa|3/3/2018|Goiás|2500|NaN|10000|
|479|6378|HL2714|Tablet|1|Thiago|Nóbrega|11/5/2018|Goiás|1600|NaN|1600|
|480|6401|HL4379|Televisão|5|Henrique|Lencastre|5/7/2018|Goiás|2500|NaN|12500|
|481|6404|HL4379|Televisão|1|Jônatas|Tanaka|8/23/2018|Goiás|2500|NaN|2500|
|482|6423|HL4379|Televisão|5|Thayane|Resende|4/23/2018|Goiás|2500|NaN|12500|
|483|6436|HL2714|Tablet|2|Myllena|Corrêa|8/27/2018|Goiás|1600|NaN|3200|
|484|6454|HL1918|iPhone|4|Thaís|Ribeiro|8/29/2018|Goiás|5300|NaN|21200|
|485|6456|HL9962|Android|3|Marina|Aragão|9/30/2018|Goiás|3400|NaN|10200|
|486|6467|HL4379|Televisão|2|Michelle|Miura|8/14/2018|Goiás|2500|NaN|5000|
|487|6471|HL2714|Tablet|4|Eric|Carvalho|6/2/2018|Goiás|1600|NaN|6400|
|488|6486|HL8851|Notebook|4|Guilherme|Jordao|1/6/2018|Goiás|3500|NaN|14000|
|489|6492|HL4379|Televisão|5|Isabela|Rodrigues|10/25/2018|Goiás|2500|NaN|12500|
|490|6503|HL4379|Televisão|5|Ives|Teixeira|10/23/2018|Goiás|2500|NaN|12500|
|491|6523|HL7348|SmartWatch|5|Gabriela|Aliani|8/15/2018|Goiás|1400|NaN|7000|
|492|6533|HL9962|Android|2|Isabela|Rodrigues|11/13/2018|Goiás|3400|NaN|6800|
|493|6542|HL4379|Televisão|4|Gabriela|Mello|12/26/2018|Goiás|2500|NaN|10000|
|494|6544|HL1918|iPhone|4|Thales|Portillo|11/7/2018|Goiás|5300|NaN|21200|
|495|6612|HL1148|Câmera|5|Clara|Bruno|5/22/2018|Goiás|2100|NaN|10500|
|496|6640|HL1918|iPhone|4|Izabel|Miura|1/3/2018|Goiás|5300|NaN|21200|
|497|6693|HL8851|Notebook|3|Mateus|Franco|2/25/2018|Goiás|3500|NaN|10500|
|498|6697|HL1918|iPhone|5|Mariana|Barrozo|10/3/2018|Goiás|5300|NaN|26500|
|499|6700|HL2714|Tablet|5|Amanda|Gontijo|3/1/2018|Goiás|1600|NaN|8000|
|500|6714|HL1918|iPhone|4|Rafael|Guimarães|10/25/2018|Goiás|5300|NaN|21200|
|501|6737|HL7348|SmartWatch|3|Philipe|Morete|1/4/2018|Goiás|1400|NaN|4200|
|502|6752|HL2714|Tablet|4|Sandy|Figueiredo|8/6/2018|Goiás|1600|NaN|6400|
|503|6754|HL7348|SmartWatch|4|Maria|Mello|1/27/2018|Goiás|1400|NaN|5600|
|504|6756|HL2714|Tablet|5|Bernardo|Nauenberg|10/17/2018|Goiás|1600|NaN|8000|
|505|6767|HL1918|iPhone|2|Thayane|Resende|7/17/2018|Goiás|5300|NaN|10600|
|506|6769|HL4379|Televisão|4|Juan|Fernandes|11/25/2018|Goiás|2500|NaN|10000|
|507|6812|HL2714|Tablet|1|Luiza|Marques|11/11/2018|Goiás|1600|NaN|1600|
|508|6816|HL4379|Televisão|3|Viviane|Cunha|11/26/2018|Goiás|2500|NaN|7500|
|509|6864|HL9962|Android|2|Thais|Rodrigues|4/24/2018|Goiás|3400|NaN|6800|
|510|6870|HL1918|iPhone|2|Lucas|Reis|2/18/2018|Goiás|5300|NaN|10600|
|511|6883|HL9962|Android|1|Diego|Rodrigues|12/16/2018|Goiás|3400|NaN|3400|
|512|6930|HL9962|Android|5|Luana|Santana|7/25/2018|Goiás|3400|NaN|17000|
|513|6949|HL1918|iPhone|4|Gabriel|Puntel|1/31/2018|Goiás|5300|NaN|21200|
|514|6968|HL8851|Notebook|1|Luiza|Procaci|5/15/2018|Goiás|3500|NaN|3500|
|515|6976|HL4379|Televisão|3|Felipe|Mello|11/5/2018|Goiás|2500|NaN|7500|
|516|6988|HL9962|Android|1|Natalia|Marinho|1/10/2018|Goiás|3400|NaN|3400|
|517|6991|HL4379|Televisão|2|Matheus|Miranda|7/17/2018|Goiás|2500|NaN|5000|
|518|6994|HL1918|iPhone|2|Luísa|Fonseca|6/20/2018|Goiás|5300|NaN|10600|
|519|6998|HL4379|Televisão|5|Renan|Melo|11/4/2018|Goiás|2500|NaN|12500|
|520|7006|HL4379|Televisão|5|Luiz|Almeida|3/20/2018|Goiás|2500|NaN|12500|
|521|7022|HL7348|SmartWatch|1|Luiza|Johnson|6/8/2018|Goiás|1400|NaN|1400|
|522|7051|HL4379|Televisão|2|Rodrigo|Ramos|6/22/2018|Goiás|2500|NaN|5000|
|523|7074|HL1148|Câmera|5|Rodrigo|Silva|7/19/2018|Goiás|2100|NaN|10500|
|524|7084|HL4379|Televisão|4|Carlos|Souza|5/13/2018|Goiás|2500|NaN|10000|
|525|7093|HL4379|Televisão|1|Isabel|Leite|10/30/2018|Goiás|2500|NaN|2500|
|526|7129|HL1148|Câmera|5|Luiza|Cabral|1/15/2018|Goiás|2100|NaN|10500|
|527|7141|HL1148|Câmera|3|Jonatas|Passos|5/19/2018|Goiás|2100|NaN|6300|
|528|7187|HL4379|Televisão|1|Breno|Godoy|3/9/2018|Goiás|2500|NaN|2500|
|529|7196|HL1918|iPhone|1|Izabel|Lopes|6/10/2018|Goiás|5300|NaN|5300|
|530|7202|HL1918|iPhone|2|Lucas|Junior|12/31/2018|Goiás|5300|NaN|10600|
|531|7222|HL1918|iPhone|3|Thaís|Moura|6/29/2018|Goiás|5300|NaN|15900|
|532|7229|HL7348|SmartWatch|2|Matheus|Ramos|7/15/2018|Goiás|1400|NaN|2800|
|533|7232|HL1918|iPhone|1|Juliana|Guimarães|11/27/2018|Goiás|5300|NaN|5300|
|534|7272|HL4379|Televisão|4|Lenon|Fernandes|4/19/2018|Goiás|2500|NaN|10000|
|535|7284|HL1918|iPhone|5|Jônatas|Tanaka|8/8/2018|Goiás|5300|NaN|26500|
|536|7296|HL7348|SmartWatch|4|Priscila|Suzano|3/2/2018|Goiás|1400|NaN|5600|
|537|7303|HL7348|SmartWatch|2|Lucas|Almeida|8/8/2018|Goiás|1400|NaN|2800|
|538|7319|HL4379|Televisão|5|Vitor|Boccaletti|9/17/2018|Goiás|2500|NaN|12500|
|539|7322|HL2714|Tablet|1|Ana|Carvalho|12/11/2018|Goiás|1600|NaN|1600|
|540|7347|HL1918|iPhone|2|Alex|Fernandes|6/21/2018|Goiás|5300|NaN|10600|
|541|7353|HL1918|iPhone|4|Guilherme|Lima|3/9/2018|Goiás|5300|NaN|21200|
|542|7363|HL1918|iPhone|5|João|Junior|4/8/2018|Goiás|5300|NaN|26500|
|543|7372|HL1918|iPhone|3|Milena|Almeida|12/2/2018|Goiás|5300|NaN|15900|
|544|7386|HL2714|Tablet|5|Jônatas|Soares|6/29/2018|Goiás|1600|NaN|8000|
|545|7395|HL1918|iPhone|2|Hércules|Júnior|11/9/2018|Goiás|5300|NaN|10600|
|546|7413|HL1918|iPhone|5|Marina|Marins|6/30/2018|Goiás|5300|NaN|26500|
|547|7423|HL1148|Câmera|4|João|Guadagnino|5/15/2018|Goiás|2100|NaN|8400|
|548|7444|HL4379|Televisão|1|Andre|Sampaio|12/23/2018|Goiás|2500|NaN|2500|
|549|7452|HL7348|SmartWatch|1|Wilson|Brandão|9/14/2018|Goiás|1400|NaN|1400|
|550|7462|HL4379|Televisão|3|Isabella|Montanholi|1/23/2018|Goiás|2500|NaN|7500|
|551|7490|HL1148|Câmera|3|Mariane|Ferreira|11/10/2018|Goiás|2100|NaN|6300|
|552|7502|HL1918|iPhone|1|Adriana|Carneiro|8/28/2018|Goiás|5300|NaN|5300|
|553|7528|HL7348|SmartWatch|4|Raissa|Sales|1/18/2018|Goiás|1400|NaN|5600|
|554|7538|HL8851|Notebook|4|Pedro|Conceição|12/22/2018|Goiás|3500|NaN|14000|
|555|7546|HL2714|Tablet|4|Luis|Garcia|2/3/2018|Goiás|1600|NaN|6400|
|556|7551|HL1918|iPhone|1|Bruno|Ursulino|5/7/2018|Goiás|5300|NaN|5300|
|557|7552|HL4379|Televisão|5|Lucas|Rocha|12/17/2018|Goiás|2500|NaN|12500|
|558|7571|HL1918|iPhone|3|Luana|Santos|6/28/2018|Goiás|5300|NaN|15900|
|559|7586|HL1918|iPhone|2|Nathan|Cunha|6/15/2018|Goiás|5300|NaN|10600|
|560|7593|HL1918|iPhone|2|Bruna|Rangel|4/5/2018|Goiás|5300|NaN|10600|
|561|7605|HL7348|SmartWatch|5|Kimberly|Sad|6/14/2018|Goiás|1400|NaN|7000|
|562|7609|HL9962|Android|1|Jônatas|Tanaka|9/10/2018|Goiás|3400|NaN|3400|
|563|7615|HL1918|iPhone|5|Izabel|Lopes|1/1/2018|Goiás|5300|NaN|26500|
|564|7618|HL7348|SmartWatch|2|Elaine|Santos|3/14/2018|Goiás|1400|NaN|2800|
|565|7628|HL4379|Televisão|4|Myllena|Corrêa|2/19/2018|Goiás|2500|NaN|10000|
|566|7631|HL7348|SmartWatch|5|Daniel|Costa|11/10/2018|Goiás|1400|NaN|7000|
|567|7642|HL1918|iPhone|4|Isabelle|Firmino|7/10/2018|Goiás|5300|NaN|21200|
|568|7663|HL2714|Tablet|4|Lucas|Valim|10/1/2018|Goiás|1600|NaN|6400|
|569|7669|HL1918|iPhone|3|Luana|Santana|9/10/2018|Goiás|5300|NaN|15900|
|570|7671|HL8851|Notebook|5|Thales|Andrade|5/8/2018|Goiás|3500|NaN|17500|
|571|7708|HL4379|Televisão|5|Alon|Pestana|6/13/2018|Goiás|2500|NaN|12500|
|572|7715|HL4379|Televisão|4|André|Alves|6/26/2018|Goiás|2500|NaN|10000|
|573|7728|HL1918|iPhone|3|Rodrigo|Alves|9/17/2018|Goiás|5300|NaN|15900|
|574|7747|HL7348|SmartWatch|1|Gabriel|Ribeiro|5/14/2018|Goiás|1400|NaN|1400|
|575|7748|HL1918|iPhone|3|Rebeca|Taylor|9/9/2018|Goiás|5300|NaN|15900|
|576|7752|HL8851|Notebook|4|Roberta|Teixeira|10/23/2018|Goiás|3500|NaN|14000|
|577|7776|HL1918|iPhone|5|Isabela|Resende|2/12/2018|Goiás|5300|NaN|26500|
|578|7782|HL7348|SmartWatch|2|Lucas|Valim|12/11/2018|Goiás|1400|NaN|2800|
|579|7797|HL9962|Android|3|Breno|Godoy|4/8/2018|Goiás|3400|NaN|10200|
|580|7811|HL9962|Android|2|Eduardo|Veiga|10/31/2018|Goiás|3400|NaN|6800|
|581|7836|HL1918|iPhone|3|João|Costa|2/16/2018|Goiás|5300|NaN|15900|
|582|7844|HL7348|SmartWatch|1|Guilherme|Assis|12/14/2018|Goiás|1400|NaN|1400|
|583|7849|HL1918|iPhone|2|Hanna|Fonseca|8/9/2018|Goiás|5300|NaN|10600|
|584|7855|HL8851|Notebook|1|Caroline|Aquino|5/28/2018|Goiás|3500|NaN|3500|
|585|7856|HL1918|iPhone|2|Maria|Assumpção|4/5/2018|Goiás|5300|NaN|10600|
|586|7875|HL1148|Câmera|5|Allan|Candido|2/10/2018|Goiás|2100|NaN|10500|
|587|7918|HL8851|Notebook|5|Raíza|Lopes|9/22/2018|Goiás|3500|NaN|17500|
|588|7929|HL4379|Televisão|3|Maria|Correa|6/22/2018|Goiás|2500|NaN|7500|
|589|7941|HL1148|Câmera|1|Carlos|Assis|5/15/2018|Goiás|2100|NaN|2100|
|590|7958|HL4379|Televisão|5|Pedro|Conceição|8/7/2018|Goiás|2500|NaN|12500|
|591|7961|HL1148|Câmera|5|Matheus|Gomes|2/9/2018|Goiás|2100|NaN|10500|
|592|7966|HL1148|Câmera|2|Raul|Silveira|1/21/2018|Goiás|2100|NaN|4200|
|593|7978|HL7348|SmartWatch|3|Bruno|Temporal|4/7/2018|Goiás|1400|NaN|4200|
|594|7981|HL4379|Televisão|1|Bruna|Silveira|11/1/2018|Goiás|2500|NaN|2500|
|595|7997|HL7348|SmartWatch|5|Wendela|Mariz|7/11/2018|Goiás|1400|NaN|7000|
|596|8000|HL1918|iPhone|4|Manuela|Merege|1/3/2018|Goiás|5300|NaN|21200|
|597|8018|HL1918|iPhone|3|Gabrielle|Figueiredo|2/6/2018|Goiás|5300|NaN|15900|
|598|8033|HL1918|iPhone|4|Ruan|Lopes|11/11/2018|Goiás|5300|NaN|21200|
|599|8109|HL7348|SmartWatch|2|Pedro|Cardoso|9/4/2018|Goiás|1400|NaN|2800|
|600|8112|HL1918|iPhone|1|Gabriella|Lopes|12/19/2018|Goiás|5300|NaN|5300|
|601|8116|HL4379|Televisão|5|Fernanda|Coutinho|8/16/2018|Goiás|2500|NaN|12500|
|602|8117|HL1918|iPhone|4|Rafael|Wajnsztok|11/6/2018|Goiás|5300|NaN|21200|
|603|8141|HL1918|iPhone|4|Antônio|Soares|9/17/2018|Goiás|5300|NaN|21200|
|604|8147|HL1918|iPhone|5|Raissa|Negrelli|3/31/2018|Goiás|5300|NaN|26500|
|605|8149|HL9962|Android|2|Giuseppe|Bhering|2/8/2018|Goiás|3400|NaN|6800|
|606|8160|HL9962|Android|2|Luísa|Fonseca|2/23/2018|Goiás|3400|NaN|6800|
|607|8166|HL1918|iPhone|1|Thiago|Veiga|9/28/2018|Goiás|5300|NaN|5300|
|608|8171|HL7348|SmartWatch|4|Luiza|Ribeiro|10/9/2018|Goiás|1400|NaN|5600|
|609|8190|HL1918|iPhone|2|Guilherme|Santos|1/1/2018|Goiás|5300|NaN|10600|
|610|8220|HL1918|iPhone|2|Helena|Chafin|10/23/2018|Goiás|5300|NaN|10600|
|611|8263|HL4379|Televisão|5|Giulia|Lopes|4/12/2018|Goiás|2500|NaN|12500|
|612|8268|HL2714|Tablet|4|Ylana|Teraoka|6/5/2018|Goiás|1600|NaN|6400|
|613|8269|HL1148|Câmera|2|Ulisses|Quinto|9/5/2018|Goiás|2100|NaN|4200|
|614|8311|HL8851|Notebook|5|Daniel|Ortiz|1/13/2018|Goiás|3500|NaN|17500|
|615|8312|HL7348|SmartWatch|5|João|Matheus|8/26/2018|Goiás|1400|NaN|7000|
|616|8320|HL1918|iPhone|1|Isabel|Leite|4/30/2018|Goiás|5300|NaN|5300|
|617|8326|HL7348|SmartWatch|2|Julia|Teixeira|3/14/2018|Goiás|1400|NaN|2800|
|618|8342|HL1918|iPhone|5|Lorena|Carvalho|5/24/2018|Goiás|5300|NaN|26500|
|619|8355|HL1918|iPhone|2|Bianca|Allevato|8/7/2018|Goiás|5300|NaN|10600|
|620|8363|HL2714|Tablet|2|Carlos|Silva|1/6/2018|Goiás|1600|NaN|3200|
|621|8381|HL1918|iPhone|2|Carolina|Alfradique|6/15/2018|Goiás|5300|NaN|10600|
|622|8383|HL8851|Notebook|1|Anna|Maia|10/19/2018|Goiás|3500|NaN|3500|
|623|8386|HL9962|Android|5|Katharina|Barros|2/27/2018|Goiás|3400|NaN|17000|
|624|8389|HL8851|Notebook|5|Pedro|Macckione|8/2/2018|Goiás|3500|NaN|17500|
|625|8405|HL4379|Televisão|1|Maria|Mello|7/29/2018|Goiás|2500|NaN|2500|
|626|8416|HL4379|Televisão|3|Bruna|Silva|6/27/2018|Goiás|2500|NaN|7500|
|627|8423|HL4379|Televisão|3|Arthur|Portela|6/4/2018|Goiás|2500|NaN|7500|
|628|8428|HL9962|Android|5|Gabrielle|Viríssimo|11/29/2018|Goiás|3400|NaN|17000|
|629|8455|HL7348|SmartWatch|2|Luiz|Mendonça|4/18/2018|Goiás|1400|NaN|2800|
|630|8456|HL4379|Televisão|1|Samara|Pinto|6/7/2018|Goiás|2500|NaN|2500|
|631|8472|HL8851|Notebook|5|Victor|Lira|3/5/2018|Goiás|3500|NaN|17500|
|632|8476|HL4379|Televisão|2|Bianca|Piero|7/30/2018|Goiás|2500|NaN|5000|
|633|8511|HL1918|iPhone|5|Giovanna|Santos|5/6/2018|Goiás|5300|NaN|26500|
|634|8553|HL1918|iPhone|3|Victor|Gomes|11/1/2018|Goiás|5300|NaN|15900|
|635|8555|HL1148|Câmera|5|Fabio|Boccaletti|6/21/2018|Goiás|2100|NaN|10500|
|636|8561|HL1148|Câmera|5|Adriana|Passos|7/6/2018|Goiás|2100|NaN|10500|
|637|8589|HL2714|Tablet|5|Pedro|Macckione|10/27/2018|Goiás|1600|NaN|8000|
|638|8590|HL8851|Notebook|5|Leandro|Ferreira|12/15/2018|Goiás|3500|NaN|17500|
|639|8597|HL1918|iPhone|2|Guilherme|Monteiro|3/6/2018|Goiás|5300|NaN|10600|
|640|8613|HL1918|iPhone|2|Caio|Cardoso|2/6/2018|Goiás|5300|NaN|10600|
|641|8638|HL8851|Notebook|1|Sandy|Moreira|1/22/2018|Goiás|3500|NaN|3500|
|642|8652|HL4379|Televisão|3|Lucas|Neto|2/12/2018|Goiás|2500|NaN|7500|
|643|8655|HL2714|Tablet|4|Thiago|Nóbrega|1/23/2018|Goiás|1600|NaN|6400|
|644|8662|HL8851|Notebook|1|Thiago|Nóbrega|10/28/2018|Goiás|3500|NaN|3500|
|645|8681|HL9962|Android|2|Lucas|Baptista|7/26/2018|Goiás|3400|NaN|6800|
|646|8705|HL2714|Tablet|1|Luíza|Goulart|3/7/2018|Goiás|1600|NaN|1600|
|647|8706|HL2714|Tablet|5|Arthur|Souza|11/17/2018|Goiás|1600|NaN|8000|
|648|8709|HL1918|iPhone|3|João|Aires|7/26/2018|Goiás|5300|NaN|15900|
|649|8726|HL2714|Tablet|3|Beatriz|Silva|7/1/2018|Goiás|1600|NaN|4800|
|650|8730|HL2714|Tablet|3|Bruno|Salomão|12/25/2018|Goiás|1600|NaN|4800|
|651|8760|HL4379|Televisão|1|João|Castilho|2/6/2018|Goiás|2500|NaN|2500|
|652|8772|HL7348|SmartWatch|1|Guilherme|Marchesi|12/4/2018|Goiás|1400|NaN|1400|
|653|8781|HL4379|Televisão|3|Khaio|Mesquita|9/14/2018|Goiás|2500|NaN|7500|
|654|8795|HL1918|iPhone|3|Raul|Silveira|7/24/2018|Goiás|5300|NaN|15900|
|655|8822|HL9962|Android|2|Tadeu|Sousa|9/11/2018|Goiás|3400|NaN|6800|
|656|8829|HL7348|SmartWatch|5|Luiz|Xavier|12/16/2018|Goiás|1400|NaN|7000|
|657|8845|HL1148|Câmera|2|Stephanie|Novak|12/14/2018|Goiás|2100|NaN|4200|
|658|8850|HL1918|iPhone|2|Isabela|Teixeira|6/6/2018|Goiás|5300|NaN|10600|
|659|8860|HL1148|Câmera|1|Matheus|Santos|2/21/2018|Goiás|2100|NaN|2100|
|660|8864|HL8851|Notebook|2|Andre|Nóbrega|11/15/2018|Goiás|3500|NaN|7000|
|661|8865|HL4379|Televisão|4|Barbara|Procaci|8/15/2018|Goiás|2500|NaN|10000|
|662|8869|HL1148|Câmera|2|Henrique|Silva|10/30/2018|Goiás|2100|NaN|4200|
|663|8914|HL1918|iPhone|4|Renan|Nascimento|12/11/2018|Goiás|5300|NaN|21200|
|664|8916|HL1918|iPhone|5|Juliana|Souza|12/3/2018|Goiás|5300|NaN|26500|
|665|8930|HL1918|iPhone|3|Ylana|Teraoka|10/9/2018|Goiás|5300|NaN|15900|
|666|8932|HL9962|Android|5|Gabriela|Cavalcanti|9/20/2018|Goiás|3400|NaN|17000|
|667|8945|HL4379|Televisão|4|Raphael|Coelho|7/5/2018|Goiás|2500|NaN|10000|
|668|8959|HL9962|Android|3|Ana|Leite|10/23/2018|Goiás|3400|NaN|10200|
|669|8964|HL1918|iPhone|1|Stefan|Santos|8/24/2018|Goiás|5300|NaN|5300|
|670|8990|HL9962|Android|1|Deysiane|Medronho|7/14/2018|Goiás|3400|NaN|3400|
|671|8999|HL2714|Tablet|4|Raphael|Ferman|6/27/2018|Goiás|1600|NaN|6400|
|672|9004|HL1918|iPhone|3|Luiz|Freire|9/3/2018|Goiás|5300|NaN|15900|
|673|9023|HL4379|Televisão|3|Luiz|Almeida|12/29/2018|Goiás|2500|NaN|7500|
|674|9025|HL8851|Notebook|3|Cícero|Ramos|9/9/2018|Goiás|3500|NaN|10500|
|675|9029|HL4379|Televisão|1|Cassio|Faria|6/10/2018|Goiás|2500|NaN|2500|
|676|9091|HL1918|iPhone|5|Ana|Silva|3/25/2018|Goiás|5300|NaN|26500|
|677|9136|HL2714|Tablet|5|Diego|Rodrigues|11/16/2018|Goiás|1600|NaN|8000|
|678|9143|HL7348|SmartWatch|4|Luiza|Cabral|2/13/2018|Goiás|1400|NaN|5600|
|679|9144|HL1918|iPhone|5|Pedro|Costa|6/23/2018|Goiás|5300|NaN|26500|
|680|9151|HL1918|iPhone|2|Luis|Silva|10/19/2018|Goiás|5300|NaN|10600|
|681|9158|HL7348|SmartWatch|1|Elena|Barreto|9/19/2018|Goiás|1400|NaN|1400|
|682|9197|HL1148|Câmera|3|Ana|Felippe|4/11/2018|Goiás|2100|NaN|6300|
|683|9212|HL4379|Televisão|2|Danilo|Mendonça|10/8/2018|Goiás|2500|NaN|5000|
|684|9222|HL8851|Notebook|1|Rogério|Pereira|4/12/2018|Goiás|3500|NaN|3500|
|685|9227|HL1918|iPhone|3|Hanna|Fonseca|4/7/2018|Goiás|5300|NaN|15900|
|686|9231|HL2714|Tablet|1|Rafaela|Gomes|2/28/2018|Goiás|1600|NaN|1600|
|687|9252|HL7348|SmartWatch|1|Isabelle|Firmino|12/23/2018|Goiás|1400|NaN|1400|
|688|9290|HL1918|iPhone|5|Wendela|Veloso|9/5/2018|Goiás|5300|NaN|26500|
|689|9309|HL1918|iPhone|2|Victor|Gomes|6/22/2018|Goiás|5300|NaN|10600|
|690|9355|HL9962|Android|1|Glenda|Santos|10/15/2018|Goiás|3400|NaN|3400|
|691|9362|HL9962|Android|1|Juan|Fernandes|1/24/2018|Goiás|3400|NaN|3400|
|692|9373|HL1918|iPhone|1|Gabrielle|Figueiredo|7/25/2018|Goiás|5300|NaN|5300|
|693|9393|HL8851|Notebook|5|Gabriel|Assis|12/4/2018|Goiás|3500|NaN|17500|
|694|9395|HL8851|Notebook|1|Diego|Mello|5/27/2018|Goiás|3500|NaN|3500|
|695|9421|HL2714|Tablet|2|Joyce|Souza|5/16/2018|Goiás|1600|NaN|3200|
|696|9457|HL2714|Tablet|3|Carolina|Bernardes|7/23/2018|Goiás|1600|NaN|4800|
|697|9473|HL8851|Notebook|2|Daniel|Cardoso|3/4/2018|Goiás|3500|NaN|7000|
|698|9484|HL2714|Tablet|2|Gabriella|Lopes|8/24/2018|Goiás|1600|NaN|3200|
|699|9496|HL9962|Android|5|Isabella|Santos|5/30/2018|Goiás|3400|NaN|17000|
|700|9503|HL7348|SmartWatch|5|Willian|Albino|4/25/2018|Goiás|1400|NaN|7000|
|701|9520|HL1918|iPhone|5|Pedro|Ronfini|9/9/2018|Goiás|5300|NaN|26500|
|702|9552|HL4379|Televisão|5|Patrícia|Amaral|1/12/2018|Goiás|2500|NaN|12500|
|703|9554|HL1148|Câmera|4|Julie|Ferreira|1/26/2018|Goiás|2100|NaN|8400|
|704|9591|HL1918|iPhone|4|Marcelo|Guadagnino|12/15/2018|Goiás|5300|NaN|21200|
|705|9604|HL2714|Tablet|2|Mateus|Duque|2/13/2018|Goiás|1600|NaN|3200|
|706|9612|HL4379|Televisão|3|José|Carvalho|1/24/2018|Goiás|2500|NaN|7500|
|707|9626|HL1148|Câmera|5|Lucas|Lemos|1/26/2018|Goiás|2100|NaN|10500|
|708|9631|HL9962|Android|2|Lucas|Araújo|1/20/2018|Goiás|3400|NaN|6800|
|709|9636|HL1148|Câmera|4|Matheus|Tostes|3/3/2018|Goiás|2100|NaN|8400|
|710|9648|HL1148|Câmera|4|Isabel|Lacerda|8/21/2018|Goiás|2100|NaN|8400|
|711|9659|HL2714|Tablet|5|Carolina|Rachide|2/20/2018|Goiás|1600|NaN|8000|
|712|9704|HL1148|Câmera|4|Andre|Nóbrega|3/18/2018|Goiás|2100|NaN|8400|
|713|9705|HL1918|iPhone|5|Jéssica|Netto|8/18/2018|Goiás|5300|NaN|26500|
|714|9714|HL1918|iPhone|1|Livia|Codeceira|9/30/2018|Goiás|5300|NaN|5300|
|715|9720|HL1918|iPhone|5|Erick|Soares|4/22/2018|Goiás|5300|NaN|26500|
|716|9731|HL4379|Televisão|3|Pedro|Xavier|3/2/2018|Goiás|2500|NaN|7500|
|717|9795|HL4379|Televisão|3|Glenda|Santos|2/8/2018|Goiás|2500|NaN|7500|
|718|9804|HL8851|Notebook|5|Hércules|Moreira|1/6/2018|Goiás|3500|NaN|17500|
|719|9833|HL8851|Notebook|5|Bárbara|Lima|11/5/2018|Goiás|3500|NaN|17500|
|720|9848|HL4379|Televisão|2|Gabriel|Thoni|7/18/2018|Goiás|2500|NaN|5000|
|721|9867|HL8851|Notebook|4|Eduardo|Silva|4/19/2018|Goiás|3500|NaN|14000|
|722|9889|HL1148|Câmera|4|Dykson|Silva|6/10/2018|Goiás|2100|NaN|8400|
|723|9892|HL1918|iPhone|3|Luis|Garcia|10/19/2018|Goiás|5300|NaN|15900|
|724|9903|HL1918|iPhone|3|Karina|Camara|3/24/2018|Goiás|5300|NaN|15900|
|725|9916|HL4379|Televisão|5|Andreza|Ramos|7/16/2018|Goiás|2500|NaN|12500|
|726|9921|HL1918|iPhone|1|Mateus|Duque|5/15/2018|Goiás|5300|NaN|5300|
|727|9925|HL1918|iPhone|2|Victor|Gomes|1/9/2018|Goiás|5300|NaN|10600|
|728|9937|HL8851|Notebook|2|Gabriel|Ribeiro|11/28/2018|Goiás|3500|NaN|7000|
|729|9943|HL2714|Tablet|2|Giuseppe|Borges|10/5/2018|Goiás|1600|NaN|3200|
|730|9968|HL2714|Tablet|2|Caio|Caldas|4/4/2018|Goiás|1600|NaN|3200|
|731|9975|HL8851|Notebook|2|Anna|Maia|10/22/2018|Goiás|3500|NaN|7000|
|0|2|HL1148|Câmera|2|Camila|Sobral|10/21/2018|Fortaleza|2100|NaN|4200|
|1|3|HL1918|iPhone|3|Clara|Bruno|7/8/2018|Fortaleza|5300|NaN|15900|
|2|4|HL9962|Android|4|Eduardo|Pacheco|12/19/2018|Fortaleza|3400|NaN|13600|
|3|11|HL1918|iPhone|2|Rafael|Rocha|12/22/2018|Fortaleza|5300|NaN|10600|
|4|15|HL2714|Tablet|2|Caio|Ferreira|7/26/2018|Fortaleza|1600|NaN|3200|
|5|16|HL8851|Notebook|3|Mariana|Freire|11/4/2018|Fortaleza|3500|NaN|10500|
|6|29|HL2714|Tablet|1|Pedro|Oliveira|12/17/2018|Fortaleza|1600|NaN|1600|
|7|53|HL1918|iPhone|3|Raphael|Guedes|7/28/2018|Fortaleza|5300|NaN|15900|
|8|84|HL2714|Tablet|5|Lucas|Costa|9/14/2018|Fortaleza|1600|NaN|8000|
|9|100|HL1918|iPhone|1|Raul|Junqueira|1/17/2018|Fortaleza|5300|NaN|5300|
|10|104|HL1918|iPhone|4|Rubens|Netto|1/8/2018|Fortaleza|5300|NaN|21200|
|11|105|HL1918|iPhone|2|Isabel|Leite|6/2/2018|Fortaleza|5300|NaN|10600|
|12|108|HL4379|Televisão|4|Débora|Lopes|3/5/2018|Fortaleza|2500|NaN|10000|
|13|131|HL1918|iPhone|3|Rilson|Dias|6/7/2018|Fortaleza|5300|NaN|15900|
|14|138|HL8851|Notebook|2|Lucas|Costa|12/24/2018|Fortaleza|3500|NaN|7000|
|15|141|HL1918|iPhone|3|Eduardo|Nunes|10/19/2018|Fortaleza|5300|NaN|15900|
|16|147|HL7348|SmartWatch|5|Andreza|Ramos|1/19/2018|Fortaleza|1400|NaN|7000|
|17|157|HL4379|Televisão|4|Marcelo|Guadagnino|7/23/2018|Fortaleza|2500|NaN|10000|
|18|163|HL1918|iPhone|3|Katharina|Barros|3/12/2018|Fortaleza|5300|NaN|15900|
|19|165|HL1918|iPhone|3|Rafaela|Ferreira|12/19/2018|Fortaleza|5300|NaN|15900|
|20|169|HL9962|Android|4|Gabriella|Sagrillo|7/24/2018|Fortaleza|3400|NaN|13600|
|21|192|HL4379|Televisão|3|Roberta|Nogueira|6/24/2018|Fortaleza|2500|NaN|7500|
|22|199|HL4379|Televisão|3|João|Guadagnino|6/17/2018|Fortaleza|2500|NaN|7500|
|23|200|HL1148|Câmera|5|Michelle|Figueiredo|2/9/2018|Fortaleza|2100|NaN|10500|
|24|211|HL1918|iPhone|2|Matheus|Miranda|12/31/2018|Fortaleza|5300|NaN|10600|
|25|222|HL4379|Televisão|5|Mônica|Rotolo|9/3/2018|Fortaleza|2500|NaN|12500|
|26|230|HL8851|Notebook|1|Juliana|Correa|5/30/2018|Fortaleza|3500|NaN|3500|
|27|232|HL9962|Android|2|Lucas|Freire|2/8/2018|Fortaleza|3400|NaN|6800|
|28|234|HL4379|Televisão|1|Jonatas|Passos|12/20/2018|Fortaleza|2500|NaN|2500|
|29|236|HL1918|iPhone|5|Caio|Moraes|6/17/2018|Fortaleza|5300|NaN|26500|
|30|245|HL8851|Notebook|3|Daniel|Nauenberg|7/10/2018|Fortaleza|3500|NaN|10500|
|31|247|HL1918|iPhone|2|Viviane|Souza|8/9/2018|Fortaleza|5300|NaN|10600|
|32|252|HL1918|iPhone|3|Marina|Aragão|12/25/2018|Fortaleza|5300|NaN|15900|
|33|274|HL1148|Câmera|2|Antonio|Bernhardt|6/26/2018|Fortaleza|2100|NaN|4200|
|34|279|HL9962|Android|2|Jonatas|Essaber|4/3/2018|Fortaleza|3400|NaN|6800|
|35|296|HL9962|Android|5|Bernardo|Nauenberg|2/22/2018|Fortaleza|3400|NaN|17000|
|36|313|HL7348|SmartWatch|1|Juliana|Barreira|1/31/2018|Fortaleza|1400|NaN|1400|
|37|320|HL1918|iPhone|2|Rodrigo|Alves|11/19/2018|Fortaleza|5300|NaN|10600|
|38|325|HL4379|Televisão|5|Lucas|Lemos|8/12/2018|Fortaleza|2500|NaN|12500|
|39|327|HL7348|SmartWatch|5|Wendela|Mariz|5/24/2018|Fortaleza|1400|NaN|7000|
|40|338|HL1918|iPhone|5|Rachel|Silva|11/16/2018|Fortaleza|5300|NaN|26500|
|41|340|HL1918|iPhone|1|Rodrigo|Ramos|5/6/2018|Fortaleza|5300|NaN|5300|
|42|367|HL7348|SmartWatch|1|Michelle|Figueiredo|3/27/2018|Fortaleza|1400|NaN|1400|
|43|382|HL7348|SmartWatch|1|Cézar|Santos|11/17/2018|Fortaleza|1400|NaN|1400|
|44|383|HL9962|Android|4|Hércules|Moreira|8/1/2018|Fortaleza|3400|NaN|13600|
|45|384|HL2714|Tablet|1|Ives|Barbosa|4/27/2018|Fortaleza|1600|NaN|1600|
|46|385|HL9962|Android|2|José|Jesus|12/5/2018|Fortaleza|3400|NaN|6800|
|47|387|HL4379|Televisão|5|Guilherme|Lima|5/9/2018|Fortaleza|2500|NaN|12500|
|48|391|HL7348|SmartWatch|5|Ives|Teixeira|10/31/2018|Fortaleza|1400|NaN|7000|
|49|394|HL1918|iPhone|5|Lucas|Monte|12/25/2018|Fortaleza|5300|NaN|26500|
|50|400|HL8851|Notebook|5|Vitor|Campos|8/24/2018|Fortaleza|3500|NaN|17500|
|51|403|HL1148|Câmera|4|Gabriela|Mello|6/20/2018|Fortaleza|2100|NaN|8400|
|52|405|HL1918|iPhone|4|Lara|Moreira|12/23/2018|Fortaleza|5300|NaN|21200|
|53|416|HL1918|iPhone|5|Samara|Pinto|4/3/2018|Fortaleza|5300|NaN|26500|
|54|426|HL8851|Notebook|4|Thiago|Miura|7/15/2018|Fortaleza|3500|NaN|14000|
|55|437|HL9962|Android|4|Michelle|Pereira|6/14/2018|Fortaleza|3400|NaN|13600|
|56|448|HL4379|Televisão|5|Carlos|Azevedo|2/13/2018|Fortaleza|2500|NaN|12500|
|57|449|HL1918|iPhone|2|Anderson|Cavalcanti|10/17/2018|Fortaleza|5300|NaN|10600|
|58|459|HL8851|Notebook|4|Beatriz|Biase|7/28/2018|Fortaleza|3500|NaN|14000|
|59|465|HL7348|SmartWatch|2|Clara|Bruno|12/10/2018|Fortaleza|1400|NaN|2800|
|60|482|HL1918|iPhone|1|Matheus|Delgado|5/20/2018|Fortaleza|5300|NaN|5300|
|61|486|HL1918|iPhone|1|Jéssica|Netto|1/8/2018|Fortaleza|5300|NaN|5300|
|62|495|HL2714|Tablet|5|Tayla|Lima|1/27/2018|Fortaleza|1600|NaN|8000|
|63|496|HL8851|Notebook|5|Michelle|Pereira|3/1/2018|Fortaleza|3500|NaN|17500|
|64|499|HL8851|Notebook|5|Maria|Motta|6/9/2018|Fortaleza|3500|NaN|17500|
|65|505|HL4379|Televisão|2|Cézar|Santos|4/15/2018|Fortaleza|2500|NaN|5000|
|66|509|HL9962|Android|1|Natalia|Marinho|7/18/2018|Fortaleza|3400|NaN|3400|
|67|511|HL1918|iPhone|4|Antonio|Bernhardt|11/9/2018|Fortaleza|5300|NaN|21200|
|68|517|HL1918|iPhone|1|Juliana|Silva|8/19/2018|Fortaleza|5300|NaN|5300|
|69|518|HL1918|iPhone|4|Lucas|Assunção|7/27/2018|Fortaleza|5300|NaN|21200|
|70|527|HL4379|Televisão|1|Gustavo|Guimarães|10/23/2018|Fortaleza|2500|NaN|2500|
|71|535|HL4379|Televisão|5|Lucas|Lima|10/9/2018|Fortaleza|2500|NaN|12500|
|72|537|HL1148|Câmera|3|Dandara|Reis|3/18/2018|Fortaleza|2100|NaN|6300|
|73|538|HL4379|Televisão|1|Lucas|Almeida|12/24/2018|Fortaleza|2500|NaN|2500|
|74|547|HL1918|iPhone|2|Giovanna|Santos|1/27/2018|Fortaleza|5300|NaN|10600|
|75|554|HL7348|SmartWatch|1|Alexandre|Rodriguez|8/14/2018|Fortaleza|1400|NaN|1400|
|76|562|HL1918|iPhone|4|Dykson|Silva|1/18/2018|Fortaleza|5300|NaN|21200|
|77|569|HL2714|Tablet|1|Bruna|Chein|5/21/2018|Fortaleza|1600|NaN|1600|
|78|574|HL1918|iPhone|2|Gustavo|Gomes|9/25/2018|Fortaleza|5300|NaN|10600|
|79|584|HL7348|SmartWatch|5|David|Vasconcelos|2/15/2018|Fortaleza|1400|NaN|7000|
|80|585|HL4379|Televisão|5|Isabela|Teixeira|12/16/2018|Fortaleza|2500|NaN|12500|
|81|590|HL9962|Android|2|Jorge|Fonseca|7/27/2018|Fortaleza|3400|NaN|6800|
|82|603|HL8851|Notebook|1|Adriana|Passos|8/15/2018|Fortaleza|3500|NaN|3500|
|83|605|HL7348|SmartWatch|1|Bruna|Silva|2/22/2018|Fortaleza|1400|NaN|1400|
|84|608|HL4379|Televisão|4|Ana|Soledade|7/18/2018|Fortaleza|2500|NaN|10000|
|85|611|HL8851|Notebook|5|Fernanda|Coutinho|2/17/2018|Fortaleza|3500|NaN|17500|
|86|621|HL8851|Notebook|2|Arthur|Fernandes|2/16/2018|Fortaleza|3500|NaN|7000|
|87|629|HL9962|Android|4|Raissa|Pinheiro|1/29/2018|Fortaleza|3400|NaN|13600|
|88|635|HL4379|Televisão|5|Jorge|Carvalho|8/21/2018|Fortaleza|2500|NaN|12500|
|89|642|HL7348|SmartWatch|2|Gabriel|Pereira|2/20/2018|Fortaleza|1400|NaN|2800|
|90|646|HL4379|Televisão|2|Rachel|Silva|2/11/2018|Fortaleza|2500|NaN|5000|
|91|649|HL9962|Android|2|João|Junior|11/12/2018|Fortaleza|3400|NaN|6800|
|92|650|HL4379|Televisão|3|Caio|Affonso|3/21/2018|Fortaleza|2500|NaN|7500|
|93|677|HL1918|iPhone|2|Raul|Silveira|12/10/2018|Fortaleza|5300|NaN|10600|
|94|695|HL2714|Tablet|3|Rodrigo|Alves|7/12/2018|Fortaleza|1600|NaN|4800|
|95|707|HL1148|Câmera|5|Julia|Silva|11/10/2018|Fortaleza|2100|NaN|10500|
|96|714|HL9962|Android|5|Juliana|Goes|7/3/2018|Fortaleza|3400|NaN|17000|
|97|717|HL8851|Notebook|4|Ravena|Bhering|5/23/2018|Fortaleza|3500|NaN|14000|
|98|718|HL1148|Câmera|5|Deysiane|Medronho|11/7/2018|Fortaleza|2100|NaN|10500|
|99|725|HL2714|Tablet|4|Mariana|Freire|5/7/2018|Fortaleza|1600|NaN|6400|
|100|734|HL4379|Televisão|5|Raphael|Kurtz|10/13/2018|Fortaleza|2500|NaN|12500|
|101|741|HL4379|Televisão|2|Caroline|Pinto|6/20/2018|Fortaleza|2500|NaN|5000|
|102|747|HL4379|Televisão|1|Luiza|Cavalcanti|5/8/2018|Fortaleza|2500|NaN|2500|
|103|750|HL1918|iPhone|1|Leandro|Rodrigues|9/29/2018|Fortaleza|5300|NaN|5300|
|104|762|HL1918|iPhone|5|Elena|Barreto|5/25/2018|Fortaleza|5300|NaN|26500|
|105|772|HL1918|iPhone|4|Thales|Andrade|11/26/2018|Fortaleza|5300|NaN|21200|
|106|773|HL4379|Televisão|2|Lívia|Marques|7/23/2018|Fortaleza|2500|NaN|5000|
|107|778|HL4379|Televisão|3|Raissa|Maia|12/10/2018|Fortaleza|2500|NaN|7500|
|108|795|HL4379|Televisão|1|Diogo|Peixoto|7/18/2018|Fortaleza|2500|NaN|2500|
|109|797|HL4379|Televisão|5|Itai|Puntel|7/4/2018|Fortaleza|2500|NaN|12500|
|110|800|HL7348|SmartWatch|3|Brenno|Santos|1/3/2018|Fortaleza|1400|NaN|4200|
|111|812|HL8851|Notebook|2|Luiza|Procaci|4/5/2018|Fortaleza|3500|NaN|7000|
|112|815|HL1918|iPhone|2|Anízio|Carvalho|12/16/2018|Fortaleza|5300|NaN|10600|
|113|823|HL2714|Tablet|2|Bárbara|Cavalcante|2/27/2018|Fortaleza|1600|NaN|3200|
|114|830|HL1918|iPhone|1|Tainah|Nogueira|6/15/2018|Fortaleza|5300|NaN|5300|
|115|835|HL9962|Android|1|Gabriel|Ribeiro|1/29/2018|Fortaleza|3400|NaN|3400|
|116|860|HL9962|Android|2|Maria|Costa|5/2/2018|Fortaleza|3400|NaN|6800|
|117|861|HL9962|Android|5|Guilherme|Assis|8/26/2018|Fortaleza|3400|NaN|17000|
|118|867|HL4379|Televisão|5|Ana|Leite|9/5/2018|Fortaleza|2500|NaN|12500|
|119|871|HL7348|SmartWatch|1|Hércules|Moreira|4/9/2018|Fortaleza|1400|NaN|1400|
|120|874|HL1148|Câmera|4|Fernanda|Rubim|9/11/2018|Fortaleza|2100|NaN|8400|
|121|879|HL1918|iPhone|3|Jorge|Fonseca|1/11/2018|Fortaleza|5300|NaN|15900|
|122|881|HL8851|Notebook|3|Milena|Almeida|1/11/2018|Fortaleza|3500|NaN|10500|
|123|887|HL4379|Televisão|4|Joyce|Souza|7/12/2018|Fortaleza|2500|NaN|10000|
|124|893|HL1148|Câmera|4|Renan|Melo|1/29/2018|Fortaleza|2100|NaN|8400|
|125|897|HL1918|iPhone|1|Cézar|Santos|2/14/2018|Fortaleza|5300|NaN|5300|
|126|898|HL1918|iPhone|2|Luiz|Xavier|5/30/2018|Fortaleza|5300|NaN|10600|
|127|915|HL4379|Televisão|1|Isabelle|Firmino|3/13/2018|Fortaleza|2500|NaN|2500|
|128|917|HL7348|SmartWatch|1|Pedro|Oliveira|11/1/2018|Fortaleza|1400|NaN|1400|
|129|936|HL1918|iPhone|3|Pedro|Rodrigues|6/5/2018|Fortaleza|5300|NaN|15900|
|130|964|HL7348|SmartWatch|5|Carlos|Azevedo|8/30/2018|Fortaleza|1400|NaN|7000|
|131|986|HL1148|Câmera|5|Aline|Morais|9/30/2018|Fortaleza|2100|NaN|10500|
|132|994|HL8851|Notebook|3|Guilherme|Vianna|7/5/2018|Fortaleza|3500|NaN|10500|
|133|1007|HL2714|Tablet|3|Giovana|Vilela|7/5/2018|Fortaleza|1600|NaN|4800|
|134|1025|HL4379|Televisão|3|Lucas|Assunção|4/19/2018|Fortaleza|2500|NaN|7500|
|135|1044|HL1918|iPhone|4|Rafaela|Gomes|11/8/2018|Fortaleza|5300|NaN|21200|
|136|1061|HL2714|Tablet|3|Pedro|Santos|9/30/2018|Fortaleza|1600|NaN|4800|
|137|1074|HL1918|iPhone|5|Marina|Perdomo|1/27/2018|Fortaleza|5300|NaN|26500|
|138|1075|HL8851|Notebook|2|Jônatas|Soares|9/22/2018|Fortaleza|3500|NaN|7000|
|139|1077|HL4379|Televisão|5|Giuseppe|Bhering|3/30/2018|Fortaleza|2500|NaN|12500|
|140|1091|HL4379|Televisão|3|Danilo|Rubim|7/16/2018|Fortaleza|2500|NaN|7500|
|141|1100|HL7348|SmartWatch|1|Silvio|Provenzano|5/26/2018|Fortaleza|1400|NaN|1400|
|142|1103|HL2714|Tablet|4|Victor|Gomes|12/4/2018|Fortaleza|1600|NaN|6400|
|143|1107|HL1918|iPhone|4|Jeferson|Costa|7/17/2018|Fortaleza|5300|NaN|21200|
|144|1115|HL1918|iPhone|3|Carlos|Barbosa|8/23/2018|Fortaleza|5300|NaN|15900|
|145|1126|HL9962|Android|3|Carla|Zakhm|9/3/2018|Fortaleza|3400|NaN|10200|
|146|1138|HL4379|Televisão|1|Gabrielle|Viríssimo|9/11/2018|Fortaleza|2500|NaN|2500|
|147|1153|HL1148|Câmera|1|Lucas|Neto|8/3/2018|Fortaleza|2100|NaN|2100|
|148|1162|HL2714|Tablet|3|Erick|Soares|7/21/2018|Fortaleza|1600|NaN|4800|
|149|1164|HL1148|Câmera|5|Luiz|Conceição|9/24/2018|Fortaleza|2100|NaN|10500|
|150|1180|HL9962|Android|3|Gabriela|Cavalcanti|5/19/2018|Fortaleza|3400|NaN|10200|
|151|1181|HL2714|Tablet|4|Rachel|Silva|8/4/2018|Fortaleza|1600|NaN|6400|
|152|1187|HL1148|Câmera|5|Joao|Silva|9/11/2018|Fortaleza|2100|NaN|10500|
|153|1192|HL4379|Televisão|1|Guilherme|Santos|10/7/2018|Fortaleza|2500|NaN|2500|
|154|1204|HL1148|Câmera|1|Gustavo|Accardo|1/19/2018|Fortaleza|2100|NaN|2100|
|155|1216|HL9962|Android|2|Marina|Gama|10/10/2018|Fortaleza|3400|NaN|6800|
|156|1221|HL2714|Tablet|4|Camille|Silva|8/29/2018|Fortaleza|1600|NaN|6400|
|157|1229|HL7348|SmartWatch|5|Douglas|Rodrigues|8/7/2018|Fortaleza|1400|NaN|7000|
|158|1238|HL1918|iPhone|4|Marcela|Medeiros|4/27/2018|Fortaleza|5300|NaN|21200|
|159|1242|HL9962|Android|1|Caio|Vianna|6/18/2018|Fortaleza|3400|NaN|3400|
|160|1249|HL2714|Tablet|5|Renan|Melo|6/26/2018|Fortaleza|1600|NaN|8000|
|161|1251|HL4379|Televisão|2|Jéssica|Resinente|8/22/2018|Fortaleza|2500|NaN|5000|
|162|1259|HL1148|Câmera|2|Wen|Santos|4/18/2018|Fortaleza|2100|NaN|4200|
|163|1261|HL1918|iPhone|1|João|Guadagnino|3/11/2018|Fortaleza|5300|NaN|5300|
|164|1270|HL1918|iPhone|4|Juliana|Goes|10/27/2018|Fortaleza|5300|NaN|21200|
|165|1273|HL2714|Tablet|5|João|Oliveira|1/7/2018|Fortaleza|1600|NaN|8000|
|166|1276|HL4379|Televisão|4|Lucas|Neto|5/1/2018|Fortaleza|2500|NaN|10000|
|167|1277|HL1918|iPhone|2|Ulisses|Filho|3/19/2018|Fortaleza|5300|NaN|10600|
|168|1284|HL9962|Android|4|Priscila|Carvalho|7/14/2018|Fortaleza|3400|NaN|13600|
|169|1291|HL1918|iPhone|3|Daniela|Pereira|2/9/2018|Fortaleza|5300|NaN|15900|
|170|1297|HL8851|Notebook|4|Antonio|Manhães|1/16/2018|Fortaleza|3500|NaN|14000|
|171|1315|HL2714|Tablet|3|Daniel|Terra|11/26/2018|Fortaleza|1600|NaN|4800|
|172|1321|HL9962|Android|3|Pedro|Lyra|3/20/2018|Fortaleza|3400|NaN|10200|
|173|1331|HL7348|SmartWatch|4|Fernanda|Ferreira|4/4/2018|Fortaleza|1400|NaN|5600|
|174|1333|HL7348|SmartWatch|3|Carolina|Santos|2/3/2018|Fortaleza|1400|NaN|4200|
|175|1334|HL2714|Tablet|4|Lucas|Chagas|9/24/2018|Fortaleza|1600|NaN|6400|
|176|1336|HL1148|Câmera|4|Clara|Bruno|7/11/2018|Fortaleza|2100|NaN|8400|
|177|1351|HL1918|iPhone|2|Jônatas|Soares|7/5/2018|Fortaleza|5300|NaN|10600|
|178|1358|HL1918|iPhone|4|João|Luz|7/13/2018|Fortaleza|5300|NaN|21200|
|179|1359|HL4379|Televisão|4|Camille|Silva|11/4/2018|Fortaleza|2500|NaN|10000|
|180|1360|HL2714|Tablet|4|Cézar|Santos|11/11/2018|Fortaleza|1600|NaN|6400|
|181|1362|HL9962|Android|5|Nathan|Morelli|12/11/2018|Fortaleza|3400|NaN|17000|
|182|1371|HL9962|Android|5|Jessica|Ferreira|7/8/2018|Fortaleza|3400|NaN|17000|
|183|1376|HL7348|SmartWatch|3|Larissa|Florim|3/21/2018|Fortaleza|1400|NaN|4200|
|184|1381|HL7348|SmartWatch|3|Sylvio|Bernhardt|1/30/2018|Fortaleza|1400|NaN|4200|
|185|1384|HL4379|Televisão|5|Matheus|Ramos|9/26/2018|Fortaleza|2500|NaN|12500|
|186|1387|HL1918|iPhone|3|Beatriz|Rocha|6/14/2018|Fortaleza|5300|NaN|15900|
|187|1405|HL2714|Tablet|2|Hércules|Júnior|10/15/2018|Fortaleza|1600|NaN|3200|
|188|1415|HL8851|Notebook|4|Beatriz|Perdomo|9/23/2018|Fortaleza|3500|NaN|14000|
|189|1418|HL4379|Televisão|1|Guilherme|Lima|4/22/2018|Fortaleza|2500|NaN|2500|
|190|1430|HL4379|Televisão|2|Milena|Alcoforado|11/10/2018|Fortaleza|2500|NaN|5000|
|191|1442|HL1148|Câmera|3|Rodrigo|Bruno|8/14/2018|Fortaleza|2100|NaN|6300|
|192|1444|HL2714|Tablet|3|Luiz|Conceição|12/7/2018|Fortaleza|1600|NaN|4800|
|193|1455|HL8851|Notebook|3|Vanessa|Rodrigues|7/25/2018|Fortaleza|3500|NaN|10500|
|194|1483|HL2714|Tablet|5|Luiza|Marques|11/2/2018|Fortaleza|1600|NaN|8000|
|195|1488|HL4379|Televisão|4|Eduardo|Pacheco|2/8/2018|Fortaleza|2500|NaN|10000|
|196|1490|HL4379|Televisão|1|Breno|Britto|1/23/2018|Fortaleza|2500|NaN|2500|
|197|1502|HL8851|Notebook|4|Thales|Portillo|5/10/2018|Fortaleza|3500|NaN|14000|
|198|1511|HL1918|iPhone|3|Marina|Cormack|9/5/2018|Fortaleza|5300|NaN|15900|
|199|1517|HL9962|Android|5|Bernardo|Souza|4/4/2018|Fortaleza|3400|NaN|17000|
|200|1528|HL1148|Câmera|3|Letícia|Araujo|10/22/2018|Fortaleza|2100|NaN|6300|
|201|1530|HL4379|Televisão|1|Marina|Miranda|11/26/2018|Fortaleza|2500|NaN|2500|
|202|1540|HL7348|SmartWatch|3|Gustavo|Accardo|9/25/2018|Fortaleza|1400|NaN|4200|
|203|1564|HL4379|Televisão|1|Livia|Cozendey|10/21/2018|Fortaleza|2500|NaN|2500|
|204|1565|HL2714|Tablet|5|Lívia|Marques|11/24/2018|Fortaleza|1600|NaN|8000|
|205|1580|HL8851|Notebook|1|Natalia|Accioly|1/15/2018|Fortaleza|3500|NaN|3500|
|206|1582|HL8851|Notebook|3|Bruna|Franco|5/28/2018|Fortaleza|3500|NaN|10500|
|207|1597|HL1918|iPhone|2|Lunna|Vannier|10/24/2018|Fortaleza|5300|NaN|10600|
|208|1601|HL1918|iPhone|4|Ana|Gonzaga|6/12/2018|Fortaleza|5300|NaN|21200|
|209|1602|HL7348|SmartWatch|1|Antônio|Oliveira|12/31/2018|Fortaleza|1400|NaN|1400|
|210|1607|HL1918|iPhone|5|Thiago|Veiga|4/23/2018|Fortaleza|5300|NaN|26500|
|211|1610|HL1918|iPhone|2|Eric|Neves|12/23/2018|Fortaleza|5300|NaN|10600|
|212|1613|HL1148|Câmera|3|Gabriel|Thoni|4/8/2018|Fortaleza|2100|NaN|6300|
|213|1616|HL4379|Televisão|2|Fernanda|Figueiredo|9/11/2018|Fortaleza|2500|NaN|5000|
|214|1630|HL4379|Televisão|3|Karine|Barros|6/3/2018|Fortaleza|2500|NaN|7500|
|215|1638|HL1918|iPhone|3|Maria|Costa|12/10/2018|Fortaleza|5300|NaN|15900|
|216|1639|HL4379|Televisão|2|Matheus|Afonso|9/2/2018|Fortaleza|2500|NaN|5000|
|217|1652|HL1918|iPhone|5|Natalia|Accioly|10/25/2018|Fortaleza|5300|NaN|26500|
|218|1653|HL8851|Notebook|2|Thales|Portillo|4/16/2018|Fortaleza|3500|NaN|7000|
|219|1667|HL4379|Televisão|1|Michelle|Miura|11/16/2018|Fortaleza|2500|NaN|2500|
|220|1670|HL4379|Televisão|5|Wendela|Veloso|9/16/2018|Fortaleza|2500|NaN|12500|
|221|1674|HL1918|iPhone|1|Bruno|Salomão|5/10/2018|Fortaleza|5300|NaN|5300|
|222|1676|HL8851|Notebook|3|Rafaela|Rodrigues|4/9/2018|Fortaleza|3500|NaN|10500|
|223|1684|HL4379|Televisão|4|Caroll|Johnson|10/3/2018|Fortaleza|2500|NaN|10000|
|224|1695|HL8851|Notebook|2|Raphael|Machado|10/25/2018|Fortaleza|3500|NaN|7000|
|225|1698|HL2714|Tablet|5|Antonio|Manhães|6/17/2018|Fortaleza|1600|NaN|8000|
|226|1700|HL4379|Televisão|2|Pedro|Oliveira|9/4/2018|Fortaleza|2500|NaN|5000|
|227|1705|HL7348|SmartWatch|3|Wilson|Farias|2/20/2018|Fortaleza|1400|NaN|4200|
|228|1706|HL1918|iPhone|2|Ana|Gonzaga|7/12/2018|Fortaleza|5300|NaN|10600|
|229|1709|HL7348|SmartWatch|2|Livia|Codeceira|10/24/2018|Fortaleza|1400|NaN|2800|
|230|1710|HL7348|SmartWatch|2|Chan|Santos|1/3/2018|Fortaleza|1400|NaN|2800|
|231|1718|HL1148|Câmera|3|Gabriel|Azevedo|5/23/2018|Fortaleza|2100|NaN|6300|
|232|1719|HL9962|Android|2|Raphael|Coelho|1/8/2018|Fortaleza|3400|NaN|6800|
|233|1720|HL2714|Tablet|1|Beatriz|Cavalcanti|10/31/2018|Fortaleza|1600|NaN|1600|
|234|1722|HL4379|Televisão|2|Beatriz|Silva|7/12/2018|Fortaleza|2500|NaN|5000|
|235|1723|HL8851|Notebook|2|Lucas|Reis|1/11/2018|Fortaleza|3500|NaN|7000|
|236|1740|HL8851|Notebook|5|Matheus|Silva|9/4/2018|Fortaleza|3500|NaN|17500|
|237|1759|HL1918|iPhone|5|Lucas|Freire|1/17/2018|Fortaleza|5300|NaN|26500|
|238|1771|HL4379|Televisão|1|Mateus|Polastri|5/12/2018|Fortaleza|2500|NaN|2500|
|239|1774|HL1918|iPhone|3|Mariana|Barrozo|5/30/2018|Fortaleza|5300|NaN|15900|
|240|1777|HL2714|Tablet|1|Marina|Perdomo|11/4/2018|Fortaleza|1600|NaN|1600|
|241|1784|HL9962|Android|2|Pedro|Cardoso|12/13/2018|Fortaleza|3400|NaN|6800|
|242|1789|HL9962|Android|1|Mateus|Polastri|9/8/2018|Fortaleza|3400|NaN|3400|
|243|1804|HL4379|Televisão|3|Alon|Palmeira|2/14/2018|Fortaleza|2500|NaN|7500|
|244|1812|HL4379|Televisão|3|Bianca|Procaci|8/18/2018|Fortaleza|2500|NaN|7500|
|245|1818|HL1918|iPhone|5|Raísa|Berto|7/21/2018|Fortaleza|5300|NaN|26500|
|246|1841|HL4379|Televisão|4|Nicolas|Monteiro|1/6/2018|Fortaleza|2500|NaN|10000|
|247|1843|HL8851|Notebook|1|Gabriel|Puntel|9/19/2018|Fortaleza|3500|NaN|3500|
|248|1845|HL1918|iPhone|4|Bianca|Piero|9/11/2018|Fortaleza|5300|NaN|21200|
|249|1860|HL1918|iPhone|2|Fernanda|Coutinho|12/5/2018|Fortaleza|5300|NaN|10600|
|250|1865|HL7348|SmartWatch|1|Julia|Penteado|5/3/2018|Fortaleza|1400|NaN|1400|
|251|1872|HL1148|Câmera|2|Thomáz|Rodriguez|8/21/2018|Fortaleza|2100|NaN|4200|
|252|1891|HL1148|Câmera|3|Victor|Firmino|1/24/2018|Fortaleza|2100|NaN|6300|
|253|1896|HL9962|Android|3|Anna|Figueiredo|4/13/2018|Fortaleza|3400|NaN|10200|
|254|1904|HL1918|iPhone|5|Thomaz|Ferreira|2/3/2018|Fortaleza|5300|NaN|26500|
|255|1906|HL8851|Notebook|2|Chan|Santos|1/17/2018|Fortaleza|3500|NaN|7000|
|256|1922|HL4379|Televisão|2|Giselia|Thiele|3/30/2018|Fortaleza|2500|NaN|5000|
|257|1954|HL4379|Televisão|2|Izabel|Miura|4/13/2018|Fortaleza|2500|NaN|5000|
|258|1956|HL8851|Notebook|4|Mateus|Maia|8/3/2018|Fortaleza|3500|NaN|14000|
|259|1961|HL4379|Televisão|2|Matheus|Santos|10/3/2018|Fortaleza|2500|NaN|5000|
|260|1962|HL1918|iPhone|1|Arthur|Portela|8/15/2018|Fortaleza|5300|NaN|5300|
|261|1971|HL1918|iPhone|2|Rebeca|Reis|10/14/2018|Fortaleza|5300|NaN|10600|
|262|1989|HL1918|iPhone|1|Julie|Ferreira|2/4/2018|Fortaleza|5300|NaN|5300|
|263|1990|HL1918|iPhone|3|Julia|Figueiredo|4/26/2018|Fortaleza|5300|NaN|15900|
|264|1995|HL1918|iPhone|1|Hércules|Moreira|10/22/2018|Fortaleza|5300|NaN|5300|
|265|1997|HL9962|Android|3|Victor|Gomes|6/5/2018|Fortaleza|3400|NaN|10200|
|266|2020|HL4379|Televisão|3|Miguel|Carneiro|11/3/2018|Fortaleza|2500|NaN|7500|
|267|2021|HL8851|Notebook|3|Caroline|Aquino|9/3/2018|Fortaleza|3500|NaN|10500|
|268|2035|HL1148|Câmera|2|Bruna|Rosa|1/18/2018|Fortaleza|2100|NaN|4200|
|269|2045|HL8851|Notebook|3|Jeferson|Costa|10/16/2018|Fortaleza|3500|NaN|10500|
|270|2055|HL9962|Android|1|Rafaela|Gomes|6/12/2018|Fortaleza|3400|NaN|3400|
|271|2076|HL7348|SmartWatch|2|Mariana|Freire|10/15/2018|Fortaleza|1400|NaN|2800|
|272|2083|HL1148|Câmera|1|Ives|Teixeira|2/5/2018|Fortaleza|2100|NaN|2100|
|273|2101|HL9962|Android|5|Natalia|Marinho|11/16/2018|Fortaleza|3400|NaN|17000|
|274|2118|HL4379|Televisão|3|Ana|Leite|1/6/2018|Fortaleza|2500|NaN|7500|
|275|2123|HL9962|Android|5|Marina|Cormack|6/27/2018|Fortaleza|3400|NaN|17000|
|276|2132|HL1918|iPhone|5|Maria|Correa|8/11/2018|Fortaleza|5300|NaN|26500|
|277|2149|HL7348|SmartWatch|2|Joyce|Souza|9/30/2018|Fortaleza|1400|NaN|2800|
|278|2175|HL8851|Notebook|2|Diogo|Ressurreição|12/25/2018|Fortaleza|3500|NaN|7000|
|279|2176|HL8851|Notebook|3|Thales|Santos|12/26/2018|Fortaleza|3500|NaN|10500|
|280|2185|HL8851|Notebook|1|Carolina|Siqueira|2/16/2018|Fortaleza|3500|NaN|3500|
|281|2190|HL2714|Tablet|2|Breno|Varella|8/30/2018|Fortaleza|1600|NaN|3200|
|282|2193|HL1148|Câmera|5|Adrielle|Forte|7/3/2018|Fortaleza|2100|NaN|10500|
|283|2194|HL1918|iPhone|5|Rafael|Guimarães|12/21/2018|Fortaleza|5300|NaN|26500|
|284|2210|HL1918|iPhone|5|Sandy|Figueiredo|3/24/2018|Fortaleza|5300|NaN|26500|
|285|2211|HL1148|Câmera|1|Ana|Almeida|6/25/2018|Fortaleza|2100|NaN|2100|
|286|2212|HL8851|Notebook|2|Juliana|Hollander|7/31/2018|Fortaleza|3500|NaN|7000|
|287|2215|HL8851|Notebook|1|Lucas|Neto|6/12/2018|Fortaleza|3500|NaN|3500|
|288|2216|HL4379|Televisão|5|Rogério|Gentile|10/21/2018|Fortaleza|2500|NaN|12500|
|289|2222|HL1918|iPhone|1|Bruno|Souza|12/22/2018|Fortaleza|5300|NaN|5300|
|290|2240|HL4379|Televisão|1|Marianna|Pestana|5/7/2018|Fortaleza|2500|NaN|2500|
|291|2243|HL4379|Televisão|2|Ramon|Araujo|8/11/2018|Fortaleza|2500|NaN|5000|
|292|2251|HL4379|Televisão|5|Joyce|Souza|4/23/2018|Fortaleza|2500|NaN|12500|
|293|2252|HL1918|iPhone|2|Wilson|Meirelles|9/21/2018|Fortaleza|5300|NaN|10600|
|294|2261|HL1918|iPhone|5|Anderson|Barreto|6/22/2018|Fortaleza|5300|NaN|26500|
|295|2270|HL1918|iPhone|2|Guilherme|Monteiro|2/19/2018|Fortaleza|5300|NaN|10600|
|296|2273|HL1918|iPhone|4|Lucas|Costa|1/5/2018|Fortaleza|5300|NaN|21200|
|297|2293|HL1918|iPhone|5|Renan|Freire|11/6/2018|Fortaleza|5300|NaN|26500|
|298|2294|HL1148|Câmera|2|Paola|Abreu|5/8/2018|Fortaleza|2100|NaN|4200|
|299|2301|HL8851|Notebook|3|Bruna|Franco|5/12/2018|Fortaleza|3500|NaN|10500|
|300|2305|HL1918|iPhone|5|Gustavo|Guimarães|9/9/2018|Fortaleza|5300|NaN|26500|
|301|2320|HL9962|Android|1|Marcelo|Borges|6/21/2018|Fortaleza|3400|NaN|3400|
|302|2325|HL1148|Câmera|1|Samara|Pinto|3/24/2018|Fortaleza|2100|NaN|2100|
|303|2327|HL4379|Televisão|4|Julia|Penteado|6/20/2018|Fortaleza|2500|NaN|10000|
|304|2340|HL1918|iPhone|1|Rodrigo|Mendes|1/7/2018|Fortaleza|5300|NaN|5300|
|305|2342|HL1918|iPhone|3|Fernanda|Silva|5/13/2018|Fortaleza|5300|NaN|15900|
|306|2344|HL4379|Televisão|1|Rogério|Gentile|9/7/2018|Fortaleza|2500|NaN|2500|
|307|2347|HL1148|Câmera|1|Ana|Silva|8/26/2018|Fortaleza|2100|NaN|2100|
|308|2348|HL1918|iPhone|2|Rebeca|Reis|9/28/2018|Fortaleza|5300|NaN|10600|
|309|2350|HL9962|Android|5|Bernardo|Ribeiro|2/9/2018|Fortaleza|3400|NaN|17000|
|310|2355|HL1918|iPhone|4|Monique|Vasconcelos|4/15/2018|Fortaleza|5300|NaN|21200|
|311|2366|HL1148|Câmera|5|Letícia|Araujo|2/24/2018|Fortaleza|2100|NaN|10500|
|312|2373|HL1918|iPhone|1|Rodrigo|Souza|8/24/2018|Fortaleza|5300|NaN|5300|
|313|2374|HL1918|iPhone|2|Vittorio|Freitas|10/15/2018|Fortaleza|5300|NaN|10600|
|314|2380|HL1918|iPhone|2|Gabriel|Silva|6/7/2018|Fortaleza|5300|NaN|10600|
|315|2382|HL8851|Notebook|2|Livia|Codeceira|8/28/2018|Fortaleza|3500|NaN|7000|
|316|2388|HL4379|Televisão|4|Raíssa|Oliveira|10/11/2018|Fortaleza|2500|NaN|10000|
|317|2404|HL8851|Notebook|3|Gabriel|Rocha|2/20/2018|Fortaleza|3500|NaN|10500|
|318|2414|HL2714|Tablet|3|Gabriel|Ribeiro|6/6/2018|Fortaleza|1600|NaN|4800|
|319|2415|HL2714|Tablet|4|Raíssa|Nimer|5/21/2018|Fortaleza|1600|NaN|6400|
|320|2416|HL4379|Televisão|3|Lais|Candido|10/30/2018|Fortaleza|2500|NaN|7500|
|321|2430|HL2714|Tablet|2|Eduardo|Lopes|11/13/2018|Fortaleza|1600|NaN|3200|
|322|2432|HL7348|SmartWatch|5|Gabriel|Azevedo|11/6/2018|Fortaleza|1400|NaN|7000|
|323|2433|HL4379|Televisão|2|Anderson|Cavalcanti|6/13/2018|Fortaleza|2500|NaN|5000|
|324|2435|HL4379|Televisão|5|Khaio|Mesquita|8/4/2018|Fortaleza|2500|NaN|12500|
|325|2439|HL9962|Android|5|Mariane|Ferreira|3/25/2018|Fortaleza|3400|NaN|17000|
|326|2446|HL7348|SmartWatch|4|Pedro|Rodrigues|10/25/2018|Fortaleza|1400|NaN|5600|
|327|2447|HL4379|Televisão|2|Célio|Xavier|3/26/2018|Fortaleza|2500|NaN|5000|
|328|2452|HL4379|Televisão|1|Tiago|Pereira|10/5/2018|Fortaleza|2500|NaN|2500|
|329|2468|HL1918|iPhone|4|Rilson|Dias|6/6/2018|Fortaleza|5300|NaN|21200|
|330|2474|HL4379|Televisão|5|Raphael|Kurtz|6/7/2018|Fortaleza|2500|NaN|12500|
|331|2489|HL1918|iPhone|5|Adriane|Gomes|8/8/2018|Fortaleza|5300|NaN|26500|
|332|2516|HL7348|SmartWatch|4|Raissa|Sales|10/5/2018|Fortaleza|1400|NaN|5600|
|333|2517|HL9962|Android|2|Gabrielle|Costa|3/27/2018|Fortaleza|3400|NaN|6800|
|334|2537|HL8851|Notebook|4|Luana|Santos|6/18/2018|Fortaleza|3500|NaN|14000|
|335|2546|HL1918|iPhone|4|Paloma|Sperandei|7/17/2018|Fortaleza|5300|NaN|21200|
|336|2556|HL1918|iPhone|5|Stefan|Santos|4/14/2018|Fortaleza|5300|NaN|26500|
|337|2560|HL2714|Tablet|2|Thiago|Nóbrega|11/13/2018|Fortaleza|1600|NaN|3200|
|338|2564|HL4379|Televisão|5|Guido|Monteiro|11/15/2018|Fortaleza|2500|NaN|12500|
|339|2570|HL1918|iPhone|3|João|Rodrigues|9/12/2018|Fortaleza|5300|NaN|15900|
|340|2576|HL4379|Televisão|2|Laura|Araujo|1/17/2018|Fortaleza|2500|NaN|5000|
|341|2578|HL8851|Notebook|5|Paula|Cavalcanti|12/25/2018|Fortaleza|3500|NaN|17500|
|342|2581|HL4379|Televisão|3|Breno|Britto|6/8/2018|Fortaleza|2500|NaN|7500|
|343|2587|HL1918|iPhone|4|Giovana|Vilela|10/10/2018|Fortaleza|5300|NaN|21200|
|344|2589|HL4379|Televisão|5|Breno|Costa|2/4/2018|Fortaleza|2500|NaN|12500|
|345|2590|HL9962|Android|3|Raul|Junqueira|4/14/2018|Fortaleza|3400|NaN|10200|
|346|2592|HL1918|iPhone|2|Rafaella|Mello|8/16/2018|Fortaleza|5300|NaN|10600|
|347|2593|HL7348|SmartWatch|3|Gabrielle|Figueiredo|5/29/2018|Fortaleza|1400|NaN|4200|
|348|2601|HL1918|iPhone|3|Caio|Moura|2/22/2018|Fortaleza|5300|NaN|15900|
|349|2610|HL7348|SmartWatch|2|Rafael|Wajnsztok|9/12/2018|Fortaleza|1400|NaN|2800|
|350|2612|HL1148|Câmera|4|Adriana|Carneiro|6/12/2018|Fortaleza|2100|NaN|8400|
|351|2620|HL1918|iPhone|3|Patrick|Silva|9/25/2018|Fortaleza|5300|NaN|15900|
|352|2626|HL1918|iPhone|3|Lucas|Machado|11/28/2018|Fortaleza|5300|NaN|15900|
|353|2630|HL1148|Câmera|1|Clara|Silveira|4/27/2018|Fortaleza|2100|NaN|2100|
|354|2637|HL2714|Tablet|1|Júlio|Freire|4/16/2018|Fortaleza|1600|NaN|1600|
|355|2643|HL1918|iPhone|2|Giulia|Lopes|3/4/2018|Fortaleza|5300|NaN|10600|
|356|2644|HL1918|iPhone|2|Pedro|Oliveira|11/27/2018|Fortaleza|5300|NaN|10600|
|357|2657|HL1918|iPhone|2|Elena|Barreto|7/19/2018|Fortaleza|5300|NaN|10600|
|358|2658|HL1148|Câmera|1|Adriane|Chagas|5/30/2018|Fortaleza|2100|NaN|2100|
|359|2662|HL9962|Android|4|Luiza|Marques|6/17/2018|Fortaleza|3400|NaN|13600|
|360|2664|HL8851|Notebook|2|Anna|Silva|1/17/2018|Fortaleza|3500|NaN|7000|
|361|2676|HL2714|Tablet|2|Bianca|Procaci|12/25/2018|Fortaleza|1600|NaN|3200|
|362|2677|HL7348|SmartWatch|2|Clara|Bruno|9/16/2018|Fortaleza|1400|NaN|2800|
|363|2679|HL7348|SmartWatch|1|Jorge|Fonseca|5/12/2018|Fortaleza|1400|NaN|1400|
|364|2685|HL1918|iPhone|2|João|Costa|5/12/2018|Fortaleza|5300|NaN|10600|
|365|2690|HL1918|iPhone|1|Camilla|Vieira|11/28/2018|Fortaleza|5300|NaN|5300|
|366|2691|HL7348|SmartWatch|2|Guilherme|Jordao|4/28/2018|Fortaleza|1400|NaN|2800|
|367|2692|HL4379|Televisão|5|Raíssa|Oliveira|5/4/2018|Fortaleza|2500|NaN|12500|
|368|2699|HL1918|iPhone|2|Joao|Silva|11/12/2018|Fortaleza|5300|NaN|10600|
|369|2702|HL8851|Notebook|1|Mateus|Polastri|4/30/2018|Fortaleza|3500|NaN|3500|
|370|2708|HL2714|Tablet|2|Leticia|Mesquita|9/5/2018|Fortaleza|1600|NaN|3200|
|371|2738|HL9962|Android|1|João|Bach|10/11/2018|Fortaleza|3400|NaN|3400|
|372|2739|HL1148|Câmera|5|Gustavo|Aragão|3/1/2018|Fortaleza|2100|NaN|10500|
|373|2744|HL1918|iPhone|4|Pedro|Cardoso|10/23/2018|Fortaleza|5300|NaN|21200|
|374|2758|HL1918|iPhone|1|Júlio|Fraga|3/26/2018|Fortaleza|5300|NaN|5300|
|375|2776|HL2714|Tablet|1|Vitor|Arruda|9/17/2018|Fortaleza|1600|NaN|1600|
|376|2784|HL1148|Câmera|4|Ulisses|Quinto|11/22/2018|Fortaleza|2100|NaN|8400|
|377|2790|HL8851|Notebook|2|Beatriz|Cavalcanti|3/22/2018|Fortaleza|3500|NaN|7000|
|378|2798|HL8851|Notebook|1|Mariane|Ferreira|11/14/2018|Fortaleza|3500|NaN|3500|
|379|2828|HL2714|Tablet|1|Lorena|Carvalho|4/19/2018|Fortaleza|1600|NaN|1600|
|380|2837|HL4379|Televisão|1|Matheus|Afonso|2/6/2018|Fortaleza|2500|NaN|2500|
|381|2851|HL1918|iPhone|1|Vanessa|Neves|9/9/2018|Fortaleza|5300|NaN|5300|
|382|2854|HL9962|Android|5|Rojane|Lima|12/17/2018|Fortaleza|3400|NaN|17000|
|383|2858|HL4379|Televisão|4|Breno|Quinto|10/9/2018|Fortaleza|2500|NaN|10000|
|384|2859|HL2714|Tablet|1|Matheus|Silva|7/7/2018|Fortaleza|1600|NaN|1600|
|385|2860|HL1918|iPhone|1|Isaac|Santos|3/6/2018|Fortaleza|5300|NaN|5300|
|386|2879|HL4379|Televisão|1|Eduardo|Ferreira|5/11/2018|Fortaleza|2500|NaN|2500|
|387|2884|HL2714|Tablet|4|Tadeu|Nakayama|5/3/2018|Fortaleza|1600|NaN|6400|
|388|2887|HL4379|Televisão|3|Lorena|Carvalho|3/15/2018|Fortaleza|2500|NaN|7500|
|389|2906|HL1148|Câmera|3|Fernanda|Coutinho|1/5/2018|Fortaleza|2100|NaN|6300|
|390|2922|HL8851|Notebook|2|Jonas|Gomes|4/17/2018|Fortaleza|3500|NaN|7000|
|391|2927|HL8851|Notebook|5|Maria|Motta|11/6/2018|Fortaleza|3500|NaN|17500|
|392|2928|HL7348|SmartWatch|3|Leandro|Ferreira|4/29/2018|Fortaleza|1400|NaN|4200|
|393|2931|HL1918|iPhone|4|Diego|Marchesi|10/4/2018|Fortaleza|5300|NaN|21200|
|394|2941|HL1148|Câmera|3|Beatriz|Li|10/9/2018|Fortaleza|2100|NaN|6300|
|395|2946|HL1918|iPhone|2|Philipe|Morete|9/24/2018|Fortaleza|5300|NaN|10600|
|396|2951|HL7348|SmartWatch|1|Letícia|Leal|8/2/2018|Fortaleza|1400|NaN|1400|
|397|2958|HL2714|Tablet|4|Célio|Xavier|8/13/2018|Fortaleza|1600|NaN|6400|
|398|2960|HL1918|iPhone|3|Luíza|Garcia|9/16/2018|Fortaleza|5300|NaN|15900|
|399|2961|HL4379|Televisão|5|Raissa|Maia|3/27/2018|Fortaleza|2500|NaN|12500|
|400|2971|HL2714|Tablet|5|Natalia|Accioly|6/24/2018|Fortaleza|1600|NaN|8000|
|401|2976|HL1918|iPhone|3|Leonardo|Ferreira|8/10/2018|Fortaleza|5300|NaN|15900|
|402|2984|HL8851|Notebook|2|Marianna|Pestana|8/13/2018|Fortaleza|3500|NaN|7000|
|403|2989|HL8851|Notebook|5|Tainah|Nogueira|12/28/2018|Fortaleza|3500|NaN|17500|
|404|2998|HL8851|Notebook|5|Nathan|Cunha|3/30/2018|Fortaleza|3500|NaN|17500|
|405|3001|HL1918|iPhone|3|Rodrigo|Alves|2/14/2018|Fortaleza|5300|NaN|15900|
|406|3003|HL4379|Televisão|4|Larissa|Vasconcellos|6/3/2018|Fortaleza|2500|NaN|10000|
|407|3005|HL1918|iPhone|4|Alexandre|Rodriguez|7/18/2018|Fortaleza|5300|NaN|21200|
|408|3008|HL1148|Câmera|3|Carolina|Siqueira|10/6/2018|Fortaleza|2100|NaN|6300|
|409|3021|HL1918|iPhone|1|Fernanda|Bhering|9/21/2018|Fortaleza|5300|NaN|5300|
|410|3024|HL2714|Tablet|4|Diego|Marchesi|8/6/2018|Fortaleza|1600|NaN|6400|
|411|3034|HL8851|Notebook|3|Andre|Nóbrega|4/20/2018|Fortaleza|3500|NaN|10500|
|412|3035|HL7348|SmartWatch|5|Beatriz|Li|6/24/2018|Fortaleza|1400|NaN|7000|
|413|3036|HL7348|SmartWatch|3|Julie|Ferreira|8/17/2018|Fortaleza|1400|NaN|4200|
|414|3048|HL1918|iPhone|3|Giselia|Thiele|5/4/2018|Fortaleza|5300|NaN|15900|
|415|3060|HL1918|iPhone|1|Thomáz|Bôas|8/24/2018|Fortaleza|5300|NaN|5300|
|416|3062|HL4379|Televisão|3|Danilo|Rubim|3/24/2018|Fortaleza|2500|NaN|7500|
|417|3069|HL2714|Tablet|2|Ylana|Teraoka|9/2/2018|Fortaleza|1600|NaN|3200|
|418|3076|HL8851|Notebook|5|Pedro|Martins|1/12/2018|Fortaleza|3500|NaN|17500|
|419|3081|HL1918|iPhone|1|Elaine|Santos|12/2/2018|Fortaleza|5300|NaN|5300|
|420|3094|HL1918|iPhone|2|Gabriel|Azevedo|2/5/2018|Fortaleza|5300|NaN|10600|
|421|3100|HL1918|iPhone|4|Jorge|Fonseca|12/14/2018|Fortaleza|5300|NaN|21200|
|422|3101|HL2714|Tablet|4|Roberta|Teixeira|11/15/2018|Fortaleza|1600|NaN|6400|
|423|3105|HL1148|Câmera|3|Guilherme|Santos|6/6/2018|Fortaleza|2100|NaN|6300|
|424|3106|HL1148|Câmera|1|Leticia|Mesquita|2/28/2018|Fortaleza|2100|NaN|2100|
|425|3107|HL4379|Televisão|3|Ana|Soledade|10/2/2018|Fortaleza|2500|NaN|7500|
|426|3117|HL1148|Câmera|2|Bárbara|Cavalcante|10/15/2018|Fortaleza|2100|NaN|4200|
|427|3121|HL4379|Televisão|1|Marina|Mesquita|10/6/2018|Fortaleza|2500|NaN|2500|
|428|3136|HL7348|SmartWatch|4|Adriane|Chagas|11/18/2018|Fortaleza|1400|NaN|5600|
|429|3141|HL7348|SmartWatch|4|Roberto|Nogueira|5/4/2018|Fortaleza|1400|NaN|5600|
|430|3143|HL4379|Televisão|2|Antônio|Oliveira|12/2/2018|Fortaleza|2500|NaN|5000|
|431|3149|HL4379|Televisão|2|Amanda|Braga|6/12/2018|Fortaleza|2500|NaN|5000|
|432|3161|HL4379|Televisão|4|Fernanda|Junior|12/5/2018|Fortaleza|2500|NaN|10000|
|433|3182|HL8851|Notebook|5|Bianca|Piero|12/8/2018|Fortaleza|3500|NaN|17500|
|434|3184|HL9962|Android|1|Myllena|Corrêa|12/24/2018|Fortaleza|3400|NaN|3400|
|435|3188|HL2714|Tablet|1|Carlos|Mesquita|8/14/2018|Fortaleza|1600|NaN|1600|
|436|3189|HL7348|SmartWatch|4|Giuseppe|Bhering|10/28/2018|Fortaleza|1400|NaN|5600|
|437|3208|HL4379|Televisão|5|Marina|Gama|4/20/2018|Fortaleza|2500|NaN|12500|
|438|3222|HL9962|Android|5|Caroline|Aquino|5/25/2018|Fortaleza|3400|NaN|17000|
|439|3232|HL4379|Televisão|5|Rebeca|Taylor|5/12/2018|Fortaleza|2500|NaN|12500|
|440|3234|HL4379|Televisão|1|Dykson|Silva|3/2/2018|Fortaleza|2500|NaN|2500|
|441|3240|HL8851|Notebook|2|Lívia|Marques|11/11/2018|Fortaleza|3500|NaN|7000|
|442|3247|HL1918|iPhone|5|João|Ribeiro|6/21/2018|Fortaleza|5300|NaN|26500|
|443|3257|HL8851|Notebook|2|João|Peçanha|9/19/2018|Fortaleza|3500|NaN|7000|
|444|3266|HL2714|Tablet|2|Desirée|Heimlich|8/22/2018|Fortaleza|1600|NaN|3200|
|445|3269|HL1918|iPhone|1|João|Monteiro|6/30/2018|Fortaleza|5300|NaN|5300|
|446|3275|HL8851|Notebook|1|Lucas|Lemos|3/16/2018|Fortaleza|3500|NaN|3500|
|447|3290|HL1918|iPhone|2|Rodrigo|Mendes|7/5/2018|Fortaleza|5300|NaN|10600|
|448|3297|HL8851|Notebook|4|Tainah|Nogueira|8/19/2018|Fortaleza|3500|NaN|14000|
|449|3299|HL1918|iPhone|4|Júlia|Almeida|6/18/2018|Fortaleza|5300|NaN|21200|
|450|3325|HL1918|iPhone|5|Thays|Castro|8/16/2018|Fortaleza|5300|NaN|26500|
|451|3326|HL7348|SmartWatch|1|Wilson|Meirelles|12/17/2018|Fortaleza|1400|NaN|1400|
|452|3327|HL9962|Android|5|Rogério|Gentile|9/4/2018|Fortaleza|3400|NaN|17000|
|453|3332|HL2714|Tablet|5|Rafaela|Gomes|4/17/2018|Fortaleza|1600|NaN|8000|
|454|3347|HL4379|Televisão|2|Giulia|Lopes|5/9/2018|Fortaleza|2500|NaN|5000|
|455|3348|HL7348|SmartWatch|5|Paula|Carneiro|8/28/2018|Fortaleza|1400|NaN|7000|
|456|3355|HL4379|Televisão|3|Rodrigo|Mendes|3/31/2018|Fortaleza|2500|NaN|7500|
|457|3364|HL7348|SmartWatch|5|Carolina|Vasconcelos|2/23/2018|Fortaleza|1400|NaN|7000|
|458|3374|HL4379|Televisão|3|Julia|Aliani|11/27/2018|Fortaleza|2500|NaN|7500|
|459|3380|HL8851|Notebook|5|Miguel|Carneiro|2/9/2018|Fortaleza|3500|NaN|17500|
|460|3381|HL1918|iPhone|5|Pedro|Ayres|2/8/2018|Fortaleza|5300|NaN|26500|
|461|3390|HL8851|Notebook|5|Larissa|Cruz|7/23/2018|Fortaleza|3500|NaN|17500|
|462|3394|HL4379|Televisão|4|Camilla|Guimarães|2/19/2018|Fortaleza|2500|NaN|10000|
|463|3400|HL1918|iPhone|1|Stephanie|Gonçalves|12/1/2018|Fortaleza|5300|NaN|5300|
|464|3403|HL8851|Notebook|3|Diego|Rodrigues|4/22/2018|Fortaleza|3500|NaN|10500|
|465|3407|HL9962|Android|2|Jéssica|Netto|6/14/2018|Fortaleza|3400|NaN|6800|
|466|3410|HL7348|SmartWatch|5|Caroline|Cavalcanti|10/11/2018|Fortaleza|1400|NaN|7000|
|467|3416|HL1918|iPhone|5|Iuri|Barbosa|2/22/2018|Fortaleza|5300|NaN|26500|
|468|3417|HL1918|iPhone|3|Paola|Abreu|10/10/2018|Fortaleza|5300|NaN|15900|
|469|3441|HL9962|Android|1|Marcela|Johnson|1/6/2018|Fortaleza|3400|NaN|3400|
|470|3448|HL7348|SmartWatch|2|Daniela|Rosa|2/2/2018|Fortaleza|1400|NaN|2800|
|471|3450|HL7348|SmartWatch|2|Gabriel|Brito|5/12/2018|Fortaleza|1400|NaN|2800|
|472|3453|HL1918|iPhone|2|Rodrigo|Bruno|7/24/2018|Fortaleza|5300|NaN|10600|
|473|3454|HL4379|Televisão|4|Vitor|Boccaletti|5/27/2018|Fortaleza|2500|NaN|10000|
|474|3455|HL1918|iPhone|2|Leandro|Melo|7/14/2018|Fortaleza|5300|NaN|10600|
|475|3457|HL2714|Tablet|2|João|Bach|5/11/2018|Fortaleza|1600|NaN|3200|
|476|3458|HL1148|Câmera|2|Gabriela|Aliani|3/16/2018|Fortaleza|2100|NaN|4200|
|477|3488|HL1918|iPhone|3|Silvio|Provenzano|4/16/2018|Fortaleza|5300|NaN|15900|
|478|3494|HL2714|Tablet|3|Wendela|Mariz|1/19/2018|Fortaleza|1600|NaN|4800|
|479|3495|HL4379|Televisão|1|João|Fonseca|5/13/2018|Fortaleza|2500|NaN|2500|
|480|3501|HL1148|Câmera|3|João|Monteiro|7/5/2018|Fortaleza|2100|NaN|6300|
|481|3504|HL7348|SmartWatch|4|Pedro|Pereira|8/25/2018|Fortaleza|1400|NaN|5600|
|482|3507|HL1148|Câmera|1|Rafael|Carneiro|10/7/2018|Fortaleza|2100|NaN|2100|
|483|3512|HL8851|Notebook|1|Mariana|Miranda|9/18/2018|Fortaleza|3500|NaN|3500|
|484|3533|HL4379|Televisão|3|Renan|Nascimento|9/12/2018|Fortaleza|2500|NaN|7500|
|485|3534|HL2714|Tablet|3|Bianca|Allevato|11/9/2018|Fortaleza|1600|NaN|4800|
|486|3542|HL1148|Câmera|3|Carlos|Silva|6/4/2018|Fortaleza|2100|NaN|6300|
|487|3543|HL9962|Android|1|Lucas|Aragão|11/28/2018|Fortaleza|3400|NaN|3400|
|488|3549|HL1148|Câmera|3|Fabio|Boccaletti|10/6/2018|Fortaleza|2100|NaN|6300|
|489|3550|HL1918|iPhone|5|Guilherme|Seixas|5/25/2018|Fortaleza|5300|NaN|26500|
|490|3554|HL9962|Android|1|Victor|Ferreira|11/20/2018|Fortaleza|3400|NaN|3400|
|491|3574|HL1918|iPhone|5|Rebeca|Taylor|12/16/2018|Fortaleza|5300|NaN|26500|
|492|3580|HL1918|iPhone|5|Breno|Britto|1/24/2018|Fortaleza|5300|NaN|26500|
|493|3585|HL4379|Televisão|5|Ulisses|Arruda|2/15/2018|Fortaleza|2500|NaN|12500|
|494|3586|HL1918|iPhone|3|Thainá|Binello|1/22/2018|Fortaleza|5300|NaN|15900|
|495|3594|HL4379|Televisão|5|Carlos|Souza|3/2/2018|Fortaleza|2500|NaN|12500|
|496|3597|HL8851|Notebook|1|Gabriela|Fernandes|6/21/2018|Fortaleza|3500|NaN|3500|
|497|3601|HL1918|iPhone|4|Carlos|Araujo|5/26/2018|Fortaleza|5300|NaN|21200|
|498|3613|HL8851|Notebook|2|Douglas|Rodrigues|2/24/2018|Fortaleza|3500|NaN|7000|
|499|3615|HL1918|iPhone|3|Livia|Corrêa|7/21/2018|Fortaleza|5300|NaN|15900|
|500|3650|HL8851|Notebook|2|Ives|Pinheiro|11/3/2018|Fortaleza|3500|NaN|7000|
|501|3654|HL2714|Tablet|5|Izabel|Miura|7/8/2018|Fortaleza|1600|NaN|8000|
|502|3658|HL1148|Câmera|5|Lucas|Chagas|7/13/2018|Fortaleza|2100|NaN|10500|
|503|3667|HL1148|Câmera|3|Juan|Barbosa|1/21/2018|Fortaleza|2100|NaN|6300|
|504|3679|HL8851|Notebook|5|Leonardo|Ferreira|8/5/2018|Fortaleza|3500|NaN|17500|
|505|3681|HL9962|Android|5|Thiago|Lima|9/18/2018|Fortaleza|3400|NaN|17000|
|506|3690|HL9962|Android|3|Paula|Calbucci|10/23/2018|Fortaleza|3400|NaN|10200|
|507|3696|HL1918|iPhone|4|Marina|Correa|4/5/2018|Fortaleza|5300|NaN|21200|
|508|3698|HL7348|SmartWatch|5|Sandy|Moreira|12/20/2018|Fortaleza|1400|NaN|7000|
|509|3709|HL7348|SmartWatch|2|Guilherme|Lima|5/21/2018|Fortaleza|1400|NaN|2800|
|510|3714|HL1918|iPhone|4|Yasser|Calbucci|9/15/2018|Fortaleza|5300|NaN|21200|
|511|3716|HL8851|Notebook|3|Carlos|Portela|7/25/2018|Fortaleza|3500|NaN|10500|
|512|3718|HL1918|iPhone|1|Breno|Varella|4/11/2018|Fortaleza|5300|NaN|5300|
|513|3724|HL4379|Televisão|4|David|Vasconcelos|9/16/2018|Fortaleza|2500|NaN|10000|
|514|3741|HL1918|iPhone|5|Matheus|Sapir|3/16/2018|Fortaleza|5300|NaN|26500|
|515|3742|HL2714|Tablet|1|Glenda|Santos|12/21/2018|Fortaleza|1600|NaN|1600|
|516|3755|HL8851|Notebook|3|Sandy|Ribeiro|4/26/2018|Fortaleza|3500|NaN|10500|
|517|3760|HL7348|SmartWatch|3|Laís|Oliveira|12/10/2018|Fortaleza|1400|NaN|4200|
|518|3769|HL7348|SmartWatch|5|Mariana|Baptista|2/28/2018|Fortaleza|1400|NaN|7000|
|519|3770|HL8851|Notebook|1|Rachel|Silva|1/25/2018|Fortaleza|3500|NaN|3500|
|520|3785|HL1918|iPhone|4|Anna|Silva|5/3/2018|Fortaleza|5300|NaN|21200|
|521|3787|HL1148|Câmera|3|Juliana|Barreira|7/26/2018|Fortaleza|2100|NaN|6300|
|522|3790|HL7348|SmartWatch|2|Felipe|Mello|4/12/2018|Fortaleza|1400|NaN|2800|
|523|3794|HL1918|iPhone|5|Gabriel|Puntel|8/23/2018|Fortaleza|5300|NaN|26500|
|524|3797|HL2714|Tablet|2|Fernanda|Junior|7/11/2018|Fortaleza|1600|NaN|3200|
|525|3799|HL1918|iPhone|1|Julia|Figueiredo|5/29/2018|Fortaleza|5300|NaN|5300|
|526|3807|HL7348|SmartWatch|2|Elena|Barreto|1/29/2018|Fortaleza|1400|NaN|2800|
|527|3812|HL4379|Televisão|4|Victor|Lira|9/11/2018|Fortaleza|2500|NaN|10000|
|528|3823|HL7348|SmartWatch|3|Luíza|Garcia|8/31/2018|Fortaleza|1400|NaN|4200|
|529|3830|HL9962|Android|1|Priscila|Carvalho|1/3/2018|Fortaleza|3400|NaN|3400|
|530|3833|HL7348|SmartWatch|2|Raphael|Ferman|11/3/2018|Fortaleza|1400|NaN|2800|
|531|3834|HL4379|Televisão|2|Eduardo|Veiga|3/9/2018|Fortaleza|2500|NaN|5000|
|532|3838|HL1918|iPhone|3|Tiago|Pereira|4/23/2018|Fortaleza|5300|NaN|15900|
|533|3841|HL1918|iPhone|3|André|Alves|4/5/2018|Fortaleza|5300|NaN|15900|
|534|3862|HL1918|iPhone|2|Matheus|Tostes|6/10/2018|Fortaleza|5300|NaN|10600|
|535|3867|HL2714|Tablet|5|Victor|Lira|7/23/2018|Fortaleza|1600|NaN|8000|
|536|3869|HL7348|SmartWatch|5|Marina|Perdomo|1/14/2018|Fortaleza|1400|NaN|7000|
|537|3878|HL9962|Android|1|Mariane|Racy|8/25/2018|Fortaleza|3400|NaN|3400|
|538|3885|HL4379|Televisão|2|Bruna|Brandao|1/18/2018|Fortaleza|2500|NaN|5000|
|539|3894|HL4379|Televisão|3|Camila|Sobral|12/7/2018|Fortaleza|2500|NaN|7500|
|540|3916|HL7348|SmartWatch|2|Daniela|Andrada|11/9/2018|Fortaleza|1400|NaN|2800|
|541|3928|HL7348|SmartWatch|1|Isabella|Montanholi|5/8/2018|Fortaleza|1400|NaN|1400|
|542|3936|HL8851|Notebook|1|Carlos|Cardoso|6/17/2018|Fortaleza|3500|NaN|3500|
|543|3942|HL4379|Televisão|2|Anna|Figueiredo|11/23/2018|Fortaleza|2500|NaN|5000|
|544|3945|HL4379|Televisão|4|Juliana|Silva|11/17/2018|Fortaleza|2500|NaN|10000|
|545|3946|HL1918|iPhone|5|Anna|Maia|10/3/2018|Fortaleza|5300|NaN|26500|
|546|3951|HL1918|iPhone|1|Izabel|Miura|8/7/2018|Fortaleza|5300|NaN|5300|
|547|3955|HL1918|iPhone|3|Lucas|Lemos|9/30/2018|Fortaleza|5300|NaN|15900|
|548|3958|HL2714|Tablet|3|Adrielle|Gabriel|3/21/2018|Fortaleza|1600|NaN|4800|
|549|3966|HL4379|Televisão|4|Breno|Costa|2/28/2018|Fortaleza|2500|NaN|10000|
|550|3969|HL1918|iPhone|3|Bianca|Tatsch|3/15/2018|Fortaleza|5300|NaN|15900|
|551|3970|HL4379|Televisão|3|Caio|Caldas|10/11/2018|Fortaleza|2500|NaN|7500|
|552|3975|HL4379|Televisão|3|Caio|Vianna|11/18/2018|Fortaleza|2500|NaN|7500|
|553|3984|HL2714|Tablet|5|Vitor|Boccaletti|3/31/2018|Fortaleza|1600|NaN|8000|
|554|3989|HL1918|iPhone|3|Samara|Pinto|3/23/2018|Fortaleza|5300|NaN|15900|
|555|3996|HL1148|Câmera|5|Rodrigo|Feijo|8/16/2018|Fortaleza|2100|NaN|10500|
|556|4013|HL4379|Televisão|1|Lucas|Aragão|8/10/2018|Fortaleza|2500|NaN|2500|
|557|4014|HL1148|Câmera|1|Nathan|Morelli|4/16/2018|Fortaleza|2100|NaN|2100|
|558|4020|HL1148|Câmera|4|Thiago|Costa|1/18/2018|Fortaleza|2100|NaN|8400|
|559|4021|HL8851|Notebook|2|Breno|Varella|5/12/2018|Fortaleza|3500|NaN|7000|
|560|4027|HL1918|iPhone|4|Deysiane|Medronho|7/11/2018|Fortaleza|5300|NaN|21200|
|561|4040|HL7348|SmartWatch|3|Ravena|Bhering|2/16/2018|Fortaleza|1400|NaN|4200|
|562|4052|HL7348|SmartWatch|2|Elena|Barreto|11/10/2018|Fortaleza|1400|NaN|2800|
|563|4075|HL1918|iPhone|5|Juliana|Souza|3/3/2018|Fortaleza|5300|NaN|26500|
|564|4080|HL2714|Tablet|2|Stephanie|Novak|11/20/2018|Fortaleza|1600|NaN|3200|
|565|4090|HL1918|iPhone|1|Victor|Franco|10/24/2018|Fortaleza|5300|NaN|5300|
|566|4096|HL4379|Televisão|2|Mateus|Duque|2/21/2018|Fortaleza|2500|NaN|5000|
|567|4110|HL1918|iPhone|2|Izabel|Miura|3/6/2018|Fortaleza|5300|NaN|10600|
|568|4113|HL1918|iPhone|3|Guilherme|Lima|11/9/2018|Fortaleza|5300|NaN|15900|
|569|4130|HL2714|Tablet|1|Beatriz|Perdomo|7/21/2018|Fortaleza|1600|NaN|1600|
|570|4132|HL2714|Tablet|1|Itai|Puntel|7/5/2018|Fortaleza|1600|NaN|1600|
|571|4146|HL7348|SmartWatch|4|Pedro|Rodrigues|10/27/2018|Fortaleza|1400|NaN|5600|
|572|4150|HL1148|Câmera|5|Camila|Bastazini|12/12/2018|Fortaleza|2100|NaN|10500|
|573|4161|HL1918|iPhone|2|Ana|Miura|5/10/2018|Fortaleza|5300|NaN|10600|
|574|4172|HL9962|Android|4|Matheus|Gomes|11/28/2018|Fortaleza|3400|NaN|13600|
|575|4173|HL1918|iPhone|1|Fernanda|Figueiredo|12/21/2018|Fortaleza|5300|NaN|5300|
|576|4181|HL1918|iPhone|2|Luiz|Xavier|7/10/2018|Fortaleza|5300|NaN|10600|
|577|4185|HL7348|SmartWatch|1|Rafael|Carneiro|11/13/2018|Fortaleza|1400|NaN|1400|
|578|4192|HL1918|iPhone|1|Beatriz|Rocha|1/29/2018|Fortaleza|5300|NaN|5300|
|579|4206|HL1918|iPhone|2|Jonas|Gomes|11/29/2018|Fortaleza|5300|NaN|10600|
|580|4209|HL2714|Tablet|3|Gabrielle|Costa|6/18/2018|Fortaleza|1600|NaN|4800|
|581|4223|HL7348|SmartWatch|2|Mariana|Miranda|3/1/2018|Fortaleza|1400|NaN|2800|
|582|4231|HL1918|iPhone|1|Marina|Marins|3/14/2018|Fortaleza|5300|NaN|5300|
|583|4232|HL1918|iPhone|3|Philipe|Morete|5/11/2018|Fortaleza|5300|NaN|15900|
|584|4235|HL2714|Tablet|3|Fernanda|Ferreira|2/26/2018|Fortaleza|1600|NaN|4800|
|585|4243|HL9962|Android|5|Victor|Gomes|6/26/2018|Fortaleza|3400|NaN|17000|
|586|4248|HL7348|SmartWatch|1|David|Assumpção|9/11/2018|Fortaleza|1400|NaN|1400|
|587|4252|HL1918|iPhone|4|Lívia|Tanaka|11/17/2018|Fortaleza|5300|NaN|21200|
|588|4262|HL8851|Notebook|2|Roberta|Nogueira|5/6/2018|Fortaleza|3500|NaN|7000|
|589|4264|HL1918|iPhone|4|Pedro|Conceição|2/9/2018|Fortaleza|5300|NaN|21200|
|590|4271|HL1148|Câmera|1|Eduardo|Nunes|6/21/2018|Fortaleza|2100|NaN|2100|
|591|4273|HL1918|iPhone|2|Jeferson|Sone|4/30/2018|Fortaleza|5300|NaN|10600|
|592|4284|HL9962|Android|5|Guilherme|Vianna|11/12/2018|Fortaleza|3400|NaN|17000|
|593|4291|HL1918|iPhone|1|Danilo|Rubim|9/29/2018|Fortaleza|5300|NaN|5300|
|594|4310|HL2714|Tablet|4|João|Pedrazza|4/25/2018|Fortaleza|1600|NaN|6400|
|595|4322|HL8851|Notebook|4|Sthefeson|Pereira|2/11/2018|Fortaleza|3500|NaN|14000|
|596|4323|HL9962|Android|4|Rafael|Carneiro|8/13/2018|Fortaleza|3400|NaN|13600|
|597|4326|HL1918|iPhone|2|Natalia|Marinho|12/29/2018|Fortaleza|5300|NaN|10600|
|598|4334|HL4379|Televisão|3|Izabel|Lopes|10/26/2018|Fortaleza|2500|NaN|7500|
|599|4337|HL9962|Android|1|Lucas|Valim|8/24/2018|Fortaleza|3400|NaN|3400|
|600|4339|HL7348|SmartWatch|5|Guilherme|Vianna|9/14/2018|Fortaleza|1400|NaN|7000|
|601|4352|HL1918|iPhone|3|Diego|Mello|10/29/2018|Fortaleza|5300|NaN|15900|
|602|4353|HL8851|Notebook|2|Priscila|Suzano|4/29/2018|Fortaleza|3500|NaN|7000|
|603|4367|HL1918|iPhone|4|Luiz|Campista|1/24/2018|Fortaleza|5300|NaN|21200|
|604|4369|HL2714|Tablet|4|Wendela|Mariz|3/7/2018|Fortaleza|1600|NaN|6400|
|605|4371|HL4379|Televisão|4|Ulisses|Filho|1/2/2018|Fortaleza|2500|NaN|10000|
|606|4382|HL7348|SmartWatch|3|Henrique|Villanova|1/2/2018|Fortaleza|1400|NaN|4200|
|607|4393|HL8851|Notebook|4|Bruna|Silva|3/9/2018|Fortaleza|3500|NaN|14000|
|608|4399|HL8851|Notebook|5|Gabriella|Sagrillo|4/25/2018|Fortaleza|3500|NaN|17500|
|609|4405|HL1918|iPhone|5|Beatriz|Santos|8/20/2018|Fortaleza|5300|NaN|26500|
|610|4418|HL1148|Câmera|1|Aline|Morais|8/9/2018|Fortaleza|2100|NaN|2100|
|611|4420|HL4379|Televisão|5|Gabriel|Pereira|2/13/2018|Fortaleza|2500|NaN|12500|
|612|4439|HL2714|Tablet|1|Lucas|Lima|10/17/2018|Fortaleza|1600|NaN|1600|
|613|4446|HL1148|Câmera|3|Giuseppe|Bhering|6/21/2018|Fortaleza|2100|NaN|6300|
|614|4454|HL4379|Televisão|5|Joyce|Souza|4/15/2018|Fortaleza|2500|NaN|12500|
|615|4464|HL4379|Televisão|3|Camilla|Cardeman|4/11/2018|Fortaleza|2500|NaN|7500|
|616|4483|HL1918|iPhone|1|Alessandra|Martins|4/8/2018|Fortaleza|5300|NaN|5300|
|617|4492|HL1918|iPhone|1|Roberto|Mattos|6/7/2018|Fortaleza|5300|NaN|5300|
|618|4496|HL7348|SmartWatch|2|Daniel|Valente|8/28/2018|Fortaleza|1400|NaN|2800|
|619|4504|HL1918|iPhone|3|Renan|Freire|7/17/2018|Fortaleza|5300|NaN|15900|
|620|4506|HL1148|Câmera|3|Lucas|Rocha|4/5/2018|Fortaleza|2100|NaN|6300|
|621|4512|HL2714|Tablet|3|Luis|Souza|7/5/2018|Fortaleza|1600|NaN|4800|
|622|4514|HL1918|iPhone|1|Luíza|Goulart|2/5/2018|Fortaleza|5300|NaN|5300|
|623|4517|HL2714|Tablet|3|Henrique|Lencastre|11/28/2018|Fortaleza|1600|NaN|4800|
|624|4519|HL1918|iPhone|4|Helvio|Pedrosa|11/22/2018|Fortaleza|5300|NaN|21200|
|625|4524|HL9962|Android|4|Philipe|Morete|3/30/2018|Fortaleza|3400|NaN|13600|
|626|4527|HL2714|Tablet|4|Silvio|Fahrnholz|12/17/2018|Fortaleza|1600|NaN|6400|
|627|4530|HL1918|iPhone|2|Jessica|Ferreira|9/22/2018|Fortaleza|5300|NaN|10600|
|628|4535|HL1148|Câmera|4|Catarina|Teixeira|7/9/2018|Fortaleza|2100|NaN|8400|
|629|4540|HL1148|Câmera|3|Amanda|Gontijo|8/12/2018|Fortaleza|2100|NaN|6300|
|630|4542|HL8851|Notebook|1|Guilherme|Lima|12/2/2018|Fortaleza|3500|NaN|3500|
|631|4549|HL2714|Tablet|2|João|Guadagnino|6/24/2018|Fortaleza|1600|NaN|3200|
|632|4559|HL1918|iPhone|1|Victor|Zakhm|2/16/2018|Fortaleza|5300|NaN|5300|
|633|4567|HL9962|Android|3|Joao|Pereira|2/4/2018|Fortaleza|3400|NaN|10200|
|634|4585|HL1148|Câmera|2|Matheus|Ramos|4/3/2018|Fortaleza|2100|NaN|4200|
|635|4593|HL4379|Televisão|3|Lunna|Vannier|12/22/2018|Fortaleza|2500|NaN|7500|
|636|4600|HL1148|Câmera|4|Luis|Oliveira|11/16/2018|Fortaleza|2100|NaN|8400|
|637|4602|HL7348|SmartWatch|1|João|Siqueira|4/25/2018|Fortaleza|1400|NaN|1400|
|638|4607|HL1918|iPhone|1|Raíssa|Oliveira|5/6/2018|Fortaleza|5300|NaN|5300|
|639|4610|HL9962|Android|1|Leandro|Rodrigues|1/3/2018|Fortaleza|3400|NaN|3400|
|640|4614|HL2714|Tablet|5|Juliana|Silva|10/8/2018|Fortaleza|1600|NaN|8000|
|641|4615|HL1918|iPhone|2|Gabrielle|Wanderley|10/3/2018|Fortaleza|5300|NaN|10600|
|642|4618|HL4379|Televisão|3|Ulisses|Filho|11/12/2018|Fortaleza|2500|NaN|7500|
|643|4620|HL4379|Televisão|5|Carolina|Motta|8/29/2018|Fortaleza|2500|NaN|12500|
|644|4630|HL2714|Tablet|2|Luana|Santana|6/24/2018|Fortaleza|1600|NaN|3200|
|645|4642|HL9962|Android|4|Cícero|Ramos|11/1/2018|Fortaleza|3400|NaN|13600|
|646|4646|HL7348|SmartWatch|1|Vanessa|Neves|6/5/2018|Fortaleza|1400|NaN|1400|
|647|4647|HL4379|Televisão|3|Raíssa|Oros|4/7/2018|Fortaleza|2500|NaN|7500|
|648|4654|HL2714|Tablet|4|Bárbara|Cavalcante|3/31/2018|Fortaleza|1600|NaN|6400|
|649|4655|HL7348|SmartWatch|2|Victor|Lira|10/16/2018|Fortaleza|1400|NaN|2800|
|650|4673|HL1148|Câmera|3|Luíza|Goulart|6/18/2018|Fortaleza|2100|NaN|6300|
|651|4676|HL1148|Câmera|3|Henrique|Silva|9/1/2018|Fortaleza|2100|NaN|6300|
|652|4679|HL4379|Televisão|5|Silvio|Fahrnholz|11/20/2018|Fortaleza|2500|NaN|12500|
|653|4693|HL9962|Android|2|Diogo|Peixoto|2/15/2018|Fortaleza|3400|NaN|6800|
|654|4715|HL4379|Televisão|1|Larissa|Florim|7/26/2018|Fortaleza|2500|NaN|2500|
|655|4719|HL2714|Tablet|3|Julia|Penteado|9/13/2018|Fortaleza|1600|NaN|4800|
|656|4720|HL9962|Android|3|Ives|Teixeira|3/19/2018|Fortaleza|3400|NaN|10200|
|657|4725|HL1918|iPhone|5|Juliana|Correa|1/30/2018|Fortaleza|5300|NaN|26500|
|658|4727|HL8851|Notebook|1|João|Peçanha|9/22/2018|Fortaleza|3500|NaN|3500|
|659|4739|HL8851|Notebook|4|Arthur|Fernandes|6/19/2018|Fortaleza|3500|NaN|14000|
|660|4740|HL1918|iPhone|1|Guilherme|Monteiro|8/3/2018|Fortaleza|5300|NaN|5300|
|661|4741|HL1918|iPhone|2|Pedro|Santana|9/16/2018|Fortaleza|5300|NaN|10600|
|662|4744|HL1918|iPhone|3|Gabrielle|Viríssimo|6/11/2018|Fortaleza|5300|NaN|15900|
|663|4745|HL4379|Televisão|2|Matheus|Silva|3/15/2018|Fortaleza|2500|NaN|5000|
|664|4749|HL4379|Televisão|5|Carolina|Figueiredo|11/26/2018|Fortaleza|2500|NaN|12500|
|665|4757|HL8851|Notebook|2|Bruno|Temporal|8/15/2018|Fortaleza|3500|NaN|7000|
|666|4758|HL9962|Android|1|João|Costa|9/3/2018|Fortaleza|3400|NaN|3400|
|667|4760|HL2714|Tablet|3|Eduardo|Ferreira|6/11/2018|Fortaleza|1600|NaN|4800|
|668|4764|HL4379|Televisão|5|Eduardo|Soares|11/1/2018|Fortaleza|2500|NaN|12500|
|669|4774|HL1918|iPhone|3|Paula|Cavalcanti|7/29/2018|Fortaleza|5300|NaN|15900|
|670|4779|HL1918|iPhone|1|Juliana|Mesquita|11/4/2018|Fortaleza|5300|NaN|5300|
|671|4791|HL1918|iPhone|3|Maria|Junior|10/3/2018|Fortaleza|5300|NaN|15900|
|672|4793|HL9962|Android|3|Rilson|Guedes|3/4/2018|Fortaleza|3400|NaN|10200|
|673|4799|HL8851|Notebook|2|Thiago|Veiga|6/29/2018|Fortaleza|3500|NaN|7000|
|674|4801|HL4379|Televisão|4|Hanna|Fonseca|8/5/2018|Fortaleza|2500|NaN|10000|
|675|4804|HL9962|Android|2|Bruna|Londero|3/7/2018|Fortaleza|3400|NaN|6800|
|676|4805|HL4379|Televisão|5|Luiza|Farias|7/25/2018|Fortaleza|2500|NaN|12500|
|677|4817|HL1918|iPhone|4|Caio|Silva|11/22/2018|Fortaleza|5300|NaN|21200|
|678|4818|HL7348|SmartWatch|1|Dandara|Reis|10/25/2018|Fortaleza|1400|NaN|1400|
|679|4831|HL1148|Câmera|5|Pedro|Bitencourt|9/30/2018|Fortaleza|2100|NaN|10500|
|680|4832|HL1918|iPhone|2|Jéssica|Netto|9/15/2018|Fortaleza|5300|NaN|10600|
|681|4833|HL4379|Televisão|3|Ana|Gonzaga|3/7/2018|Fortaleza|2500|NaN|7500|
|682|4841|HL4379|Televisão|5|Diogo|Ressurreição|3/26/2018|Fortaleza|2500|NaN|12500|
|683|4843|HL7348|SmartWatch|4|Pedro|Xavier|5/3/2018|Fortaleza|1400|NaN|5600|
|684|4845|HL4379|Televisão|3|Rogério|Gentile|9/12/2018|Fortaleza|2500|NaN|7500|
|685|4852|HL1918|iPhone|4|Raíza|Lopes|6/5/2018|Fortaleza|5300|NaN|21200|
|686|4856|HL1148|Câmera|2|Guilherme|Merotto|1/23/2018|Fortaleza|2100|NaN|4200|
|687|4872|HL1918|iPhone|5|Ives|Teixeira|12/16/2018|Fortaleza|5300|NaN|26500|
|688|4884|HL1148|Câmera|1|Leonardo|Ferreira|7/3/2018|Fortaleza|2100|NaN|2100|
|689|4885|HL4379|Televisão|5|Arthur|Portela|10/18/2018|Fortaleza|2500|NaN|12500|
|690|4889|HL4379|Televisão|5|Guilherme|Monteiro|5/25/2018|Fortaleza|2500|NaN|12500|
|691|4896|HL9962|Android|1|Victor|Soares|5/11/2018|Fortaleza|3400|NaN|3400|
|692|4898|HL1148|Câmera|2|Thiago|Veiga|10/3/2018|Fortaleza|2100|NaN|4200|
|693|4907|HL1918|iPhone|3|Pedro|Santos|10/14/2018|Fortaleza|5300|NaN|15900|
|694|4915|HL9962|Android|1|Joana|Calmon|4/29/2018|Fortaleza|3400|NaN|3400|
|695|4939|HL4379|Televisão|4|José|Seixas|6/16/2018|Fortaleza|2500|NaN|10000|
|696|4944|HL2714|Tablet|3|Wilson|Brandão|11/9/2018|Fortaleza|1600|NaN|4800|
|697|4945|HL2714|Tablet|2|Ruan|Lopes|4/15/2018|Fortaleza|1600|NaN|3200|
|698|4949|HL8851|Notebook|5|Thais|Rodrigues|9/3/2018|Fortaleza|3500|NaN|17500|
|699|4950|HL1918|iPhone|1|Carolina|Motta|9/30/2018|Fortaleza|5300|NaN|5300|
|700|4956|HL1918|iPhone|1|Anna|Silva|4/3/2018|Fortaleza|5300|NaN|5300|
|701|4962|HL1918|iPhone|3|Rogério|Pereira|2/11/2018|Fortaleza|5300|NaN|15900|
|702|4977|HL7348|SmartWatch|3|Letícia|Araujo|8/10/2018|Fortaleza|1400|NaN|4200|
|703|4987|HL2714|Tablet|2|Leticia|Mesquita|7/31/2018|Fortaleza|1600|NaN|3200|
|704|4988|HL4379|Televisão|4|Roberto|Tiradentes|12/22/2018|Fortaleza|2500|NaN|10000|
|705|4993|HL4379|Televisão|2|Julia|Aliani|10/10/2018|Fortaleza|2500|NaN|5000|
|706|5010|HL9962|Android|2|Juliana|Souza|8/10/2018|Fortaleza|3400|NaN|6800|
|707|5016|HL4379|Televisão|5|Antônio|Oliveira|1/26/2018|Fortaleza|2500|NaN|12500|
|708|5022|HL1918|iPhone|5|Adriane|Gomes|2/20/2018|Fortaleza|5300|NaN|26500|
|709|5023|HL1918|iPhone|3|Renan|Ventura|11/15/2018|Fortaleza|5300|NaN|15900|
|710|5043|HL1148|Câmera|3|Aline|Andrade|8/18/2018|Fortaleza|2100|NaN|6300|
|711|5051|HL1918|iPhone|4|Adriane|Chagas|2/3/2018|Fortaleza|5300|NaN|21200|
|712|5056|HL7348|SmartWatch|2|Rafael|Rocha|8/6/2018|Fortaleza|1400|NaN|2800|
|713|5060|HL1918|iPhone|4|Gustavo|Junior|4/23/2018|Fortaleza|5300|NaN|21200|
|714|5063|HL2714|Tablet|3|David|Campelo|6/14/2018|Fortaleza|1600|NaN|4800|
|715|5071|HL9962|Android|5|Rebeca|Reis|9/2/2018|Fortaleza|3400|NaN|17000|
|716|5073|HL1918|iPhone|3|Cícero|Ramos|1/7/2018|Fortaleza|5300|NaN|15900|
|717|5077|HL7348|SmartWatch|1|Mariana|Miranda|2/21/2018|Fortaleza|1400|NaN|1400|
|718|5083|HL1918|iPhone|2|Lucas|Chagas|12/13/2018|Fortaleza|5300|NaN|10600|
|719|5094|HL9962|Android|2|Joao|Pereira|4/9/2018|Fortaleza|3400|NaN|6800|
|720|5095|HL1148|Câmera|1|Caio|Moraes|12/24/2018|Fortaleza|2100|NaN|2100|
|721|5103|HL4379|Televisão|2|Carolina|Carneiro|10/1/2018|Fortaleza|2500|NaN|5000|
|722|5105|HL1918|iPhone|4|Isabel|Leite|8/7/2018|Fortaleza|5300|NaN|21200|
|723|5116|HL1918|iPhone|2|Fernanda|Rubim|3/29/2018|Fortaleza|5300|NaN|10600|
|724|5122|HL1918|iPhone|4|Nathan|Morelli|7/13/2018|Fortaleza|5300|NaN|21200|
|725|5130|HL9962|Android|1|Fernanda|Figueiredo|1/24/2018|Fortaleza|3400|NaN|3400|
|726|5138|HL1918|iPhone|3|Pedro|Sena|3/9/2018|Fortaleza|5300|NaN|15900|
|727|5140|HL9962|Android|1|Jeferson|Sone|4/30/2018|Fortaleza|3400|NaN|3400|
|728|5146|HL1918|iPhone|4|Thayna|Martins|4/23/2018|Fortaleza|5300|NaN|21200|
|729|5150|HL4379|Televisão|2|Raphael|Mattos|5/3/2018|Fortaleza|2500|NaN|5000|
|730|5165|HL1918|iPhone|5|Carolina|Vasconcelos|2/21/2018|Fortaleza|5300|NaN|26500|
|731|5169|HL1918|iPhone|5|Anna|Silva|12/30/2018|Fortaleza|5300|NaN|26500|
|732|5174|HL1148|Câmera|3|Lucas|Lima|1/8/2018|Fortaleza|2100|NaN|6300|
|733|5184|HL1918|iPhone|2|Jéssica|Teixeira|12/7/2018|Fortaleza|5300|NaN|10600|
|734|5186|HL9962|Android|2|Dykson|Silva|1/18/2018|Fortaleza|3400|NaN|6800|
|735|5193|HL4379|Televisão|4|Monique|Vasconcelos|3/14/2018|Fortaleza|2500|NaN|10000|
|736|5201|HL2714|Tablet|3|Gabriela|Fernandes|9/3/2018|Fortaleza|1600|NaN|4800|
|737|5210|HL1918|iPhone|5|Hanna|Fonseca|4/14/2018|Fortaleza|5300|NaN|26500|
|738|5222|HL1918|iPhone|2|Ylana|Teraoka|1/22/2018|Fortaleza|5300|NaN|10600|
|739|5223|HL9962|Android|5|Ulisses|Filho|12/24/2018|Fortaleza|3400|NaN|17000|
|740|5230|HL4379|Televisão|1|Lorena|Carvalho|7/10/2018|Fortaleza|2500|NaN|2500|
|741|5231|HL8851|Notebook|5|Michelle|Figueiredo|5/4/2018|Fortaleza|3500|NaN|17500|
|742|5241|HL9962|Android|1|Lucas|Baptista|8/27/2018|Fortaleza|3400|NaN|3400|
|743|5249|HL2714|Tablet|5|Guilherme|Lima|7/2/2018|Fortaleza|1600|NaN|8000|
|744|5251|HL9962|Android|5|Luiza|Cabral|1/30/2018|Fortaleza|3400|NaN|17000|
|745|5256|HL4379|Televisão|3|Eduardo|Ferreira|9/11/2018|Fortaleza|2500|NaN|7500|
|746|5264|HL1918|iPhone|5|Pedro|Rodrigues|2/11/2018|Fortaleza|5300|NaN|26500|
|747|5271|HL1918|iPhone|5|Rodrigo|Souza|10/1/2018|Fortaleza|5300|NaN|26500|
|748|5281|HL1918|iPhone|1|Karina|Camara|11/28/2018|Fortaleza|5300|NaN|5300|
|749|5297|HL1918|iPhone|5|Caio|Cardoso|1/18/2018|Fortaleza|5300|NaN|26500|
|750|5300|HL4379|Televisão|3|Igor|Lima|1/11/2018|Fortaleza|2500|NaN|7500|
|751|5312|HL8851|Notebook|1|Brenno|Santos|12/28/2018|Fortaleza|3500|NaN|3500|
|752|5313|HL7348|SmartWatch|4|Paola|Abreu|4/14/2018|Fortaleza|1400|NaN|5600|
|753|5332|HL4379|Televisão|3|Allan|Guedes|11/2/2018|Fortaleza|2500|NaN|7500|
|754|5336|HL1148|Câmera|1|João|Castilho|7/23/2018|Fortaleza|2100|NaN|2100|
|755|5342|HL2714|Tablet|1|João|Abraçado|4/20/2018|Fortaleza|1600|NaN|1600|
|756|5348|HL7348|SmartWatch|4|Joao|Pereira|8/2/2018|Fortaleza|1400|NaN|5600|
|757|5349|HL1918|iPhone|2|Adriane|Chagas|11/27/2018|Fortaleza|5300|NaN|10600|
|758|5350|HL1918|iPhone|3|Eduardo|Ferreira|10/15/2018|Fortaleza|5300|NaN|15900|
|759|5362|HL1918|iPhone|3|José|Jesus|8/6/2018|Fortaleza|5300|NaN|15900|
|760|5364|HL2714|Tablet|4|Lucas|Baptista|7/4/2018|Fortaleza|1600|NaN|6400|
|761|5367|HL8851|Notebook|2|Thomáz|Bôas|9/29/2018|Fortaleza|3500|NaN|7000|
|762|5387|HL4379|Televisão|3|Luiz|Almeida|6/17/2018|Fortaleza|2500|NaN|7500|
|763|5391|HL2714|Tablet|1|Priscila|Vogel|8/12/2018|Fortaleza|1600|NaN|1600|
|764|5400|HL7348|SmartWatch|1|Alvaro|Kranz|11/30/2018|Fortaleza|1400|NaN|1400|
|765|5401|HL4379|Televisão|4|Beatriz|Silva|8/15/2018|Fortaleza|2500|NaN|10000|
|766|5408|HL1918|iPhone|5|Lucas|Machado|11/19/2018|Fortaleza|5300|NaN|26500|
|767|5418|HL1918|iPhone|5|Eduardo|Vargas|4/25/2018|Fortaleza|5300|NaN|26500|
|768|5421|HL2714|Tablet|5|Igor|Lima|1/29/2018|Fortaleza|1600|NaN|8000|
|769|5433|HL4379|Televisão|5|Bruna|Gomes|7/11/2018|Fortaleza|2500|NaN|12500|
|770|5438|HL1918|iPhone|4|Rogério|Pereira|10/21/2018|Fortaleza|5300|NaN|21200|
|771|5440|HL4379|Televisão|1|Gabrielle|Porto|12/12/2018|Fortaleza|2500|NaN|2500|
|772|5450|HL1918|iPhone|5|Morgana|Correa|4/23/2018|Fortaleza|5300|NaN|26500|
|773|5462|HL1918|iPhone|3|Manuela|Merege|7/29/2018|Fortaleza|5300|NaN|15900|
|774|5466|HL4379|Televisão|2|Raissa|Pinheiro|11/19/2018|Fortaleza|2500|NaN|5000|
|775|5471|HL1148|Câmera|3|Rafael|Guimarães|1/22/2018|Fortaleza|2100|NaN|6300|
|776|5473|HL7348|SmartWatch|4|Lucas|Freire|9/29/2018|Fortaleza|1400|NaN|5600|
|777|5475|HL7348|SmartWatch|2|Matheus|Gomes|12/20/2018|Fortaleza|1400|NaN|2800|
|778|5481|HL8851|Notebook|5|Lucas|Freire|11/16/2018|Fortaleza|3500|NaN|17500|
|779|5482|HL4379|Televisão|4|Yasmim|Bittencourt|11/11/2018|Fortaleza|2500|NaN|10000|
|780|5498|HL4379|Televisão|3|João|Araujo|9/20/2018|Fortaleza|2500|NaN|7500|
|781|5501|HL1918|iPhone|3|Michelle|Figueiredo|12/27/2018|Fortaleza|5300|NaN|15900|
|782|5520|HL4379|Televisão|2|Tadeu|Sousa|8/19/2018|Fortaleza|2500|NaN|5000|
|783|5522|HL1918|iPhone|5|Lívia|Marques|12/27/2018|Fortaleza|5300|NaN|26500|
|784|5523|HL1918|iPhone|4|Andre|Sampaio|4/11/2018|Fortaleza|5300|NaN|21200|
|785|5534|HL4379|Televisão|3|Izabel|Miura|10/31/2018|Fortaleza|2500|NaN|7500|
|786|5547|HL8851|Notebook|5|Bianca|Piero|3/13/2018|Fortaleza|3500|NaN|17500|
|787|5549|HL1148|Câmera|1|Morgana|Correa|8/25/2018|Fortaleza|2100|NaN|2100|
|788|5561|HL8851|Notebook|4|Bianca|Piero|1/28/2018|Fortaleza|3500|NaN|14000|
|789|5572|HL8851|Notebook|1|Caio|Moraes|6/20/2018|Fortaleza|3500|NaN|3500|
|790|5591|HL2714|Tablet|2|Yasser|Calbucci|11/11/2018|Fortaleza|1600|NaN|3200|
|791|5607|HL1918|iPhone|1|Luis|Villanova|2/10/2018|Fortaleza|5300|NaN|5300|
|792|5617|HL1148|Câmera|2|Thales|Andrade|10/20/2018|Fortaleza|2100|NaN|4200|
|793|5625|HL1918|iPhone|3|Juliana|Barreira|5/4/2018|Fortaleza|5300|NaN|15900|
|794|5628|HL8851|Notebook|3|Jorge|Fonseca|7/5/2018|Fortaleza|3500|NaN|10500|
|795|5631|HL9962|Android|3|Daniel|Felippe|8/19/2018|Fortaleza|3400|NaN|10200|
|796|5637|HL1918|iPhone|4|Andre|Nóbrega|11/23/2018|Fortaleza|5300|NaN|21200|
|797|5639|HL1148|Câmera|2|Bernardo|Soares|8/17/2018|Fortaleza|2100|NaN|4200|
|798|5642|HL4379|Televisão|3|Paola|Abreu|3/11/2018|Fortaleza|2500|NaN|7500|
|799|5652|HL8851|Notebook|2|Rachel|Silva|12/13/2018|Fortaleza|3500|NaN|7000|
|800|5659|HL8851|Notebook|2|Luíza|Garcia|4/27/2018|Fortaleza|3500|NaN|7000|
|801|5671|HL1918|iPhone|1|Ana|Gomes|2/8/2018|Fortaleza|5300|NaN|5300|
|802|5674|HL9962|Android|3|Igor|Lima|9/14/2018|Fortaleza|3400|NaN|10200|
|803|5675|HL8851|Notebook|5|Bruno|Temporal|1/3/2018|Fortaleza|3500|NaN|17500|
|804|5683|HL1918|iPhone|5|Myllena|Corrêa|9/8/2018|Fortaleza|5300|NaN|26500|
|805|5684|HL2714|Tablet|1|Sandy|Figueiredo|6/19/2018|Fortaleza|1600|NaN|1600|
|806|5698|HL9962|Android|1|Raísa|Rodrigues|8/30/2018|Fortaleza|3400|NaN|3400|
|807|5706|HL4379|Televisão|1|Jéssica|Stefanelli|2/14/2018|Fortaleza|2500|NaN|2500|
|808|5715|HL8851|Notebook|3|Ana|Silva|11/7/2018|Fortaleza|3500|NaN|10500|
|809|5716|HL1918|iPhone|3|Amanda|Roberto|7/16/2018|Fortaleza|5300|NaN|15900|
|810|5738|HL9962|Android|4|Hiaiune|Valim|10/3/2018|Fortaleza|3400|NaN|13600|
|811|5739|HL1918|iPhone|5|Luísa|Fonseca|6/3/2018|Fortaleza|5300|NaN|26500|
|812|5746|HL4379|Televisão|3|Danilo|Alves|7/30/2018|Fortaleza|2500|NaN|7500|
|813|5748|HL4379|Televisão|3|Mariane|Ferreira|6/4/2018|Fortaleza|2500|NaN|7500|
|814|5749|HL1918|iPhone|1|Eric|Júnior|2/23/2018|Fortaleza|5300|NaN|5300|
|815|5754|HL4379|Televisão|5|Raphael|Filho|3/11/2018|Fortaleza|2500|NaN|12500|
|816|5760|HL2714|Tablet|3|Gustavo|Azevedo|1/17/2018|Fortaleza|1600|NaN|4800|
|817|5761|HL4379|Televisão|2|Thomáz|Bôas|7/4/2018|Fortaleza|2500|NaN|5000|
|818|5769|HL1918|iPhone|3|Victor|Lira|1/22/2018|Fortaleza|5300|NaN|15900|
|819|5781|HL8851|Notebook|1|Raíza|Lopes|11/30/2018|Fortaleza|3500|NaN|3500|
|820|5794|HL1148|Câmera|4|Marcelo|Pereira|4/25/2018|Fortaleza|2100|NaN|8400|
|821|5796|HL9962|Android|4|Giovana|Vilela|5/10/2018|Fortaleza|3400|NaN|13600|
|822|5802|HL9962|Android|1|Lucas|Rocha|4/6/2018|Fortaleza|3400|NaN|3400|
|823|5808|HL1918|iPhone|2|Luiz|Almeida|1/1/2018|Fortaleza|5300|NaN|10600|
|824|5834|HL2714|Tablet|1|Cláudio|Aragão|10/15/2018|Fortaleza|1600|NaN|1600|
|825|5836|HL1918|iPhone|2|Carlos|Mesquita|7/15/2018|Fortaleza|5300|NaN|10600|
|826|5837|HL2714|Tablet|4|Amanda|Delgado|12/18/2018|Fortaleza|1600|NaN|6400|
|827|5842|HL1918|iPhone|2|Victor|Lira|6/29/2018|Fortaleza|5300|NaN|10600|
|828|5844|HL7348|SmartWatch|5|Marina|Gama|3/12/2018|Fortaleza|1400|NaN|7000|
|829|5846|HL4379|Televisão|2|Raissa|Maia|6/13/2018|Fortaleza|2500|NaN|5000|
|830|5847|HL9962|Android|5|Deysiane|Medronho|1/30/2018|Fortaleza|3400|NaN|17000|
|831|5852|HL1918|iPhone|1|Daniel|Felippe|6/19/2018|Fortaleza|5300|NaN|5300|
|832|5868|HL9962|Android|5|Ana|Michetti|12/1/2018|Fortaleza|3400|NaN|17000|
|833|5874|HL4379|Televisão|2|Beatriz|Almeida|3/3/2018|Fortaleza|2500|NaN|5000|
|834|5878|HL1918|iPhone|1|Victor|Gomes|11/4/2018|Fortaleza|5300|NaN|5300|
|835|5887|HL7348|SmartWatch|1|Ruan|Gonçalves|12/21/2018|Fortaleza|1400|NaN|1400|
|836|5888|HL7348|SmartWatch|1|Igor|Lima|8/22/2018|Fortaleza|1400|NaN|1400|
|837|5893|HL8851|Notebook|2|Thales|Santos|8/2/2018|Fortaleza|3500|NaN|7000|
|838|5906|HL7348|SmartWatch|5|Douglas|Rodrigues|12/4/2018|Fortaleza|1400|NaN|7000|
|839|5909|HL4379|Televisão|3|Beatriz|Silva|8/4/2018|Fortaleza|2500|NaN|7500|
|840|5913|HL1918|iPhone|3|Mariane|Ferreira|12/1/2018|Fortaleza|5300|NaN|15900|
|841|5920|HL8851|Notebook|2|Giulia|Pessanha|5/24/2018|Fortaleza|3500|NaN|7000|
|842|5922|HL8851|Notebook|4|Henrique|Villanova|7/15/2018|Fortaleza|3500|NaN|14000|
|843|5932|HL7348|SmartWatch|3|Luiz|Limp|10/13/2018|Fortaleza|1400|NaN|4200|
|844|5935|HL1148|Câmera|1|Kim|Ferreira|7/23/2018|Fortaleza|2100|NaN|2100|
|845|5952|HL4379|Televisão|3|Gabriel|Rubim|10/8/2018|Fortaleza|2500|NaN|7500|
|846|5963|HL8851|Notebook|5|Thomáz|Rodriguez|7/15/2018|Fortaleza|3500|NaN|17500|
|847|5970|HL9962|Android|2|Rafaela|Feio|8/3/2018|Fortaleza|3400|NaN|6800|
|848|5985|HL1918|iPhone|4|Philipe|Morete|12/26/2018|Fortaleza|5300|NaN|21200|
|849|5987|HL9962|Android|2|Thomáz|Bôas|5/18/2018|Fortaleza|3400|NaN|6800|
|850|5995|HL7348|SmartWatch|1|Joao|Silva|11/19/2018|Fortaleza|1400|NaN|1400|
|851|6006|HL1918|iPhone|5|Pedro|Macckione|12/23/2018|Fortaleza|5300|NaN|26500|
|852|6014|HL1918|iPhone|3|Andre|Nóbrega|5/18/2018|Fortaleza|5300|NaN|15900|
|853|6020|HL9962|Android|4|Elaine|Santos|11/21/2018|Fortaleza|3400|NaN|13600|
|854|6041|HL7348|SmartWatch|4|Samara|Pinto|11/17/2018|Fortaleza|1400|NaN|5600|
|855|6049|HL1918|iPhone|4|Carlos|Mesquita|10/21/2018|Fortaleza|5300|NaN|21200|
|856|6066|HL1918|iPhone|2|Felipe|Mendonça|1/18/2018|Fortaleza|5300|NaN|10600|
|857|6095|HL2714|Tablet|1|Lívia|Tanaka|9/27/2018|Fortaleza|1600|NaN|1600|
|858|6096|HL7348|SmartWatch|2|Jonatas|Essaber|3/1/2018|Fortaleza|1400|NaN|2800|
|859|6104|HL9962|Android|2|Isabela|Chagas|7/27/2018|Fortaleza|3400|NaN|6800|
|860|6111|HL4379|Televisão|1|Jessica|Ferreira|9/8/2018|Fortaleza|2500|NaN|2500|
|861|6114|HL1148|Câmera|5|Sylvio|Bernhardt|2/22/2018|Fortaleza|2100|NaN|10500|
|862|6129|HL2714|Tablet|1|Carolina|Vasconcelos|11/10/2018|Fortaleza|1600|NaN|1600|
|863|6130|HL9962|Android|3|Ana|Miura|6/1/2018|Fortaleza|3400|NaN|10200|
|864|6134|HL1918|iPhone|2|Bruna|Gomes|9/27/2018|Fortaleza|5300|NaN|10600|
|865|6137|HL9962|Android|3|Beatriz|Rocha|12/18/2018|Fortaleza|3400|NaN|10200|
|866|6141|HL1148|Câmera|2|Luiza|Cabral|6/9/2018|Fortaleza|2100|NaN|4200|
|867|6181|HL9962|Android|3|Priscila|Garcia|6/12/2018|Fortaleza|3400|NaN|10200|
|868|6189|HL9962|Android|1|Thales|Fanara|8/24/2018|Fortaleza|3400|NaN|3400|
|869|6192|HL4379|Televisão|3|Camilla|Guimarães|3/4/2018|Fortaleza|2500|NaN|7500|
|870|6194|HL1148|Câmera|5|Pedro|Oliveira|7/6/2018|Fortaleza|2100|NaN|10500|
|871|6200|HL4379|Televisão|1|João|Júnior|9/18/2018|Fortaleza|2500|NaN|2500|
|872|6205|HL1918|iPhone|3|Vitor|Arruda|7/20/2018|Fortaleza|5300|NaN|15900|
|873|6215|HL9962|Android|1|Jonatas|Essaber|6/5/2018|Fortaleza|3400|NaN|3400|
|874|6220|HL4379|Televisão|5|Isabela|Rodrigues|3/27/2018|Fortaleza|2500|NaN|12500|
|875|6221|HL7348|SmartWatch|2|João|Ribeiro|4/13/2018|Fortaleza|1400|NaN|2800|
|876|6243|HL4379|Televisão|2|Ana|Monte|3/18/2018|Fortaleza|2500|NaN|5000|
|877|6251|HL1918|iPhone|5|Pedro|Ferrari|6/23/2018|Fortaleza|5300|NaN|26500|
|878|6254|HL4379|Televisão|3|Antonio|Manhães|2/23/2018|Fortaleza|2500|NaN|7500|
|879|6260|HL8851|Notebook|5|Yasmim|Bittencourt|10/7/2018|Fortaleza|3500|NaN|17500|
|880|6289|HL8851|Notebook|5|Rilson|Guedes|4/2/2018|Fortaleza|3500|NaN|17500|
|881|6291|HL4379|Televisão|5|Rafael|Wajnsztok|4/9/2018|Fortaleza|2500|NaN|12500|
|882|6315|HL1918|iPhone|5|Thayna|Martins|7/28/2018|Fortaleza|5300|NaN|26500|
|883|6352|HL2714|Tablet|3|Carla|Zakhm|4/26/2018|Fortaleza|1600|NaN|4800|
|884|6353|HL1148|Câmera|5|Mateus|Maia|1/17/2018|Fortaleza|2100|NaN|10500|
|885|6355|HL4379|Televisão|1|Giulia|Pessanha|6/8/2018|Fortaleza|2500|NaN|2500|
|886|6356|HL1918|iPhone|5|David|Assumpção|10/5/2018|Fortaleza|5300|NaN|26500|
|887|6365|HL4379|Televisão|1|Mariana|Miranda|8/13/2018|Fortaleza|2500|NaN|2500|
|888|6381|HL7348|SmartWatch|4|Isabella|Rodrigues|10/18/2018|Fortaleza|1400|NaN|5600|
|889|6385|HL8851|Notebook|4|Lucas|Freitas|10/21/2018|Fortaleza|3500|NaN|14000|
|890|6396|HL4379|Televisão|4|Bernardo|Botelho|12/5/2018|Fortaleza|2500|NaN|10000|
|891|6417|HL1918|iPhone|5|Gabriel|Thoni|12/25/2018|Fortaleza|5300|NaN|26500|
|892|6420|HL1918|iPhone|4|Rafaela|Feio|11/23/2018|Fortaleza|5300|NaN|21200|
|893|6425|HL1918|iPhone|3|Pedro|Pereira|4/9/2018|Fortaleza|5300|NaN|15900|
|894|6434|HL1918|iPhone|4|Lucas|Valim|9/4/2018|Fortaleza|5300|NaN|21200|
|895|6438|HL4379|Televisão|4|Sandy|Figueiredo|4/7/2018|Fortaleza|2500|NaN|10000|
|896|6447|HL8851|Notebook|4|Felipe|Paulo|8/3/2018|Fortaleza|3500|NaN|14000|
|897|6455|HL2714|Tablet|3|Sandy|Figueiredo|4/13/2018|Fortaleza|1600|NaN|4800|
|898|6460|HL7348|SmartWatch|4|Mayara|Soares|12/4/2018|Fortaleza|1400|NaN|5600|
|899|6464|HL7348|SmartWatch|1|Arthur|Fernandes|6/9/2018|Fortaleza|1400|NaN|1400|
|900|6470|HL1918|iPhone|1|Daniel|Sousa|11/4/2018|Fortaleza|5300|NaN|5300|
|901|6472|HL8851|Notebook|2|Livia|Codeceira|6/16/2018|Fortaleza|3500|NaN|7000|
|902|6475|HL2714|Tablet|1|Antônio|Oliveira|12/3/2018|Fortaleza|1600|NaN|1600|
|903|6476|HL1918|iPhone|5|Marcos|Nucci|10/10/2018|Fortaleza|5300|NaN|26500|
|904|6482|HL4379|Televisão|4|Luiza|Procaci|12/23/2018|Fortaleza|2500|NaN|10000|
|905|6494|HL4379|Televisão|1|Bruna|Londero|7/12/2018|Fortaleza|2500|NaN|2500|
|906|6495|HL1918|iPhone|3|Maria|Gasperi|8/15/2018|Fortaleza|5300|NaN|15900|
|907|6498|HL4379|Televisão|4|Ives|Pinheiro|6/28/2018|Fortaleza|2500|NaN|10000|
|908|6516|HL9962|Android|3|Thayna|Martins|11/23/2018|Fortaleza|3400|NaN|10200|
|909|6517|HL1918|iPhone|4|Victor|Franco|3/10/2018|Fortaleza|5300|NaN|21200|
|910|6518|HL2714|Tablet|1|Stephanie|Oliveira|11/18/2018|Fortaleza|1600|NaN|1600|
|911|6524|HL7348|SmartWatch|5|Gabriel|Almeida|3/28/2018|Fortaleza|1400|NaN|7000|
|912|6525|HL8851|Notebook|5|Luiza|Cabral|6/1/2018|Fortaleza|3500|NaN|17500|
|913|6532|HL1918|iPhone|3|Lucas|Wanderley|2/16/2018|Fortaleza|5300|NaN|15900|
|914|6534|HL7348|SmartWatch|1|Lucas|Fontoura|5/23/2018|Fortaleza|1400|NaN|1400|
|915|6536|HL8851|Notebook|2|Luíza|Melo|4/19/2018|Fortaleza|3500|NaN|7000|
|916|6546|HL7348|SmartWatch|1|Amanda|Roberto|10/17/2018|Fortaleza|1400|NaN|1400|
|917|6548|HL9962|Android|4|Wen|Santos|2/28/2018|Fortaleza|3400|NaN|13600|
|918|6550|HL8851|Notebook|4|Beatriz|Santos|11/2/2018|Fortaleza|3500|NaN|14000|
|919|6552|HL7348|SmartWatch|4|Guilherme|Castilho|6/8/2018|Fortaleza|1400|NaN|5600|
|920|6553|HL1918|iPhone|3|Tiago|Pereira|7/26/2018|Fortaleza|5300|NaN|15900|
|921|6556|HL1918|iPhone|5|Isabela|Teixeira|12/20/2018|Fortaleza|5300|NaN|26500|
|922|6557|HL4379|Televisão|3|Allan|Candido|5/15/2018|Fortaleza|2500|NaN|7500|
|923|6565|HL4379|Televisão|5|Adriana|Carneiro|5/24/2018|Fortaleza|2500|NaN|12500|
|924|6568|HL1148|Câmera|3|Breno|Costa|5/8/2018|Fortaleza|2100|NaN|6300|
|925|6588|HL9962|Android|5|Adriana|Passos|11/10/2018|Fortaleza|3400|NaN|17000|
|926|6591|HL4379|Televisão|5|Beatriz|Rocha|9/24/2018|Fortaleza|2500|NaN|12500|
|927|6592|HL1918|iPhone|5|Alon|Pestana|11/16/2018|Fortaleza|5300|NaN|26500|
|928|6597|HL8851|Notebook|2|Bruna|Ramos|7/11/2018|Fortaleza|3500|NaN|7000|
|929|6599|HL1918|iPhone|2|Mateus|Maia|10/30/2018|Fortaleza|5300|NaN|10600|
|930|6615|HL4379|Televisão|1|Marianna|Pestana|11/21/2018|Fortaleza|2500|NaN|2500|
|931|6622|HL9962|Android|4|Jessica|Ferreira|2/23/2018|Fortaleza|3400|NaN|13600|
|932|6630|HL1918|iPhone|3|Gabriela|Fernandes|1/22/2018|Fortaleza|5300|NaN|15900|
|933|6633|HL4379|Televisão|1|Luiza|Procaci|9/8/2018|Fortaleza|2500|NaN|2500|
|934|6636|HL9962|Android|3|Anderson|Martins|10/24/2018|Fortaleza|3400|NaN|10200|
|935|6638|HL4379|Televisão|5|Luiz|Conceição|5/22/2018|Fortaleza|2500|NaN|12500|
|936|6649|HL7348|SmartWatch|3|Henrique|Oliveira|3/29/2018|Fortaleza|1400|NaN|4200|
|937|6651|HL1918|iPhone|5|Sandy|Moreira|3/17/2018|Fortaleza|5300|NaN|26500|
|938|6653|HL8851|Notebook|1|Eduardo|Veiga|5/22/2018|Fortaleza|3500|NaN|3500|
|939|6654|HL4379|Televisão|2|Felipe|Mello|5/5/2018|Fortaleza|2500|NaN|5000|
|940|6658|HL9962|Android|5|Aline|Andrade|3/8/2018|Fortaleza|3400|NaN|17000|
|941|6659|HL7348|SmartWatch|3|Isabela|Teixeira|8/10/2018|Fortaleza|1400|NaN|4200|
|942|6660|HL2714|Tablet|5|Guilherme|Merotto|10/16/2018|Fortaleza|1600|NaN|8000|
|943|6672|HL9962|Android|3|Yasmim|Verly|3/30/2018|Fortaleza|3400|NaN|10200|
|944|6677|HL4379|Televisão|2|Caroline|Aquino|11/10/2018|Fortaleza|2500|NaN|5000|
|945|6689|HL1918|iPhone|2|José|Vieira|11/13/2018|Fortaleza|5300|NaN|10600|
|946|6690|HL9962|Android|1|Jéssica|Stefanelli|9/20/2018|Fortaleza|3400|NaN|3400|
|947|6691|HL8851|Notebook|5|Diego|Mello|11/7/2018|Fortaleza|3500|NaN|17500|
|948|6699|HL4379|Televisão|5|Catarina|Teixeira|8/22/2018|Fortaleza|2500|NaN|12500|
|949|6727|HL2714|Tablet|4|Bianca|Piero|3/7/2018|Fortaleza|1600|NaN|6400|
|950|6729|HL4379|Televisão|1|Danilo|Rubim|8/25/2018|Fortaleza|2500|NaN|2500|
|951|6730|HL1918|iPhone|4|Bianca|Paz|3/4/2018|Fortaleza|5300|NaN|21200|
|952|6732|HL1918|iPhone|3|Gabrielle|Silva|12/10/2018|Fortaleza|5300|NaN|15900|
|953|6740|HL1148|Câmera|3|Fernanda|Silva|4/28/2018|Fortaleza|2100|NaN|6300|
|954|6742|HL9962|Android|2|Guilherme|Castilho|10/14/2018|Fortaleza|3400|NaN|6800|
|955|6759|HL7348|SmartWatch|2|Deysiane|Medronho|2/2/2018|Fortaleza|1400|NaN|2800|
|956|6772|HL8851|Notebook|5|Debora|Silva|12/10/2018|Fortaleza|3500|NaN|17500|
|957|6775|HL4379|Televisão|1|Lucas|Costa|5/28/2018|Fortaleza|2500|NaN|2500|
|958|6776|HL4379|Televisão|1|Roberto|Tiradentes|1/7/2018|Fortaleza|2500|NaN|2500|
|959|6778|HL7348|SmartWatch|4|Isabelle|Gonçalves|2/8/2018|Fortaleza|1400|NaN|5600|
|960|6790|HL8851|Notebook|5|Thomáz|Vannier|4/3/2018|Fortaleza|3500|NaN|17500|
|961|6792|HL8851|Notebook|3|Joao|Pereira|11/19/2018|Fortaleza|3500|NaN|10500|
|962|6793|HL1918|iPhone|2|Michelle|Miura|5/22/2018|Fortaleza|5300|NaN|10600|
|963|6799|HL4379|Televisão|2|Luana|Santos|6/9/2018|Fortaleza|2500|NaN|5000|
|964|6801|HL2714|Tablet|4|Livia|Codeceira|11/29/2018|Fortaleza|1600|NaN|6400|
|965|6809|HL4379|Televisão|2|Vanessa|Rodrigues|4/6/2018|Fortaleza|2500|NaN|5000|
|966|6813|HL2714|Tablet|3|Iuri|Barbosa|10/2/2018|Fortaleza|1600|NaN|4800|
|967|6837|HL2714|Tablet|3|Eduardo|Veiga|9/29/2018|Fortaleza|1600|NaN|4800|
|968|6839|HL1148|Câmera|3|Mariana|Rotava|1/27/2018|Fortaleza|2100|NaN|6300|
|969|6850|HL7348|SmartWatch|3|Gabriel|Thome|6/18/2018|Fortaleza|1400|NaN|4200|
|970|6854|HL1918|iPhone|4|Mateus|Duque|1/19/2018|Fortaleza|5300|NaN|21200|
|971|6857|HL4379|Televisão|2|Raphael|Ferman|6/29/2018|Fortaleza|2500|NaN|5000|
|972|6868|HL2714|Tablet|3|Eduardo|Pacheco|9/25/2018|Fortaleza|1600|NaN|4800|
|973|6876|HL4379|Televisão|5|Ruan|Gonçalves|12/18/2018|Fortaleza|2500|NaN|12500|
|974|6879|HL1148|Câmera|5|Larissa|Jesus|12/20/2018|Fortaleza|2100|NaN|10500|
|975|6889|HL7348|SmartWatch|3|Marina|Correa|5/19/2018|Fortaleza|1400|NaN|4200|
|976|6891|HL1918|iPhone|1|Carolina|Bernardes|2/11/2018|Fortaleza|5300|NaN|5300|
|977|6894|HL8851|Notebook|4|Amanda|Delgado|7/19/2018|Fortaleza|3500|NaN|14000|
|978|6899|HL1148|Câmera|2|David|Vasconcelos|8/25/2018|Fortaleza|2100|NaN|4200|
|979|6901|HL8851|Notebook|4|Rojane|Lima|4/22/2018|Fortaleza|3500|NaN|14000|
|980|6911|HL1918|iPhone|3|Victor|Zakhm|2/23/2018|Fortaleza|5300|NaN|15900|
|981|6921|HL7348|SmartWatch|3|Fernanda|Junior|7/19/2018|Fortaleza|1400|NaN|4200|
|982|6926|HL1918|iPhone|2|Ives|Teixeira|6/13/2018|Fortaleza|5300|NaN|10600|
|983|6927|HL8851|Notebook|5|Beatriz|Rocha|11/29/2018|Fortaleza|3500|NaN|17500|
|984|6928|HL4379|Televisão|3|Vivianne|Rodrigues|8/28/2018|Fortaleza|2500|NaN|7500|
|985|6934|HL2714|Tablet|5|Carlos|Galvão|9/22/2018|Fortaleza|1600|NaN|8000|
|986|6935|HL8851|Notebook|3|Giovana|Vilela|4/28/2018|Fortaleza|3500|NaN|10500|
|987|6938|HL4379|Televisão|3|Adrielle|Gabriel|8/7/2018|Fortaleza|2500|NaN|7500|
|988|6940|HL1918|iPhone|4|Michelle|Miura|8/21/2018|Fortaleza|5300|NaN|21200|
|989|6945|HL4379|Televisão|2|Alessandra|Martins|7/10/2018|Fortaleza|2500|NaN|5000|
|990|6952|HL2714|Tablet|3|Nina|Magalhães|2/26/2018|Fortaleza|1600|NaN|4800|
|991|6974|HL2714|Tablet|5|Sthefeson|Pereira|4/14/2018|Fortaleza|1600|NaN|8000|
|992|6989|HL4379|Televisão|3|Anderson|Barreto|5/25/2018|Fortaleza|2500|NaN|7500|
|993|6995|HL1918|iPhone|4|Beatriz|Biase|5/7/2018|Fortaleza|5300|NaN|21200|
|994|6996|HL2714|Tablet|2|Lucas|Machado|8/4/2018|Fortaleza|1600|NaN|3200|
|995|7002|HL4379|Televisão|5|Breno|Caputo|12/10/2018|Fortaleza|2500|NaN|12500|
|996|7008|HL7348|SmartWatch|4|Eric|Júnior|12/26/2018|Fortaleza|1400|NaN|5600|
|997|7023|HL2714|Tablet|4|David|Assumpção|1/16/2018|Fortaleza|1600|NaN|6400|
|998|7033|HL4379|Televisão|1|Rodrigo|Silva|8/26/2018|Fortaleza|2500|NaN|2500|
|999|7048|HL4379|Televisão|1|Pedro|Jorge|11/3/2018|Fortaleza|2500|NaN|2500|
|1000|7049|HL2714|Tablet|5|Paola|Abreu|11/20/2018|Fortaleza|1600|NaN|8000|
|1001|7055|HL7348|SmartWatch|4|Rebeca|Reis|12/13/2018|Fortaleza|1400|NaN|5600|
|1002|7065|HL2714|Tablet|3|Alon|Pestana|7/24/2018|Fortaleza|1600|NaN|4800|
|1003|7069|HL1918|iPhone|4|Fabio|Boccaletti|7/19/2018|Fortaleza|5300|NaN|21200|
|1004|7072|HL1148|Câmera|1|Joyce|Medina|7/14/2018|Fortaleza|2100|NaN|2100|
|1005|7083|HL4379|Televisão|1|Priscila|Garcia|12/29/2018|Fortaleza|2500|NaN|2500|
|1006|7088|HL9962|Android|2|Eduardo|Lopes|5/23/2018|Fortaleza|3400|NaN|6800|
|1007|7101|HL8851|Notebook|5|Victor|Firmino|10/28/2018|Fortaleza|3500|NaN|17500|
|1008|7103|HL8851|Notebook|4|Marcelo|Rosa|9/3/2018|Fortaleza|3500|NaN|14000|
|1009|7105|HL4379|Televisão|5|Clarissa|Santos|6/25/2018|Fortaleza|2500|NaN|12500|
|1010|7108|HL1918|iPhone|1|Carlos|Azevedo|11/24/2018|Fortaleza|5300|NaN|5300|
|1011|7111|HL9962|Android|5|Julia|Teixeira|2/5/2018|Fortaleza|3400|NaN|17000|
|1012|7116|HL1918|iPhone|5|Victor|Gomes|2/20/2018|Fortaleza|5300|NaN|26500|
|1013|7131|HL1148|Câmera|3|Luis|Garcia|12/9/2018|Fortaleza|2100|NaN|6300|
|1014|7135|HL7348|SmartWatch|4|Izabel|Lopes|9/28/2018|Fortaleza|1400|NaN|5600|
|1015|7159|HL1918|iPhone|3|Marina|Gama|12/19/2018|Fortaleza|5300|NaN|15900|
|1016|7163|HL2714|Tablet|5|Beatriz|Rodrigues|5/2/2018|Fortaleza|1600|NaN|8000|
|1017|7165|HL4379|Televisão|2|Maurício|Dias|4/23/2018|Fortaleza|2500|NaN|5000|
|1018|7171|HL8851|Notebook|3|Mateus|Polastri|6/10/2018|Fortaleza|3500|NaN|10500|
|1019|7173|HL1918|iPhone|3|Juliana|Goes|5/18/2018|Fortaleza|5300|NaN|15900|
|1020|7180|HL4379|Televisão|1|Pedro|Cardoso|11/24/2018|Fortaleza|2500|NaN|2500|
|1021|7184|HL1918|iPhone|3|Victor|Oliveira|10/14/2018|Fortaleza|5300|NaN|15900|
|1022|7190|HL7348|SmartWatch|5|João|Luz|7/5/2018|Fortaleza|1400|NaN|7000|
|1023|7194|HL1918|iPhone|2|Júlio|Fraga|12/16/2018|Fortaleza|5300|NaN|10600|
|1024|7203|HL8851|Notebook|3|Bruno|Salomão|6/1/2018|Fortaleza|3500|NaN|10500|
|1025|7207|HL1148|Câmera|1|Victor|Corrêa|6/1/2018|Fortaleza|2100|NaN|2100|
|1026|7216|HL4379|Televisão|5|Ravena|Bhering|7/9/2018|Fortaleza|2500|NaN|12500|
|1027|7227|HL7348|SmartWatch|1|Luísa|Fonseca|5/1/2018|Fortaleza|1400|NaN|1400|
|1028|7234|HL1148|Câmera|3|Adriane|Chagas|9/6/2018|Fortaleza|2100|NaN|6300|
|1029|7238|HL1918|iPhone|5|Paula|Cavalcanti|8/10/2018|Fortaleza|5300|NaN|26500|
|1030|7240|HL4379|Televisão|4|Luis|Silva|2/28/2018|Fortaleza|2500|NaN|10000|
|1031|7244|HL1918|iPhone|4|Gabrielle|Viríssimo|2/16/2018|Fortaleza|5300|NaN|21200|
|1032|7246|HL9962|Android|2|Joana|Calmon|2/21/2018|Fortaleza|3400|NaN|6800|
|1033|7247|HL2714|Tablet|3|Izabel|Lopes|6/20/2018|Fortaleza|1600|NaN|4800|
|1034|7251|HL1918|iPhone|1|Gustavo|Erthal|9/12/2018|Fortaleza|5300|NaN|5300|
|1035|7252|HL1918|iPhone|3|Rafaela|Gomes|10/11/2018|Fortaleza|5300|NaN|15900|
|1036|7255|HL1918|iPhone|3|Matheus|Gomes|10/21/2018|Fortaleza|5300|NaN|15900|
|1037|7258|HL7348|SmartWatch|4|Beatriz|Rocha|12/24/2018|Fortaleza|1400|NaN|5600|
|1038|7268|HL1918|iPhone|4|Lais|Candido|6/16/2018|Fortaleza|5300|NaN|21200|
|1039|7276|HL4379|Televisão|4|Wendela|Veloso|5/15/2018|Fortaleza|2500|NaN|10000|
|1040|7278|HL1918|iPhone|4|Rodrigo|Alves|1/15/2018|Fortaleza|5300|NaN|21200|
|1041|7281|HL4379|Televisão|4|João|Peçanha|7/15/2018|Fortaleza|2500|NaN|10000|
|1042|7289|HL1918|iPhone|4|Erick|Soares|4/12/2018|Fortaleza|5300|NaN|21200|
|1043|7307|HL2714|Tablet|1|Jorge|Fonseca|3/4/2018|Fortaleza|1600|NaN|1600|
|1044|7308|HL1918|iPhone|1|Kim|Ferreira|7/12/2018|Fortaleza|5300|NaN|5300|
|1045|7328|HL1918|iPhone|2|Bianca|Procaci|3/3/2018|Fortaleza|5300|NaN|10600|
|1046|7332|HL1148|Câmera|3|Wilson|Brandão|3/4/2018|Fortaleza|2100|NaN|6300|
|1047|7333|HL9962|Android|2|Hygor|Essaber|8/24/2018|Fortaleza|3400|NaN|6800|
|1048|7343|HL1918|iPhone|3|Rilson|Dias|9/15/2018|Fortaleza|5300|NaN|15900|
|1049|7349|HL4379|Televisão|3|José|Fonseca|4/15/2018|Fortaleza|2500|NaN|7500|
|1050|7354|HL8851|Notebook|3|Gabriel|Soares|6/27/2018|Fortaleza|3500|NaN|10500|
|1051|7356|HL4379|Televisão|1|Carolina|Abrahão|3/23/2018|Fortaleza|2500|NaN|2500|
|1052|7357|HL2714|Tablet|4|Carolina|Silva|7/11/2018|Fortaleza|1600|NaN|6400|
|1053|7366|HL9962|Android|5|Clarissa|Santos|7/24/2018|Fortaleza|3400|NaN|17000|
|1054|7367|HL2714|Tablet|2|Eduardo|Ferreira|5/7/2018|Fortaleza|1600|NaN|3200|
|1055|7390|HL8851|Notebook|5|Carlos|Araujo|7/25/2018|Fortaleza|3500|NaN|17500|
|1056|7392|HL7348|SmartWatch|3|Iuri|Barbosa|7/6/2018|Fortaleza|1400|NaN|4200|
|1057|7393|HL8851|Notebook|1|Carolina|Santos|12/24/2018|Fortaleza|3500|NaN|3500|
|1058|7401|HL9962|Android|1|Victor|Corrêa|11/2/2018|Fortaleza|3400|NaN|3400|
|1059|7408|HL9962|Android|1|Jonatas|Passos|11/3/2018|Fortaleza|3400|NaN|3400|
|1060|7420|HL1918|iPhone|3|Paola|Abreu|11/21/2018|Fortaleza|5300|NaN|15900|
|1061|7421|HL9962|Android|2|Rafael|Ramos|7/24/2018|Fortaleza|3400|NaN|6800|
|1062|7426|HL9962|Android|1|Caio|Moura|1/12/2018|Fortaleza|3400|NaN|3400|
|1063|7428|HL1918|iPhone|1|Giuseppe|Borges|2/9/2018|Fortaleza|5300|NaN|5300|
|1064|7429|HL4379|Televisão|5|Marina|Perdomo|3/22/2018|Fortaleza|2500|NaN|12500|
|1065|7438|HL1148|Câmera|4|Ramon|Araujo|5/2/2018|Fortaleza|2100|NaN|8400|
|1066|7439|HL1148|Câmera|1|Carlos|Cardoso|11/8/2018|Fortaleza|2100|NaN|2100|
|1067|7440|HL1148|Câmera|1|Bernard|Pedrosa|8/30/2018|Fortaleza|2100|NaN|2100|
|1068|7445|HL1918|iPhone|2|Adriane|Gomes|5/10/2018|Fortaleza|5300|NaN|10600|
|1069|7450|HL1148|Câmera|2|Guilherme|Assis|8/15/2018|Fortaleza|2100|NaN|4200|
|1070|7451|HL8851|Notebook|4|Wilson|Vianna|4/4/2018|Fortaleza|3500|NaN|14000|
|1071|7453|HL7348|SmartWatch|3|Marina|Cormack|5/19/2018|Fortaleza|1400|NaN|4200|
|1072|7455|HL2714|Tablet|2|Diego|Mello|4/10/2018|Fortaleza|1600|NaN|3200|
|1073|7457|HL1918|iPhone|5|Hércules|Moreira|2/28/2018|Fortaleza|5300|NaN|26500|
|1074|7468|HL1918|iPhone|5|Vitor|Boccaletti|1/20/2018|Fortaleza|5300|NaN|26500|
|1075|7477|HL4379|Televisão|4|Lucas|Freitas|7/31/2018|Fortaleza|2500|NaN|10000|
|1076|7484|HL9962|Android|2|Sthefeson|Pereira|9/29/2018|Fortaleza|3400|NaN|6800|
|1077|7507|HL4379|Televisão|3|Viviane|Cunha|6/8/2018|Fortaleza|2500|NaN|7500|
|1078|7509|HL9962|Android|1|Daniel|Sousa|1/6/2018|Fortaleza|3400|NaN|3400|
|1079|7521|HL2714|Tablet|4|Bruna|Gomes|7/9/2018|Fortaleza|1600|NaN|6400|
|1080|7524|HL4379|Televisão|5|Dykson|Silva|9/7/2018|Fortaleza|2500|NaN|12500|
|1081|7527|HL4379|Televisão|4|Beatriz|Silva|11/13/2018|Fortaleza|2500|NaN|10000|
|1082|7529|HL4379|Televisão|2|Renan|Nascimento|11/21/2018|Fortaleza|2500|NaN|5000|
|1083|7531|HL2714|Tablet|4|Luiza|Johnson|8/23/2018|Fortaleza|1600|NaN|6400|
|1084|7537|HL8851|Notebook|4|Carlos|Barbosa|2/21/2018|Fortaleza|3500|NaN|14000|
|1085|7545|HL2714|Tablet|5|Larissa|Vasconcellos|10/20/2018|Fortaleza|1600|NaN|8000|
|1086|7564|HL4379|Televisão|2|Lucas|Monte|12/15/2018|Fortaleza|2500|NaN|5000|
|1087|7573|HL4379|Televisão|5|Carolina|Vasconcelos|6/28/2018|Fortaleza|2500|NaN|12500|
|1088|7598|HL8851|Notebook|4|Gabriel|Puntel|7/14/2018|Fortaleza|3500|NaN|14000|
|1089|7602|HL7348|SmartWatch|5|Roberto|Nogueira|5/27/2018|Fortaleza|1400|NaN|7000|
|1090|7603|HL2714|Tablet|3|Jackson|Derossi|10/22/2018|Fortaleza|1600|NaN|4800|
|1091|7604|HL9962|Android|4|Rebeca|Manhães|9/27/2018|Fortaleza|3400|NaN|13600|
|1092|7606|HL1918|iPhone|2|Luis|Souza|8/10/2018|Fortaleza|5300|NaN|10600|
|1093|7612|HL8851|Notebook|4|Julia|Penteado|11/20/2018|Fortaleza|3500|NaN|14000|
|1094|7614|HL8851|Notebook|4|Débora|Lopes|10/2/2018|Fortaleza|3500|NaN|14000|
|1095|7616|HL7348|SmartWatch|4|Marcelo|Pereira|8/14/2018|Fortaleza|1400|NaN|5600|
|1096|7630|HL1148|Câmera|2|Deysiane|Medronho|6/15/2018|Fortaleza|2100|NaN|4200|
|1097|7634|HL1918|iPhone|1|João|Rodrigues|2/2/2018|Fortaleza|5300|NaN|5300|
|1098|7635|HL9962|Android|4|Ruan|Lopes|7/17/2018|Fortaleza|3400|NaN|13600|
|1099|7640|HL7348|SmartWatch|4|Thaís|Ribeiro|4/28/2018|Fortaleza|1400|NaN|5600|
|1100|7646|HL8851|Notebook|5|Nathan|Cunha|11/8/2018|Fortaleza|3500|NaN|17500|
|1101|7651|HL1918|iPhone|2|Fernanda|Coutinho|5/6/2018|Fortaleza|5300|NaN|10600|
|1102|7668|HL1918|iPhone|3|Pedro|Macckione|1/24/2018|Fortaleza|5300|NaN|15900|
|1103|7673|HL1148|Câmera|3|Alon|Fahrnholz|4/9/2018|Fortaleza|2100|NaN|6300|
|1104|7676|HL1918|iPhone|5|Bruna|Ramos|9/29/2018|Fortaleza|5300|NaN|26500|
|1105|7679|HL8851|Notebook|1|Thays|Castro|6/8/2018|Fortaleza|3500|NaN|3500|
|1106|7687|HL8851|Notebook|2|Allan|Guedes|8/9/2018|Fortaleza|3500|NaN|7000|
|1107|7688|HL7348|SmartWatch|1|Luíza|Melo|11/5/2018|Fortaleza|1400|NaN|1400|
|1108|7692|HL4379|Televisão|1|Lázaro|Nascimento|2/22/2018|Fortaleza|2500|NaN|2500|
|1109|7712|HL1148|Câmera|3|Anna|Maia|2/9/2018|Fortaleza|2100|NaN|6300|
|1110|7714|HL1148|Câmera|4|Julia|Aliani|11/2/2018|Fortaleza|2100|NaN|8400|
|1111|7722|HL1918|iPhone|1|Roberta|Pimenta|3/2/2018|Fortaleza|5300|NaN|5300|
|1112|7724|HL8851|Notebook|5|João|Ribeiro|9/11/2018|Fortaleza|3500|NaN|17500|
|1113|7726|HL8851|Notebook|3|Guilherme|Jordao|11/7/2018|Fortaleza|3500|NaN|10500|
|1114|7727|HL9962|Android|3|Bruno|Mota|2/27/2018|Fortaleza|3400|NaN|10200|
|1115|7731|HL1918|iPhone|1|Bruna|Soares|12/12/2018|Fortaleza|5300|NaN|5300|
|1116|7739|HL9962|Android|4|Carlos|Portela|8/9/2018|Fortaleza|3400|NaN|13600|
|1117|7743|HL4379|Televisão|2|Wendela|Mariz|10/13/2018|Fortaleza|2500|NaN|5000|
|1118|7767|HL1918|iPhone|4|Bernardo|Botelho|10/9/2018|Fortaleza|5300|NaN|21200|
|1119|7772|HL2714|Tablet|5|Jônatas|Tanaka|7/3/2018|Fortaleza|1600|NaN|8000|
|1120|7779|HL8851|Notebook|2|Rafael|Carneiro|1/7/2018|Fortaleza|3500|NaN|7000|
|1121|7800|HL1918|iPhone|2|Bianca|Tatsch|8/11/2018|Fortaleza|5300|NaN|10600|
|1122|7802|HL7348|SmartWatch|4|Ana|Felippe|11/9/2018|Fortaleza|1400|NaN|5600|
|1123|7803|HL1918|iPhone|5|Bárbara|Cavalcante|6/24/2018|Fortaleza|5300|NaN|26500|
|1124|7804|HL1148|Câmera|2|Caio|Fernandes|12/27/2018|Fortaleza|2100|NaN|4200|
|1125|7816|HL2714|Tablet|5|Bruno|Ferreira|11/10/2018|Fortaleza|1600|NaN|8000|
|1126|7817|HL1918|iPhone|3|Larissa|Cruz|10/30/2018|Fortaleza|5300|NaN|15900|
|1127|7819|HL8851|Notebook|3|Sandy|Ribeiro|9/1/2018|Fortaleza|3500|NaN|10500|
|1128|7824|HL4379|Televisão|2|Helvio|Pedrosa|12/14/2018|Fortaleza|2500|NaN|5000|
|1129|7835|HL1918|iPhone|5|Lucas|Lima|7/16/2018|Fortaleza|5300|NaN|26500|
|1130|7841|HL1148|Câmera|4|Tayla|Lima|11/15/2018|Fortaleza|2100|NaN|8400|
|1131|7846|HL1918|iPhone|3|Antonio|Bernhardt|1/18/2018|Fortaleza|5300|NaN|15900|
|1132|7852|HL9962|Android|3|Thiago|Nóbrega|1/30/2018|Fortaleza|3400|NaN|10200|
|1133|7877|HL4379|Televisão|1|Platini|Heimlich|7/4/2018|Fortaleza|2500|NaN|2500|
|1134|7883|HL1918|iPhone|1|Luiz|Freire|4/18/2018|Fortaleza|5300|NaN|5300|
|1135|7887|HL2714|Tablet|4|Renan|Nascimento|3/29/2018|Fortaleza|1600|NaN|6400|
|1136|7890|HL8851|Notebook|2|Lais|Candido|12/14/2018|Fortaleza|3500|NaN|7000|
|1137|7900|HL8851|Notebook|5|Fernanda|Silva|4/17/2018|Fortaleza|3500|NaN|17500|
|1138|7909|HL1918|iPhone|1|Sthefeson|Kohn|4/8/2018|Fortaleza|5300|NaN|5300|
|1139|7910|HL1918|iPhone|2|Katharina|Barros|2/3/2018|Fortaleza|5300|NaN|10600|
|1140|7913|HL2714|Tablet|2|Antonio|Manhães|4/23/2018|Fortaleza|1600|NaN|3200|
|1141|7926|HL8851|Notebook|4|Victor|Lira|7/29/2018|Fortaleza|3500|NaN|14000|
|1142|7963|HL4379|Televisão|4|Guilherme|Castilho|2/26/2018|Fortaleza|2500|NaN|10000|
|1143|7971|HL1918|iPhone|2|Alon|Pestana|9/20/2018|Fortaleza|5300|NaN|10600|
|1144|7972|HL1918|iPhone|1|Guilherme|Vianna|9/21/2018|Fortaleza|5300|NaN|5300|
|1145|7977|HL7348|SmartWatch|2|Lucas|Villanova|9/19/2018|Fortaleza|1400|NaN|2800|
|1146|7982|HL4379|Televisão|1|Roberta|Pimenta|8/26/2018|Fortaleza|2500|NaN|2500|
|1147|7994|HL4379|Televisão|1|Natalia|Guedes|6/19/2018|Fortaleza|2500|NaN|2500|
|1148|8001|HL8851|Notebook|3|Cassio|Faria|3/2/2018|Fortaleza|3500|NaN|10500|
|1149|8007|HL7348|SmartWatch|1|Daniel|Nauenberg|12/22/2018|Fortaleza|1400|NaN|1400|
|1150|8025|HL1918|iPhone|2|Raísa|Rodrigues|8/21/2018|Fortaleza|5300|NaN|10600|
|1151|8026|HL9962|Android|2|Beatriz|Perdomo|12/22/2018|Fortaleza|3400|NaN|6800|
|1152|8035|HL1918|iPhone|3|Sylvio|Bernhardt|7/22/2018|Fortaleza|5300|NaN|15900|
|1153|8036|HL8851|Notebook|5|Bárbara|Lima|9/22/2018|Fortaleza|3500|NaN|17500|
|1154|8046|HL1918|iPhone|3|João|Guadagnino|11/6/2018|Fortaleza|5300|NaN|15900|
|1155|8058|HL2714|Tablet|5|Daniel|Valente|4/24/2018|Fortaleza|1600|NaN|8000|
|1156|8059|HL8851|Notebook|1|Jônatas|Castro|7/19/2018|Fortaleza|3500|NaN|3500|
|1157|8067|HL9962|Android|4|João|Ribeiro|2/14/2018|Fortaleza|3400|NaN|13600|
|1158|8083|HL4379|Televisão|5|Victor|Franco|1/7/2018|Fortaleza|2500|NaN|12500|
|1159|8085|HL1918|iPhone|1|Roberta|Nogueira|11/8/2018|Fortaleza|5300|NaN|5300|
|1160|8099|HL1918|iPhone|5|Maria|Junior|10/28/2018|Fortaleza|5300|NaN|26500|
|1161|8118|HL9962|Android|5|Thales|Santos|7/1/2018|Fortaleza|3400|NaN|17000|
|1162|8125|HL9962|Android|1|Rafaela|Gomes|11/5/2018|Fortaleza|3400|NaN|3400|
|1163|8132|HL1918|iPhone|4|Matheus|Delgado|2/25/2018|Fortaleza|5300|NaN|21200|
|1164|8134|HL8851|Notebook|2|Eduardo|Nunes|3/23/2018|Fortaleza|3500|NaN|7000|
|1165|8150|HL4379|Televisão|4|Alon|Pestana|5/31/2018|Fortaleza|2500|NaN|10000|
|1166|8164|HL1918|iPhone|2|Milena|Pereira|5/1/2018|Fortaleza|5300|NaN|10600|
|1167|8169|HL9962|Android|4|Gabriel|Rocha|10/27/2018|Fortaleza|3400|NaN|13600|
|1168|8177|HL7348|SmartWatch|3|Mariana|Barrozo|10/15/2018|Fortaleza|1400|NaN|4200|
|1169|8183|HL4379|Televisão|5|Michelle|Figueiredo|1/6/2018|Fortaleza|2500|NaN|12500|
|1170|8191|HL1148|Câmera|3|Mariane|Ferreira|1/17/2018|Fortaleza|2100|NaN|6300|
|1171|8192|HL8851|Notebook|3|Carlos|Araujo|3/26/2018|Fortaleza|3500|NaN|10500|
|1172|8199|HL1918|iPhone|1|Matheus|Ramos|6/2/2018|Fortaleza|5300|NaN|5300|
|1173|8203|HL2714|Tablet|3|Cézar|Santos|5/23/2018|Fortaleza|1600|NaN|4800|
|1174|8211|HL1918|iPhone|2|Daniel|Sousa|12/1/2018|Fortaleza|5300|NaN|10600|
|1175|8222|HL1918|iPhone|3|Raphael|Machado|9/11/2018|Fortaleza|5300|NaN|15900|
|1176|8228|HL9962|Android|4|João|Fonseca|7/30/2018|Fortaleza|3400|NaN|13600|
|1177|8230|HL1918|iPhone|3|Isabel|Leite|11/21/2018|Fortaleza|5300|NaN|15900|
|1178|8233|HL1148|Câmera|4|Luiz|Limp|1/24/2018|Fortaleza|2100|NaN|8400|
|1179|8235|HL4379|Televisão|2|Beatriz|Biase|2/13/2018|Fortaleza|2500|NaN|5000|
|1180|8237|HL1148|Câmera|1|Victoria|Mazza|4/3/2018|Fortaleza|2100|NaN|2100|
|1181|8239|HL7348|SmartWatch|5|Júlio|Fraga|6/19/2018|Fortaleza|1400|NaN|7000|
|1182|8240|HL7348|SmartWatch|5|Gabrielle|Viríssimo|2/7/2018|Fortaleza|1400|NaN|7000|
|1183|8241|HL1918|iPhone|4|Victor|Lira|1/20/2018|Fortaleza|5300|NaN|21200|
|1184|8248|HL8851|Notebook|2|Pedro|Cardoso|1/15/2018|Fortaleza|3500|NaN|7000|
|1185|8250|HL2714|Tablet|3|Gabrielle|Figueiredo|4/11/2018|Fortaleza|1600|NaN|4800|
|1186|8251|HL7348|SmartWatch|3|Raphael|Mattos|5/23/2018|Fortaleza|1400|NaN|4200|
|1187|8255|HL1148|Câmera|5|Mariane|Racy|3/21/2018|Fortaleza|2100|NaN|10500|
|1188|8275|HL2714|Tablet|5|David|Assumpção|4/2/2018|Fortaleza|1600|NaN|8000|
|1189|8288|HL7348|SmartWatch|5|Thaís|Pereira|3/30/2018|Fortaleza|1400|NaN|7000|
|1190|8289|HL1918|iPhone|3|Pedro|Martins|6/11/2018|Fortaleza|5300|NaN|15900|
|1191|8290|HL2714|Tablet|3|Luis|Silva|12/2/2018|Fortaleza|1600|NaN|4800|
|1192|8294|HL1148|Câmera|4|Antonio|Manhães|10/27/2018|Fortaleza|2100|NaN|8400|
|1193|8296|HL4379|Televisão|3|Rodrigo|Silva|12/5/2018|Fortaleza|2500|NaN|7500|
|1194|8313|HL1918|iPhone|1|Dykson|Silva|1/1/2018|Fortaleza|5300|NaN|5300|
|1195|8329|HL1918|iPhone|4|Gustavo|Azevedo|10/2/2018|Fortaleza|5300|NaN|21200|
|1196|8338|HL9962|Android|3|Carolina|Alfradique|12/27/2018|Fortaleza|3400|NaN|10200|
|1197|8350|HL2714|Tablet|3|Juliana|Pacheco|8/6/2018|Fortaleza|1600|NaN|4800|
|1198|8359|HL8851|Notebook|5|Lorena|Carvalho|10/25/2018|Fortaleza|3500|NaN|17500|
|1199|8360|HL7348|SmartWatch|4|Daniel|Alcoforado|2/23/2018|Fortaleza|1400|NaN|5600|
|1200|8366|HL7348|SmartWatch|1|Felipe|Mello|5/6/2018|Fortaleza|1400|NaN|1400|
|1201|8367|HL1918|iPhone|2|Guilherme|Lima|4/14/2018|Fortaleza|5300|NaN|10600|
|1202|8371|HL4379|Televisão|2|Pedro|Delgado|6/13/2018|Fortaleza|2500|NaN|5000|
|1203|8373|HL2714|Tablet|3|Diogo|Peixoto|9/5/2018|Fortaleza|1600|NaN|4800|
|1204|8384|HL1918|iPhone|5|Marina|Miranda|1/28/2018|Fortaleza|5300|NaN|26500|
|1205|8402|HL1918|iPhone|5|Caroline|Pinto|11/24/2018|Fortaleza|5300|NaN|26500|
|1206|8407|HL4379|Televisão|1|Luana|Santana|8/5/2018|Fortaleza|2500|NaN|2500|
|1207|8415|HL4379|Televisão|2|Luis|Oliveira|4/1/2018|Fortaleza|2500|NaN|5000|
|1208|8432|HL2714|Tablet|3|Ana|Gonzaga|8/1/2018|Fortaleza|1600|NaN|4800|
|1209|8435|HL1918|iPhone|4|Gabriel|Ribeiro|5/27/2018|Fortaleza|5300|NaN|21200|
|1210|8441|HL1918|iPhone|2|Raphael|Kurtz|8/13/2018|Fortaleza|5300|NaN|10600|
|1211|8443|HL1918|iPhone|1|Ylana|Teraoka|1/30/2018|Fortaleza|5300|NaN|5300|
|1212|8444|HL8851|Notebook|5|Gabriel|Azevedo|9/3/2018|Fortaleza|3500|NaN|17500|
|1213|8454|HL4379|Televisão|3|Mayara|Soares|6/30/2018|Fortaleza|2500|NaN|7500|
|1214|8470|HL7348|SmartWatch|5|Pedro|Macckione|11/21/2018|Fortaleza|1400|NaN|7000|
|1215|8492|HL1918|iPhone|4|Luis|Garcia|4/12/2018|Fortaleza|5300|NaN|21200|
|1216|8521|HL1918|iPhone|3|Gabriella|Sagrillo|12/8/2018|Fortaleza|5300|NaN|15900|
|1217|8522|HL1918|iPhone|1|Luis|Silva|9/11/2018|Fortaleza|5300|NaN|5300|
|1218|8528|HL1148|Câmera|3|Beatriz|Rodrigues|8/21/2018|Fortaleza|2100|NaN|6300|
|1219|8533|HL2714|Tablet|5|Isabella|Montanholi|1/11/2018|Fortaleza|1600|NaN|8000|
|1220|8543|HL8851|Notebook|3|Bárbara|Lima|5/31/2018|Fortaleza|3500|NaN|10500|
|1221|8548|HL2714|Tablet|5|Anna|Silva|3/30/2018|Fortaleza|1600|NaN|8000|
|1222|8560|HL2714|Tablet|5|Thaís|Pereira|7/27/2018|Fortaleza|1600|NaN|8000|
|1223|8562|HL4379|Televisão|4|Guilherme|Seixas|5/16/2018|Fortaleza|2500|NaN|10000|
|1224|8570|HL2714|Tablet|3|Sthefeson|Barroso|11/28/2018|Fortaleza|1600|NaN|4800|
|1225|8573|HL1148|Câmera|2|Marina|Delgado|5/13/2018|Fortaleza|2100|NaN|4200|
|1226|8579|HL8851|Notebook|5|Priscila|Carvalho|7/30/2018|Fortaleza|3500|NaN|17500|
|1227|8581|HL2714|Tablet|2|Renan|Nascimento|8/29/2018|Fortaleza|1600|NaN|3200|
|1228|8583|HL8851|Notebook|4|Joyce|Souza|12/4/2018|Fortaleza|3500|NaN|14000|
|1229|8584|HL9962|Android|1|Jessica|Ferreira|2/19/2018|Fortaleza|3400|NaN|3400|
|1230|8585|HL8851|Notebook|4|Brenno|Santos|8/9/2018|Fortaleza|3500|NaN|14000|
|1231|8586|HL4379|Televisão|5|Arthur|Pereira|7/19/2018|Fortaleza|2500|NaN|12500|
|1232|8593|HL9962|Android|2|Bruna|Rosa|1/24/2018|Fortaleza|3400|NaN|6800|
|1233|8594|HL2714|Tablet|1|Beatriz|Biase|7/10/2018|Fortaleza|1600|NaN|1600|
|1234|8599|HL4379|Televisão|3|Luis|Garcia|8/8/2018|Fortaleza|2500|NaN|7500|
|1235|8603|HL8851|Notebook|3|Matheus|Gomes|5/18/2018|Fortaleza|3500|NaN|10500|
|1236|8606|HL9962|Android|4|Thales|Andrade|8/20/2018|Fortaleza|3400|NaN|13600|
|1237|8612|HL7348|SmartWatch|4|Matheus|Silva|1/24/2018|Fortaleza|1400|NaN|5600|
|1238|8618|HL1918|iPhone|4|Gustavo|Azevedo|12/18/2018|Fortaleza|5300|NaN|21200|
|1239|8620|HL1918|iPhone|2|Matheus|Gomes|3/26/2018|Fortaleza|5300|NaN|10600|
|1240|8629|HL7348|SmartWatch|5|Marcelo|Guadagnino|1/8/2018|Fortaleza|1400|NaN|7000|
|1241|8636|HL1918|iPhone|3|Luíza|Garcia|11/9/2018|Fortaleza|5300|NaN|15900|
|1242|8647|HL4379|Televisão|4|Lunna|Vannier|12/25/2018|Fortaleza|2500|NaN|10000|
|1243|8658|HL1148|Câmera|1|Pedro|Lyra|1/25/2018|Fortaleza|2100|NaN|2100|
|1244|8663|HL8851|Notebook|4|Caio|Silva|3/25/2018|Fortaleza|3500|NaN|14000|
|1245|8669|HL1918|iPhone|5|Lázaro|Villanova|2/6/2018|Fortaleza|5300|NaN|26500|
|1246|8677|HL4379|Televisão|5|Sandy|Moreira|2/4/2018|Fortaleza|2500|NaN|12500|
|1247|8689|HL4379|Televisão|1|Bianca|Tatsch|11/20/2018|Fortaleza|2500|NaN|2500|
|1248|8712|HL4379|Televisão|5|Stefan|Nunes|11/10/2018|Fortaleza|2500|NaN|12500|
|1249|8714|HL7348|SmartWatch|2|Alon|Palmeira|9/12/2018|Fortaleza|1400|NaN|2800|
|1250|8716|HL4379|Televisão|4|Carolina|Santos|10/9/2018|Fortaleza|2500|NaN|10000|
|1251|8728|HL4379|Televisão|3|Miguel|Carneiro|8/27/2018|Fortaleza|2500|NaN|7500|
|1252|8729|HL1148|Câmera|2|Rodrigo|Feijo|3/30/2018|Fortaleza|2100|NaN|4200|
|1253|8732|HL2714|Tablet|2|Lucas|Freitas|1/21/2018|Fortaleza|1600|NaN|3200|
|1254|8734|HL1918|iPhone|4|Fabio|Ramos|5/31/2018|Fortaleza|5300|NaN|21200|
|1255|8741|HL4379|Televisão|5|Vanessa|Rodrigues|8/24/2018|Fortaleza|2500|NaN|12500|
|1256|8757|HL1918|iPhone|4|Priscila|Suzano|3/29/2018|Fortaleza|5300|NaN|21200|
|1257|8774|HL1918|iPhone|3|Vittorio|Freitas|1/15/2018|Fortaleza|5300|NaN|15900|
|1258|8784|HL1918|iPhone|1|Rafael|Carneiro|2/25/2018|Fortaleza|5300|NaN|5300|
|1259|8796|HL7348|SmartWatch|2|Ives|Pinheiro|6/20/2018|Fortaleza|1400|NaN|2800|
|1260|8799|HL4379|Televisão|3|João|Monteiro|11/22/2018|Fortaleza|2500|NaN|7500|
|1261|8820|HL2714|Tablet|5|Julia|Silva|12/26/2018|Fortaleza|1600|NaN|8000|
|1262|8821|HL1918|iPhone|3|Henrique|Oliveira|4/25/2018|Fortaleza|5300|NaN|15900|
|1263|8825|HL1918|iPhone|1|Matheus|Delgado|4/2/2018|Fortaleza|5300|NaN|5300|
|1264|8828|HL1918|iPhone|4|Caio|Affonso|8/7/2018|Fortaleza|5300|NaN|21200|
|1265|8831|HL9962|Android|5|Izabel|Lopes|10/9/2018|Fortaleza|3400|NaN|17000|
|1266|8833|HL8851|Notebook|5|Bianca|Paz|5/15/2018|Fortaleza|3500|NaN|17500|
|1267|8836|HL1918|iPhone|2|Matheus|Ramos|6/10/2018|Fortaleza|5300|NaN|10600|
|1268|8847|HL1918|iPhone|2|José|Marques|4/13/2018|Fortaleza|5300|NaN|10600|
|1269|8853|HL8851|Notebook|5|Stela|Mendonça|4/16/2018|Fortaleza|3500|NaN|17500|
|1270|8873|HL1918|iPhone|2|Juliana|Silva|2/18/2018|Fortaleza|5300|NaN|10600|
|1271|8879|HL1918|iPhone|3|Caio|Caldas|7/27/2018|Fortaleza|5300|NaN|15900|
|1272|8881|HL9962|Android|3|Carolina|Alfradique|8/11/2018|Fortaleza|3400|NaN|10200|
|1273|8889|HL1918|iPhone|3|Daniel|Ortiz|3/4/2018|Fortaleza|5300|NaN|15900|
|1274|8903|HL1148|Câmera|1|Guilherme|Marchesi|6/18/2018|Fortaleza|2100|NaN|2100|
|1275|8906|HL4379|Televisão|4|Beatriz|Nogueira|1/20/2018|Fortaleza|2500|NaN|10000|
|1276|8917|HL8851|Notebook|1|Andreza|Ramos|6/5/2018|Fortaleza|3500|NaN|3500|
|1277|8938|HL8851|Notebook|1|Rilson|Guedes|2/4/2018|Fortaleza|3500|NaN|3500|
|1278|8940|HL4379|Televisão|5|Sthefeson|Barroso|7/14/2018|Fortaleza|2500|NaN|12500|
|1279|8950|HL4379|Televisão|5|Thales|Santos|11/10/2018|Fortaleza|2500|NaN|12500|
|1280|8951|HL4379|Televisão|3|Rodrigo|Silva|5/27/2018|Fortaleza|2500|NaN|7500|
|1281|8953|HL8851|Notebook|1|Pedro|Sena|9/14/2018|Fortaleza|3500|NaN|3500|
|1282|8955|HL8851|Notebook|1|Yasser|Calbucci|8/30/2018|Fortaleza|3500|NaN|3500|
|1283|8963|HL4379|Televisão|5|Daniel|Costa|6/6/2018|Fortaleza|2500|NaN|12500|
|1284|8979|HL8851|Notebook|5|Lucas|Freire|1/25/2018|Fortaleza|3500|NaN|17500|
|1285|8980|HL4379|Televisão|5|Caio|Vianna|6/21/2018|Fortaleza|2500|NaN|12500|
|1286|8987|HL4379|Televisão|3|Tayla|Lima|5/8/2018|Fortaleza|2500|NaN|7500|
|1287|8989|HL1148|Câmera|4|Felipe|Mendonça|3/18/2018|Fortaleza|2100|NaN|8400|
|1288|8993|HL7348|SmartWatch|3|Gabriel|Almeida|12/13/2018|Fortaleza|1400|NaN|4200|
|1289|9005|HL9962|Android|5|Brenno|Santos|7/23/2018|Fortaleza|3400|NaN|17000|
|1290|9011|HL2714|Tablet|2|Pedro|Ferrari|10/29/2018|Fortaleza|1600|NaN|3200|
|1291|9021|HL1148|Câmera|5|Deysiane|Medronho|4/13/2018|Fortaleza|2100|NaN|10500|
|1292|9024|HL1918|iPhone|2|Guilherme|Castilho|1/31/2018|Fortaleza|5300|NaN|10600|
|1293|9030|HL8851|Notebook|3|Ana|Silva|12/14/2018|Fortaleza|3500|NaN|10500|
|1294|9041|HL8851|Notebook|3|Caio|Silva|1/6/2018|Fortaleza|3500|NaN|10500|
|1295|9046|HL1918|iPhone|1|José|Marques|9/18/2018|Fortaleza|5300|NaN|5300|
|1296|9058|HL1918|iPhone|3|Carolina|Rocha|9/3/2018|Fortaleza|5300|NaN|15900|
|1297|9064|HL1918|iPhone|3|Michelle|Pereira|9/11/2018|Fortaleza|5300|NaN|15900|
|1298|9070|HL4379|Televisão|4|Guilherme|Lima|10/23/2018|Fortaleza|2500|NaN|10000|
|1299|9073|HL4379|Televisão|2|Felipe|Mendonça|2/28/2018|Fortaleza|2500|NaN|5000|
|1300|9077|HL1918|iPhone|3|Camilla|Cardeman|7/25/2018|Fortaleza|5300|NaN|15900|
|1301|9079|HL7348|SmartWatch|4|Ian|Almeida|4/9/2018|Fortaleza|1400|NaN|5600|
|1302|9081|HL8851|Notebook|3|Raphael|Mattos|8/19/2018|Fortaleza|3500|NaN|10500|
|1303|9082|HL1918|iPhone|5|Wilson|Miranda|6/16/2018|Fortaleza|5300|NaN|26500|
|1304|9084|HL2714|Tablet|4|Lucas|Rocha|12/12/2018|Fortaleza|1600|NaN|6400|
|1305|9092|HL2714|Tablet|2|Amanda|Procaci|6/20/2018|Fortaleza|1600|NaN|3200|
|1306|9100|HL9962|Android|1|Isabela|Resende|2/2/2018|Fortaleza|3400|NaN|3400|
|1307|9103|HL1918|iPhone|2|Lucas|Monte|5/14/2018|Fortaleza|5300|NaN|10600|
|1308|9107|HL1918|iPhone|2|Lorena|Kohn|3/16/2018|Fortaleza|5300|NaN|10600|
|1309|9108|HL4379|Televisão|3|Jorge|Fonseca|4/2/2018|Fortaleza|2500|NaN|7500|
|1310|9109|HL4379|Televisão|4|Anderson|Barreto|5/2/2018|Fortaleza|2500|NaN|10000|
|1311|9111|HL4379|Televisão|4|Fernanda|Figueiredo|8/1/2018|Fortaleza|2500|NaN|10000|
|1312|9112|HL1918|iPhone|5|Anna|Silva|4/11/2018|Fortaleza|5300|NaN|26500|
|1313|9133|HL4379|Televisão|1|Fernanda|Figueiredo|10/31/2018|Fortaleza|2500|NaN|2500|
|1314|9153|HL8851|Notebook|4|Thales|Andrade|5/14/2018|Fortaleza|3500|NaN|14000|
|1315|9170|HL4379|Televisão|2|Mariana|Miranda|12/30/2018|Fortaleza|2500|NaN|5000|
|1316|9172|HL4379|Televisão|2|Letícia|Araujo|3/24/2018|Fortaleza|2500|NaN|5000|
|1317|9184|HL1918|iPhone|3|Victor|Franco|11/13/2018|Fortaleza|5300|NaN|15900|
|1318|9187|HL8851|Notebook|5|Marina|Gama|10/13/2018|Fortaleza|3500|NaN|17500|
|1319|9192|HL9962|Android|1|Priscila|Garcia|10/2/2018|Fortaleza|3400|NaN|3400|
|1320|9194|HL1148|Câmera|4|Sandy|Moreira|12/26/2018|Fortaleza|2100|NaN|8400|
|1321|9201|HL1918|iPhone|3|Stephanie|Oliveira|6/9/2018|Fortaleza|5300|NaN|15900|
|1322|9204|HL1918|iPhone|2|Maria|Correa|10/27/2018|Fortaleza|5300|NaN|10600|
|1323|9211|HL4379|Televisão|3|Alexandre|Dantas|5/21/2018|Fortaleza|2500|NaN|7500|
|1324|9218|HL1918|iPhone|4|Leticia|Mesquita|8/8/2018|Fortaleza|5300|NaN|21200|
|1325|9219|HL8851|Notebook|2|Alexandre|Dantas|9/23/2018|Fortaleza|3500|NaN|7000|
|1326|9228|HL1918|iPhone|1|Luiz|Conceição|7/11/2018|Fortaleza|5300|NaN|5300|
|1327|9229|HL1918|iPhone|5|Carlos|Silva|12/12/2018|Fortaleza|5300|NaN|26500|
|1328|9237|HL7348|SmartWatch|2|Rafael|Guimarães|12/20/2018|Fortaleza|1400|NaN|2800|
|1329|9241|HL8851|Notebook|2|Julie|Ferreira|12/14/2018|Fortaleza|3500|NaN|7000|
|1330|9247|HL1918|iPhone|5|Wilson|Vianna|6/18/2018|Fortaleza|5300|NaN|26500|
|1331|9248|HL2714|Tablet|2|Aline|Morais|5/9/2018|Fortaleza|1600|NaN|3200|
|1332|9257|HL4379|Televisão|3|Vivianne|Rodrigues|6/28/2018|Fortaleza|2500|NaN|7500|
|1333|9258|HL7348|SmartWatch|5|Victor|Magalhães|8/14/2018|Fortaleza|1400|NaN|7000|
|1334|9260|HL1918|iPhone|2|Gabrielle|Wanderley|10/22/2018|Fortaleza|5300|NaN|10600|
|1335|9266|HL4379|Televisão|4|Caroline|Cavalcanti|2/11/2018|Fortaleza|2500|NaN|10000|
|1336|9268|HL1918|iPhone|3|Giovana|Vilela|2/17/2018|Fortaleza|5300|NaN|15900|
|1337|9270|HL1918|iPhone|2|Wendela|Veloso|4/14/2018|Fortaleza|5300|NaN|10600|
|1338|9282|HL1918|iPhone|3|Jeferson|Sone|10/18/2018|Fortaleza|5300|NaN|15900|
|1339|9284|HL8851|Notebook|5|Rebeca|Reis|3/17/2018|Fortaleza|3500|NaN|17500|
|1340|9288|HL9962|Android|5|Raísa|Rodrigues|12/29/2018|Fortaleza|3400|NaN|17000|
|1341|9310|HL2714|Tablet|3|Pedro|Sena|6/10/2018|Fortaleza|1600|NaN|4800|
|1342|9311|HL8851|Notebook|4|Camilla|Guimarães|5/9/2018|Fortaleza|3500|NaN|14000|
|1343|9319|HL9962|Android|3|Pedro|Ronfini|6/23/2018|Fortaleza|3400|NaN|10200|
|1344|9324|HL8851|Notebook|2|Alon|Palmeira|9/14/2018|Fortaleza|3500|NaN|7000|
|1345|9353|HL9962|Android|5|Lorena|Carvalho|4/25/2018|Fortaleza|3400|NaN|17000|
|1346|9367|HL4379|Televisão|5|João|Guadagnino|9/15/2018|Fortaleza|2500|NaN|12500|
|1347|9368|HL1918|iPhone|3|Caroline|Pinto|7/13/2018|Fortaleza|5300|NaN|15900|
|1348|9372|HL1918|iPhone|2|Felipe|Mello|2/28/2018|Fortaleza|5300|NaN|10600|
|1349|9381|HL1918|iPhone|2|Dykson|Silva|9/2/2018|Fortaleza|5300|NaN|10600|
|1350|9385|HL8851|Notebook|4|Jonatas|Essaber|8/4/2018|Fortaleza|3500|NaN|14000|
|1351|9423|HL1148|Câmera|1|Letícia|Rodrigues|11/5/2018|Fortaleza|2100|NaN|2100|
|1352|9428|HL4379|Televisão|5|Roberto|Nogueira|6/6/2018|Fortaleza|2500|NaN|12500|
|1353|9429|HL1918|iPhone|2|Guilherme|Rachide|8/20/2018|Fortaleza|5300|NaN|10600|
|1354|9435|HL2714|Tablet|1|Raul|Junqueira|3/27/2018|Fortaleza|1600|NaN|1600|
|1355|9443|HL8851|Notebook|2|Lucas|Lima|12/28/2018|Fortaleza|3500|NaN|7000|
|1356|9446|HL1918|iPhone|1|Carolina|Vasconcelos|12/10/2018|Fortaleza|5300|NaN|5300|
|1357|9449|HL9962|Android|3|Lucas|Wanderley|9/25/2018|Fortaleza|3400|NaN|10200|
|1358|9461|HL1148|Câmera|5|Tiago|Pereira|6/14/2018|Fortaleza|2100|NaN|10500|
|1359|9464|HL2714|Tablet|4|Luiz|Freire|4/23/2018|Fortaleza|1600|NaN|6400|
|1360|9471|HL2714|Tablet|1|Tadeu|Nakayama|11/8/2018|Fortaleza|1600|NaN|1600|
|1361|9482|HL9962|Android|2|Julia|Aliani|5/18/2018|Fortaleza|3400|NaN|6800|
|1362|9485|HL1148|Câmera|1|Anna|Maia|12/26/2018|Fortaleza|2100|NaN|2100|
|1363|9489|HL1918|iPhone|4|Daniel|Cardoso|11/4/2018|Fortaleza|5300|NaN|21200|
|1364|9497|HL4379|Televisão|5|Jorge|Carvalho|2/15/2018|Fortaleza|2500|NaN|12500|
|1365|9506|HL8851|Notebook|2|João|Capitulo|7/30/2018|Fortaleza|3500|NaN|7000|
|1366|9507|HL1148|Câmera|2|Rafael|Rocha|3/17/2018|Fortaleza|2100|NaN|4200|
|1367|9511|HL8851|Notebook|1|Camila|Sobral|12/19/2018|Fortaleza|3500|NaN|3500|
|1368|9517|HL9962|Android|5|Bruno|Oliveira|11/25/2018|Fortaleza|3400|NaN|17000|
|1369|9526|HL9962|Android|2|João|Monteiro|4/27/2018|Fortaleza|3400|NaN|6800|
|1370|9531|HL4379|Televisão|4|Joao|Pereira|12/15/2018|Fortaleza|2500|NaN|10000|
|1371|9532|HL7348|SmartWatch|5|Arthur|Portela|1/2/2018|Fortaleza|1400|NaN|7000|
|1372|9533|HL8851|Notebook|3|Stela|Mendonça|1/15/2018|Fortaleza|3500|NaN|10500|
|1373|9537|HL1918|iPhone|1|Marcelo|Borges|2/26/2018|Fortaleza|5300|NaN|5300|
|1374|9544|HL1918|iPhone|5|Eric|Carvalho|8/31/2018|Fortaleza|5300|NaN|26500|
|1375|9546|HL1148|Câmera|2|Julie|Ferreira|7/3/2018|Fortaleza|2100|NaN|4200|
|1376|9548|HL2714|Tablet|2|Carolina|Vasconcelos|9/1/2018|Fortaleza|1600|NaN|3200|
|1377|9550|HL4379|Televisão|2|Julia|Leite|9/5/2018|Fortaleza|2500|NaN|5000|
|1378|9551|HL2714|Tablet|1|Giovanna|Santos|12/18/2018|Fortaleza|1600|NaN|1600|
|1379|9555|HL7348|SmartWatch|1|Lucas|Cavalcanti|5/24/2018|Fortaleza|1400|NaN|1400|
|1380|9557|HL1918|iPhone|3|Ulisses|Filho|3/23/2018|Fortaleza|5300|NaN|15900|
|1381|9561|HL2714|Tablet|4|Victor|Franco|3/15/2018|Fortaleza|1600|NaN|6400|
|1382|9564|HL7348|SmartWatch|3|Célio|Xavier|11/4/2018|Fortaleza|1400|NaN|4200|
|1383|9565|HL2714|Tablet|5|Ana|Bôas|12/23/2018|Fortaleza|1600|NaN|8000|
|1384|9568|HL1148|Câmera|4|Silvio|Provenzano|8/19/2018|Fortaleza|2100|NaN|8400|
|1385|9570|HL1148|Câmera|2|Alex|Fernandes|12/1/2018|Fortaleza|2100|NaN|4200|
|1386|9571|HL1918|iPhone|1|Raphael|Rezende|4/29/2018|Fortaleza|5300|NaN|5300|
|1387|9575|HL7348|SmartWatch|5|Gabrielle|Silva|10/14/2018|Fortaleza|1400|NaN|7000|
|1388|9578|HL1918|iPhone|5|Bruna|Rangel|2/17/2018|Fortaleza|5300|NaN|26500|
|1389|9601|HL9962|Android|1|Silvio|Provenzano|3/30/2018|Fortaleza|3400|NaN|3400|
|1390|9606|HL1918|iPhone|1|José|Carvalho|6/22/2018|Fortaleza|5300|NaN|5300|
|1391|9615|HL9962|Android|3|José|Vieira|6/16/2018|Fortaleza|3400|NaN|10200|
|1392|9617|HL4379|Televisão|1|Silvio|Provenzano|1/20/2018|Fortaleza|2500|NaN|2500|
|1393|9618|HL4379|Televisão|1|Rilson|Guedes|3/21/2018|Fortaleza|2500|NaN|2500|
|1394|9619|HL1148|Câmera|1|Roberto|Tiradentes|8/26/2018|Fortaleza|2100|NaN|2100|
|1395|9646|HL1148|Câmera|2|Marcos|Nucci|5/21/2018|Fortaleza|2100|NaN|4200|
|1396|9647|HL4379|Televisão|5|Igor|Azevedo|1/3/2018|Fortaleza|2500|NaN|12500|
|1397|9650|HL1148|Câmera|3|Raphael|Guedes|6/23/2018|Fortaleza|2100|NaN|6300|
|1398|9661|HL1918|iPhone|4|Luis|Garcia|10/10/2018|Fortaleza|5300|NaN|21200|
|1399|9669|HL4379|Televisão|3|Eduardo|Peluzo|7/22/2018|Fortaleza|2500|NaN|7500|
|1400|9670|HL4379|Televisão|3|Bruna|Franco|6/24/2018|Fortaleza|2500|NaN|7500|
|1401|9672|HL9962|Android|4|Vitor|Boccaletti|8/8/2018|Fortaleza|3400|NaN|13600|
|1402|9678|HL7348|SmartWatch|5|Rodrigo|Mendes|7/22/2018|Fortaleza|1400|NaN|7000|
|1403|9683|HL1148|Câmera|1|Morgana|Correa|3/13/2018|Fortaleza|2100|NaN|2100|
|1404|9696|HL1918|iPhone|1|Jessica|Cordovil|7/17/2018|Fortaleza|5300|NaN|5300|
|1405|9698|HL2714|Tablet|3|Victor|Soares|7/11/2018|Fortaleza|1600|NaN|4800|
|1406|9706|HL1148|Câmera|2|Silvio|Provenzano|7/13/2018|Fortaleza|2100|NaN|4200|
|1407|9711|HL4379|Televisão|2|Amanda|Roberto|4/26/2018|Fortaleza|2500|NaN|5000|
|1408|9718|HL7348|SmartWatch|5|Diogo|Peixoto|10/21/2018|Fortaleza|1400|NaN|7000|
|1409|9727|HL4379|Televisão|1|Breno|Costa|11/22/2018|Fortaleza|2500|NaN|2500|
|1410|9733|HL1918|iPhone|3|Lunna|Vannier|12/5/2018|Fortaleza|5300|NaN|15900|
|1411|9738|HL4379|Televisão|4|Norman|Jimbo|5/8/2018|Fortaleza|2500|NaN|10000|
|1412|9739|HL1148|Câmera|4|José|Fonseca|10/3/2018|Fortaleza|2100|NaN|8400|
|1413|9746|HL7348|SmartWatch|1|Diego|Marchesi|12/4/2018|Fortaleza|1400|NaN|1400|
|1414|9751|HL4379|Televisão|2|Audir|Franco|8/17/2018|Fortaleza|2500|NaN|5000|
|1415|9765|HL1918|iPhone|1|Ana|Gomes|1/31/2018|Fortaleza|5300|NaN|5300|
|1416|9768|HL1148|Câmera|3|Lucas|Baptista|12/5/2018|Fortaleza|2100|NaN|6300|
|1417|9774|HL1918|iPhone|2|Amanda|Felippe|1/3/2018|Fortaleza|5300|NaN|10600|
|1418|9793|HL2714|Tablet|3|Juliana|Mesquita|10/28/2018|Fortaleza|1600|NaN|4800|
|1419|9797|HL1918|iPhone|5|Arthur|Fernandes|6/7/2018|Fortaleza|5300|NaN|26500|
|1420|9799|HL4379|Televisão|1|Joao|Pereira|11/14/2018|Fortaleza|2500|NaN|2500|
|1421|9811|HL1918|iPhone|4|João|Alves|11/18/2018|Fortaleza|5300|NaN|21200|
|1422|9812|HL8851|Notebook|1|Thaís|Pereira|1/7/2018|Fortaleza|3500|NaN|3500|
|1423|9813|HL1918|iPhone|5|Maria|Mello|4/21/2018|Fortaleza|5300|NaN|26500|
|1424|9824|HL4379|Televisão|1|Adriana|Passos|7/23/2018|Fortaleza|2500|NaN|2500|
|1425|9829|HL1148|Câmera|2|Lucas|Neto|8/19/2018|Fortaleza|2100|NaN|4200|
|1426|9830|HL4379|Televisão|3|Stephanie|Gonçalves|1/15/2018|Fortaleza|2500|NaN|7500|
|1427|9834|HL4379|Televisão|5|Myllena|Corrêa|12/11/2018|Fortaleza|2500|NaN|12500|
|1428|9843|HL8851|Notebook|4|Raíssa|Nimer|1/14/2018|Fortaleza|3500|NaN|14000|
|1429|9854|HL8851|Notebook|2|Eduardo|Pacheco|4/28/2018|Fortaleza|3500|NaN|7000|
|1430|9870|HL1918|iPhone|5|Jeferson|Costa|12/8/2018|Fortaleza|5300|NaN|26500|
|1431|9878|HL4379|Televisão|1|Sthefeson|Barroso|5/2/2018|Fortaleza|2500|NaN|2500|
|1432|9886|HL9962|Android|1|Bárbara|Lima|9/10/2018|Fortaleza|3400|NaN|3400|
|1433|9890|HL1918|iPhone|4|Pedro|Dalforne|6/20/2018|Fortaleza|5300|NaN|21200|
|1434|9893|HL1918|iPhone|3|Pedro|Costa|2/28/2018|Fortaleza|5300|NaN|15900|
|1435|9901|HL1918|iPhone|3|Renan|Melo|3/12/2018|Fortaleza|5300|NaN|15900|
|1436|9912|HL1918|iPhone|3|Tayla|Lima|8/14/2018|Fortaleza|5300|NaN|15900|
|1437|9913|HL8851|Notebook|2|Larissa|Jesus|1/26/2018|Fortaleza|3500|NaN|7000|
|1438|9914|HL4379|Televisão|2|Victor|Gomes|10/24/2018|Fortaleza|2500|NaN|5000|
|1439|9923|HL9962|Android|3|Daniel|Nauenberg|5/2/2018|Fortaleza|3400|NaN|10200|
|1440|9934|HL7348|SmartWatch|5|Carlos|Portela|9/3/2018|Fortaleza|1400|NaN|7000|
|1441|9956|HL1918|iPhone|3|Antônio|Soares|11/25/2018|Fortaleza|5300|NaN|15900|
|1442|9959|HL1918|iPhone|4|Rafael|Carneiro|6/19/2018|Fortaleza|5300|NaN|21200|
|1443|9974|HL1148|Câmera|2|Thales|Gouvêa|2/20/2018|Fortaleza|2100|NaN|4200|
|1444|9979|HL1918|iPhone|5|Brenno|Santos|10/18/2018|Fortaleza|5300|NaN|26500|
|1445|9994|HL4379|Televisão|2|Caio|Ferreira|5/18/2018|Fortaleza|2500|NaN|5000|
|1446|9995|HL1148|Câmera|5|Kim|Ferreira|3/6/2018|Fortaleza|2100|NaN|10500|
|0|14|HL4379|Televisão|4|Ylana|Teraoka|6/23/2018|Porto Alegre|2500|NaN|10000|
|1|34|HL1148|Câmera|1|Rubens|Netto|7/11/2018|Porto Alegre|2100|NaN|2100|
|2|43|HL1148|Câmera|5|Paloma|Sperandei|9/15/2018|Porto Alegre|2100|NaN|10500|
|3|49|HL8851|Notebook|5|Breno|Farias|6/24/2018|Porto Alegre|3500|NaN|17500|
|4|52|HL4379|Televisão|2|Lorena|Kohn|7/31/2018|Porto Alegre|2500|NaN|5000|
|5|55|HL1918|iPhone|4|Juliana|Goes|3/20/2018|Porto Alegre|5300|NaN|21200|
|6|68|HL8851|Notebook|3|Carlos|Melo|1/22/2018|Porto Alegre|3500|NaN|10500|
|7|71|HL9962|Android|4|Raphael|Machado|12/14/2018|Porto Alegre|3400|NaN|13600|
|8|74|HL7348|SmartWatch|2|Caroline|Aquino|4/12/2018|Porto Alegre|1400|NaN|2800|
|9|91|HL1148|Câmera|4|Ulisses|Filho|9/30/2018|Porto Alegre|2100|NaN|8400|
|10|95|HL1918|iPhone|3|Aline|Andrade|11/21/2018|Porto Alegre|5300|NaN|15900|
|11|113|HL4379|Televisão|5|Alexandre|Dantas|9/15/2018|Porto Alegre|2500|NaN|12500|
|12|120|HL8851|Notebook|3|Wilson|Vianna|10/27/2018|Porto Alegre|3500|NaN|10500|
|13|132|HL7348|SmartWatch|3|Carlos|Barbosa|2/26/2018|Porto Alegre|1400|NaN|4200|
|14|136|HL1918|iPhone|3|Roberta|Nogueira|10/17/2018|Porto Alegre|5300|NaN|15900|
|15|142|HL7348|SmartWatch|1|Pedro|Rodrigues|4/23/2018|Porto Alegre|1400|NaN|1400|
|16|160|HL4379|Televisão|2|Ravena|Bhering|11/24/2018|Porto Alegre|2500|NaN|5000|
|17|166|HL2714|Tablet|5|Bruna|Gomes|8/22/2018|Porto Alegre|1600|NaN|8000|
|18|193|HL9962|Android|3|Bianca|Paz|9/13/2018|Porto Alegre|3400|NaN|10200|
|19|214|HL4379|Televisão|2|Guilherme|Lima|5/31/2018|Porto Alegre|2500|NaN|5000|
|20|238|HL4379|Televisão|5|Clara|Bruno|1/17/2018|Porto Alegre|2500|NaN|12500|
|21|243|HL9962|Android|4|Giovana|Vilela|1/25/2018|Porto Alegre|3400|NaN|13600|
|22|282|HL4379|Televisão|4|Leonardo|Ferreira|2/5/2018|Porto Alegre|2500|NaN|10000|
|23|292|HL1918|iPhone|2|Gabrielle|Silva|10/1/2018|Porto Alegre|5300|NaN|10600|
|24|323|HL4379|Televisão|3|Iuri|Barbosa|8/18/2018|Porto Alegre|2500|NaN|7500|
|25|328|HL2714|Tablet|5|Bárbara|Cavalcante|6/18/2018|Porto Alegre|1600|NaN|8000|
|26|346|HL4379|Televisão|3|Lucas|Lima|7/18/2018|Porto Alegre|2500|NaN|7500|
|27|358|HL1918|iPhone|3|Rafaela|Gomes|6/2/2018|Porto Alegre|5300|NaN|15900|
|28|360|HL1918|iPhone|3|Arthur|Souza|12/31/2018|Porto Alegre|5300|NaN|15900|
|29|371|HL4379|Televisão|5|Thales|Portillo|7/23/2018|Porto Alegre|2500|NaN|12500|
|30|375|HL9962|Android|3|Gustavo|Azevedo|3/2/2018|Porto Alegre|3400|NaN|10200|
|31|398|HL1918|iPhone|1|Stefan|Nunes|11/24/2018|Porto Alegre|5300|NaN|5300|
|32|399|HL8851|Notebook|3|Mariana|Baptista|2/28/2018|Porto Alegre|3500|NaN|10500|
|33|402|HL2714|Tablet|5|Patrícia|Ferreira|2/3/2018|Porto Alegre|1600|NaN|8000|
|34|412|HL1918|iPhone|2|Ana|Júnior|10/27/2018|Porto Alegre|5300|NaN|10600|
|35|453|HL4379|Televisão|3|Alexandre|Dantas|1/9/2018|Porto Alegre|2500|NaN|7500|
|36|464|HL1918|iPhone|1|Natali|Rangel|1/9/2018|Porto Alegre|5300|NaN|5300|
|37|470|HL1918|iPhone|3|Victor|Firmino|3/31/2018|Porto Alegre|5300|NaN|15900|
|38|490|HL7348|SmartWatch|3|Paloma|Sperandei|2/9/2018|Porto Alegre|1400|NaN|4200|
|39|491|HL8851|Notebook|3|Guilherme|Castilho|9/16/2018|Porto Alegre|3500|NaN|10500|
|40|503|HL2714|Tablet|4|Jonatas|Passos|8/11/2018|Porto Alegre|1600|NaN|6400|
|41|506|HL7348|SmartWatch|1|Jonas|Gomes|4/10/2018|Porto Alegre|1400|NaN|1400|
|42|514|HL4379|Televisão|5|Carolina|Rocha|11/29/2018|Porto Alegre|2500|NaN|12500|
|43|523|HL8851|Notebook|5|Bruna|Rosa|6/27/2018|Porto Alegre|3500|NaN|17500|
|44|533|HL8851|Notebook|2|Laura|Araujo|9/9/2018|Porto Alegre|3500|NaN|7000|
|45|548|HL8851|Notebook|3|Thais|Rodrigues|10/11/2018|Porto Alegre|3500|NaN|10500|
|46|550|HL1918|iPhone|5|João|Junior|1/22/2018|Porto Alegre|5300|NaN|26500|
|47|555|HL4379|Televisão|3|Yasmim|Verly|6/17/2018|Porto Alegre|2500|NaN|7500|
|48|567|HL4379|Televisão|1|Wen|Santos|8/19/2018|Porto Alegre|2500|NaN|2500|
|49|591|HL1918|iPhone|4|Amanda|Braga|1/1/2018|Porto Alegre|5300|NaN|21200|
|50|599|HL1918|iPhone|1|Victor|Corrêa|4/15/2018|Porto Alegre|5300|NaN|5300|
|51|601|HL4379|Televisão|3|Julie|Ferreira|3/18/2018|Porto Alegre|2500|NaN|7500|
|52|627|HL2714|Tablet|4|Raul|Silveira|12/31/2018|Porto Alegre|1600|NaN|6400|
|53|651|HL8851|Notebook|1|Ananda|Dias|11/29/2018|Porto Alegre|3500|NaN|3500|
|54|680|HL1918|iPhone|2|Ana|Gonzaga|4/15/2018|Porto Alegre|5300|NaN|10600|
|55|708|HL9962|Android|1|Patrícia|Ferreira|11/22/2018|Porto Alegre|3400|NaN|3400|
|56|745|HL1148|Câmera|5|Letícia|Leal|7/10/2018|Porto Alegre|2100|NaN|10500|
|57|756|HL1918|iPhone|3|Antônio|Soares|1/14/2018|Porto Alegre|5300|NaN|15900|
|58|780|HL1918|iPhone|3|Matheus|Delgado|2/6/2018|Porto Alegre|5300|NaN|15900|
|59|789|HL1918|iPhone|3|Pedro|Bitencourt|3/10/2018|Porto Alegre|5300|NaN|15900|
|60|798|HL8851|Notebook|4|Bruno|Velucci|6/11/2018|Porto Alegre|3500|NaN|14000|
|61|808|HL1918|iPhone|1|Isabela|Chagas|9/26/2018|Porto Alegre|5300|NaN|5300|
|62|814|HL4379|Televisão|4|Luiza|Farias|10/8/2018|Porto Alegre|2500|NaN|10000|
|63|838|HL1148|Câmera|1|Raphael|Machado|3/3/2018|Porto Alegre|2100|NaN|2100|
|64|873|HL1918|iPhone|5|Bruno|Temporal|1/23/2018|Porto Alegre|5300|NaN|26500|
|65|883|HL1148|Câmera|3|Lais|Candido|11/9/2018|Porto Alegre|2100|NaN|6300|
|66|896|HL7348|SmartWatch|3|Larissa|Cruz|5/6/2018|Porto Alegre|1400|NaN|4200|
|67|904|HL1918|iPhone|5|Guilherme|Lima|9/17/2018|Porto Alegre|5300|NaN|26500|
|68|916|HL7348|SmartWatch|3|Ian|Almeida|10/15/2018|Porto Alegre|1400|NaN|4200|
|69|918|HL9962|Android|3|Paula|Cavalcanti|7/1/2018|Porto Alegre|3400|NaN|10200|
|70|921|HL1148|Câmera|5|Jorge|Fonseca|4/1/2018|Porto Alegre|2100|NaN|10500|
|71|926|HL2714|Tablet|2|Priscila|Suzano|8/14/2018|Porto Alegre|1600|NaN|3200|
|72|935|HL8851|Notebook|3|Bruno|Souza|8/1/2018|Porto Alegre|3500|NaN|10500|
|73|942|HL7348|SmartWatch|4|Felipe|Cavalcanti|2/26/2018|Porto Alegre|1400|NaN|5600|
|74|966|HL4379|Televisão|3|Douglas|Rodrigues|8/14/2018|Porto Alegre|2500|NaN|7500|
|75|984|HL7348|SmartWatch|3|Lucas|Reis|6/19/2018|Porto Alegre|1400|NaN|4200|
|76|987|HL4379|Televisão|5|Priscila|Garcia|3/11/2018|Porto Alegre|2500|NaN|12500|
|77|996|HL7348|SmartWatch|1|Leonardo|Faria|3/20/2018|Porto Alegre|1400|NaN|1400|
|78|1016|HL2714|Tablet|1|Antonio|Bernhardt|8/7/2018|Porto Alegre|1600|NaN|1600|
|79|1047|HL8851|Notebook|4|Antonio|Bernhardt|11/16/2018|Porto Alegre|3500|NaN|14000|
|80|1050|HL2714|Tablet|1|Marina|Delgado|3/12/2018|Porto Alegre|1600|NaN|1600|
|81|1067|HL8851|Notebook|4|Gabriel|Brito|5/28/2018|Porto Alegre|3500|NaN|14000|
|82|1104|HL1148|Câmera|3|Ulisses|Filho|9/2/2018|Porto Alegre|2100|NaN|6300|
|83|1119|HL9962|Android|1|Yasmim|Verly|8/8/2018|Porto Alegre|3400|NaN|3400|
|84|1145|HL1918|iPhone|2|Jeferson|Costa|8/3/2018|Porto Alegre|5300|NaN|10600|
|85|1166|HL8851|Notebook|3|Rojane|Lima|6/1/2018|Porto Alegre|3500|NaN|10500|
|86|1186|HL2714|Tablet|1|Lenon|Fernandes|12/19/2018|Porto Alegre|1600|NaN|1600|
|87|1205|HL4379|Televisão|1|Victor|Oliveira|3/17/2018|Porto Alegre|2500|NaN|2500|
|88|1210|HL8851|Notebook|4|Pedro|Buraco|11/26/2018|Porto Alegre|3500|NaN|14000|
|89|1226|HL9962|Android|1|Raul|Junqueira|11/12/2018|Porto Alegre|3400|NaN|3400|
|90|1241|HL1148|Câmera|5|Natalia|Guedes|8/29/2018|Porto Alegre|2100|NaN|10500|
|91|1253|HL1918|iPhone|5|Thais|Rodrigues|6/16/2018|Porto Alegre|5300|NaN|26500|
|92|1308|HL4379|Televisão|4|Thayna|Martins|11/13/2018|Porto Alegre|2500|NaN|10000|
|93|1342|HL4379|Televisão|1|Katharina|Barros|1/14/2018|Porto Alegre|2500|NaN|2500|
|94|1378|HL8851|Notebook|5|Tainah|Nogueira|5/15/2018|Porto Alegre|3500|NaN|17500|
|95|1396|HL8851|Notebook|2|Lívia|Marques|1/1/2018|Porto Alegre|3500|NaN|7000|
|96|1401|HL4379|Televisão|3|Juliana|Huon|4/27/2018|Porto Alegre|2500|NaN|7500|
|97|1411|HL1918|iPhone|3|Gabriela|Cavalcanti|1/8/2018|Porto Alegre|5300|NaN|15900|
|98|1420|HL2714|Tablet|2|Victor|Lira|11/3/2018|Porto Alegre|1600|NaN|3200|
|99|1424|HL4379|Televisão|1|João|Júnior|8/31/2018|Porto Alegre|2500|NaN|2500|
|100|1451|HL1918|iPhone|5|Pedro|Pereira|4/30/2018|Porto Alegre|5300|NaN|26500|
|101|1514|HL4379|Televisão|4|David|Campelo|5/14/2018|Porto Alegre|2500|NaN|10000|
|102|1515|HL4379|Televisão|1|Mateus|Polastri|6/17/2018|Porto Alegre|2500|NaN|2500|
|103|1541|HL1918|iPhone|4|Henrique|Villanova|6/12/2018|Porto Alegre|5300|NaN|21200|
|104|1544|HL2714|Tablet|5|Rebeca|Manhães|11/6/2018|Porto Alegre|1600|NaN|8000|
|105|1560|HL9962|Android|4|Stephanie|Novak|1/20/2018|Porto Alegre|3400|NaN|13600|
|106|1585|HL7348|SmartWatch|1|João|Pedrazza|7/8/2018|Porto Alegre|1400|NaN|1400|
|107|1591|HL1918|iPhone|5|Marcelo|Rosa|10/8/2018|Porto Alegre|5300|NaN|26500|
|108|1603|HL9962|Android|5|Paula|Cavalcanti|6/13/2018|Porto Alegre|3400|NaN|17000|
|109|1668|HL9962|Android|2|Rogério|Gentile|9/19/2018|Porto Alegre|3400|NaN|6800|
|110|1669|HL4379|Televisão|2|Bruno|Silva|6/25/2018|Porto Alegre|2500|NaN|5000|
|111|1680|HL9962|Android|1|Thomáz|Bôas|5/7/2018|Porto Alegre|3400|NaN|3400|
|112|1681|HL1918|iPhone|5|Lucas|Lemos|6/6/2018|Porto Alegre|5300|NaN|26500|
|113|1682|HL1918|iPhone|1|Rubens|Netto|11/11/2018|Porto Alegre|5300|NaN|5300|
|114|1683|HL1918|iPhone|2|Mariana|Barrozo|12/31/2018|Porto Alegre|5300|NaN|10600|
|115|1713|HL4379|Televisão|3|Juliana|Goes|8/13/2018|Porto Alegre|2500|NaN|7500|
|116|1717|HL2714|Tablet|5|Marcelo|Borges|6/27/2018|Porto Alegre|1600|NaN|8000|
|117|1725|HL4379|Televisão|1|Ulisses|Quinto|3/13/2018|Porto Alegre|2500|NaN|2500|
|118|1776|HL9962|Android|3|Cláudio|Aragão|11/3/2018|Porto Alegre|3400|NaN|10200|
|119|1786|HL1148|Câmera|1|Jéssica|Netto|1/13/2018|Porto Alegre|2100|NaN|2100|
|120|1819|HL4379|Televisão|5|Thales|Santos|12/3/2018|Porto Alegre|2500|NaN|12500|
|121|1854|HL1918|iPhone|3|Caio|Vianna|5/1/2018|Porto Alegre|5300|NaN|15900|
|122|1858|HL9962|Android|5|Amanda|Delgado|11/30/2018|Porto Alegre|3400|NaN|17000|
|123|1871|HL9962|Android|4|Fabio|Boccaletti|7/21/2018|Porto Alegre|3400|NaN|13600|
|124|1889|HL2714|Tablet|4|Joao|Silva|7/1/2018|Porto Alegre|1600|NaN|6400|
|125|1892|HL1918|iPhone|4|Patrícia|Amaral|7/2/2018|Porto Alegre|5300|NaN|21200|
|126|1910|HL1918|iPhone|4|Ana|Monte|5/19/2018|Porto Alegre|5300|NaN|21200|
|127|1936|HL8851|Notebook|5|Camilla|Vieira|1/23/2018|Porto Alegre|3500|NaN|17500|
|128|1957|HL1148|Câmera|4|Julia|Silva|10/29/2018|Porto Alegre|2100|NaN|8400|
|129|1959|HL1918|iPhone|2|Aline|Andrade|2/11/2018|Porto Alegre|5300|NaN|10600|
|130|1960|HL1918|iPhone|2|Stephanie|Novak|3/19/2018|Porto Alegre|5300|NaN|10600|
|131|1964|HL1918|iPhone|1|Julie|Ferreira|4/13/2018|Porto Alegre|5300|NaN|5300|
|132|1994|HL2714|Tablet|4|Marina|Miranda|1/11/2018|Porto Alegre|1600|NaN|6400|
|133|2028|HL1918|iPhone|2|Guilherme|Vianna|3/23/2018|Porto Alegre|5300|NaN|10600|
|134|2034|HL1148|Câmera|4|Ana|Felippe|8/25/2018|Porto Alegre|2100|NaN|8400|
|135|2052|HL1918|iPhone|2|Anízio|Carvalho|9/29/2018|Porto Alegre|5300|NaN|10600|
|136|2065|HL4379|Televisão|2|Juan|Barbosa|6/12/2018|Porto Alegre|2500|NaN|5000|
|137|2086|HL4379|Televisão|5|Julia|Leig|8/31/2018|Porto Alegre|2500|NaN|12500|
|138|2099|HL1918|iPhone|1|Daniel|Costa|9/13/2018|Porto Alegre|5300|NaN|5300|
|139|2110|HL1918|iPhone|4|Carolina|Alfradique|9/16/2018|Porto Alegre|5300|NaN|21200|
|140|2120|HL4379|Televisão|4|Bruno|Barcessat|11/27/2018|Porto Alegre|2500|NaN|10000|
|141|2121|HL4379|Televisão|1|Beatriz|Li|2/13/2018|Porto Alegre|2500|NaN|2500|
|142|2163|HL2714|Tablet|5|Wilson|Brandão|4/4/2018|Porto Alegre|1600|NaN|8000|
|143|2177|HL9962|Android|4|Natalia|Guedes|9/27/2018|Porto Alegre|3400|NaN|13600|
|144|2188|HL1918|iPhone|1|Arthur|Pereira|3/2/2018|Porto Alegre|5300|NaN|5300|
|145|2199|HL1918|iPhone|3|Cézar|Santos|12/4/2018|Porto Alegre|5300|NaN|15900|
|146|2202|HL4379|Televisão|5|Luiz|Almeida|8/18/2018|Porto Alegre|2500|NaN|12500|
|147|2205|HL9962|Android|4|Alon|Guedes|9/14/2018|Porto Alegre|3400|NaN|13600|
|148|2220|HL4379|Televisão|1|Thaís|Moura|11/7/2018|Porto Alegre|2500|NaN|2500|
|149|2224|HL7348|SmartWatch|5|Adriana|Carneiro|3/14/2018|Porto Alegre|1400|NaN|7000|
|150|2245|HL4379|Televisão|1|Caroll|Johnson|10/12/2018|Porto Alegre|2500|NaN|2500|
|151|2281|HL1148|Câmera|4|Matheus|Gomes|11/17/2018|Porto Alegre|2100|NaN|8400|
|152|2311|HL4379|Televisão|1|Bárbara|Lima|5/9/2018|Porto Alegre|2500|NaN|2500|
|153|2349|HL7348|SmartWatch|4|Rachel|Restum|12/24/2018|Porto Alegre|1400|NaN|5600|
|154|2354|HL1148|Câmera|2|Alon|Pestana|12/1/2018|Porto Alegre|2100|NaN|4200|
|155|2370|HL1918|iPhone|4|Breno|Caputo|1/4/2018|Porto Alegre|5300|NaN|21200|
|156|2407|HL1148|Câmera|3|Deysiane|Medronho|7/9/2018|Porto Alegre|2100|NaN|6300|
|157|2420|HL7348|SmartWatch|3|Bruna|Silva|7/3/2018|Porto Alegre|1400|NaN|4200|
|158|2421|HL1918|iPhone|2|Giuseppe|Bhering|9/3/2018|Porto Alegre|5300|NaN|10600|
|159|2443|HL9962|Android|1|Patrick|Silva|8/18/2018|Porto Alegre|3400|NaN|3400|
|160|2458|HL4379|Televisão|2|Thayane|Resende|3/28/2018|Porto Alegre|2500|NaN|5000|
|161|2473|HL8851|Notebook|1|Vitor|Campos|2/8/2018|Porto Alegre|3500|NaN|3500|
|162|2477|HL8851|Notebook|5|João|Castilho|2/20/2018|Porto Alegre|3500|NaN|17500|
|163|2482|HL2714|Tablet|1|Julia|Penteado|9/18/2018|Porto Alegre|1600|NaN|1600|
|164|2488|HL9962|Android|5|Myllena|Corrêa|7/8/2018|Porto Alegre|3400|NaN|17000|
|165|2491|HL4379|Televisão|5|Tadeu|Nakayama|4/10/2018|Porto Alegre|2500|NaN|12500|
|166|2499|HL7348|SmartWatch|1|Renan|Ventura|11/5/2018|Porto Alegre|1400|NaN|1400|
|167|2540|HL4379|Televisão|5|José|Seixas|11/2/2018|Porto Alegre|2500|NaN|12500|
|168|2551|HL2714|Tablet|5|Eduardo|Peluzo|10/23/2018|Porto Alegre|1600|NaN|8000|
|169|2565|HL9962|Android|5|Rachel|Restum|6/24/2018|Porto Alegre|3400|NaN|17000|
|170|2566|HL8851|Notebook|1|Raphael|Machado|4/9/2018|Porto Alegre|3500|NaN|3500|
|171|2584|HL1918|iPhone|5|Bruna|Franco|11/9/2018|Porto Alegre|5300|NaN|26500|
|172|2609|HL4379|Televisão|2|Fernanda|Silva|12/7/2018|Porto Alegre|2500|NaN|5000|
|173|2641|HL4379|Televisão|2|Mônica|Rotolo|11/29/2018|Porto Alegre|2500|NaN|5000|
|174|2645|HL9962|Android|2|Renan|Ventura|11/30/2018|Porto Alegre|3400|NaN|6800|
|175|2648|HL1148|Câmera|3|João|Rodrigues|1/8/2018|Porto Alegre|2100|NaN|6300|
|176|2649|HL4379|Televisão|2|Beatriz|Rocha|11/30/2018|Porto Alegre|2500|NaN|5000|
|177|2654|HL4379|Televisão|1|Luiza|Cavalcanti|4/2/2018|Porto Alegre|2500|NaN|2500|
|178|2681|HL7348|SmartWatch|3|Eduardo|Nunes|4/7/2018|Porto Alegre|1400|NaN|4200|
|179|2707|HL2714|Tablet|3|Matheus|Gomes|3/19/2018|Porto Alegre|1600|NaN|4800|
|180|2709|HL7348|SmartWatch|4|Amanda|Roberto|1/30/2018|Porto Alegre|1400|NaN|5600|
|181|2712|HL4379|Televisão|5|Matheus|Souza|6/2/2018|Porto Alegre|2500|NaN|12500|
|182|2741|HL1918|iPhone|3|Tadeu|Nakayama|9/7/2018|Porto Alegre|5300|NaN|15900|
|183|2753|HL2714|Tablet|5|Giovanna|Santos|1/15/2018|Porto Alegre|1600|NaN|8000|
|184|2761|HL1918|iPhone|1|Priscila|Vogel|6/11/2018|Porto Alegre|5300|NaN|5300|
|185|2787|HL2714|Tablet|1|Pedro|Ronfini|11/7/2018|Porto Alegre|1600|NaN|1600|
|186|2791|HL1918|iPhone|4|Pedro|Dalforne|4/4/2018|Porto Alegre|5300|NaN|21200|
|187|2796|HL4379|Televisão|3|Bruno|Mota|6/2/2018|Porto Alegre|2500|NaN|7500|
|188|2800|HL1148|Câmera|3|Caio|Moraes|1/8/2018|Porto Alegre|2100|NaN|6300|
|189|2833|HL1918|iPhone|3|Carolina|Motta|7/20/2018|Porto Alegre|5300|NaN|15900|
|190|2844|HL4379|Televisão|2|Lucas|Valim|8/27/2018|Porto Alegre|2500|NaN|5000|
|191|2857|HL1918|iPhone|3|Ana|Júnior|4/14/2018|Porto Alegre|5300|NaN|15900|
|192|2867|HL9962|Android|2|Mariana|Miranda|2/11/2018|Porto Alegre|3400|NaN|6800|
|193|2876|HL4379|Televisão|4|Izabel|Miura|4/4/2018|Porto Alegre|2500|NaN|10000|
|194|2892|HL1918|iPhone|4|Bruno|Temporal|10/26/2018|Porto Alegre|5300|NaN|21200|
|195|2894|HL8851|Notebook|3|Milena|Pereira|10/14/2018|Porto Alegre|3500|NaN|10500|
|196|2896|HL1148|Câmera|4|Guilherme|Assis|5/21/2018|Porto Alegre|2100|NaN|8400|
|197|2897|HL1918|iPhone|3|João|Fonseca|4/15/2018|Porto Alegre|5300|NaN|15900|
|198|2918|HL9962|Android|2|Arthur|Fernandes|3/17/2018|Porto Alegre|3400|NaN|6800|
|199|2929|HL1918|iPhone|4|Lucas|Almeida|12/1/2018|Porto Alegre|5300|NaN|21200|
|200|2935|HL8851|Notebook|1|Marina|Gama|12/19/2018|Porto Alegre|3500|NaN|3500|
|201|2947|HL2714|Tablet|3|Raul|Junqueira|5/25/2018|Porto Alegre|1600|NaN|4800|
|202|2972|HL4379|Televisão|4|Guilherme|Assis|10/4/2018|Porto Alegre|2500|NaN|10000|
|203|2982|HL1148|Câmera|2|Joyce|Medina|4/27/2018|Porto Alegre|2100|NaN|4200|
|204|3026|HL9962|Android|2|Marina|Correa|2/6/2018|Porto Alegre|3400|NaN|6800|
|205|3049|HL9962|Android|1|Julia|Leig|6/18/2018|Porto Alegre|3400|NaN|3400|
|206|3052|HL1148|Câmera|5|Juliana|Huon|3/13/2018|Porto Alegre|2100|NaN|10500|
|207|3059|HL1918|iPhone|5|Rafaela|Ferreira|1/10/2018|Porto Alegre|5300|NaN|26500|
|208|3064|HL1918|iPhone|5|Paulo|Campos|2/28/2018|Porto Alegre|5300|NaN|26500|
|209|3065|HL4379|Televisão|2|Adrielle|Forte|3/24/2018|Porto Alegre|2500|NaN|5000|
|210|3074|HL4379|Televisão|2|Yasmim|Verly|11/26/2018|Porto Alegre|2500|NaN|5000|
|211|3102|HL9962|Android|2|Tayla|Lima|7/3/2018|Porto Alegre|3400|NaN|6800|
|212|3122|HL1918|iPhone|2|Gabriela|Mello|6/7/2018|Porto Alegre|5300|NaN|10600|
|213|3129|HL4379|Televisão|3|Lívia|Marques|12/18/2018|Porto Alegre|2500|NaN|7500|
|214|3148|HL9962|Android|4|Maurício|Dias|2/28/2018|Porto Alegre|3400|NaN|13600|
|215|3172|HL9962|Android|4|Mateus|Maia|6/1/2018|Porto Alegre|3400|NaN|13600|
|216|3177|HL2714|Tablet|5|Hércules|Moreira|3/7/2018|Porto Alegre|1600|NaN|8000|
|217|3216|HL7348|SmartWatch|1|Gustavo|Azevedo|9/12/2018|Porto Alegre|1400|NaN|1400|
|218|3253|HL4379|Televisão|1|Bianca|Ferezin|10/18/2018|Porto Alegre|2500|NaN|2500|
|219|3294|HL1148|Câmera|4|Gabriel|Soares|1/17/2018|Porto Alegre|2100|NaN|8400|
|220|3377|HL1148|Câmera|3|Victor|Franco|12/2/2018|Porto Alegre|2100|NaN|6300|
|221|3378|HL1918|iPhone|5|Gabriel|Garcia|2/8/2018|Porto Alegre|5300|NaN|26500|
|222|3387|HL9962|Android|2|Lucas|Neto|12/4/2018|Porto Alegre|3400|NaN|6800|
|223|3395|HL1148|Câmera|4|Hércules|Júnior|8/8/2018|Porto Alegre|2100|NaN|8400|
|224|3404|HL9962|Android|4|Thiago|Miura|6/16/2018|Porto Alegre|3400|NaN|13600|
|225|3406|HL1148|Câmera|5|Victor|Zakhm|12/4/2018|Porto Alegre|2100|NaN|10500|
|226|3427|HL2714|Tablet|2|Vitor|Arruda|2/5/2018|Porto Alegre|1600|NaN|3200|
|227|3429|HL2714|Tablet|5|Lucas|Baptista|11/1/2018|Porto Alegre|1600|NaN|8000|
|228|3447|HL1918|iPhone|1|Gabriel|Azevedo|11/28/2018|Porto Alegre|5300|NaN|5300|
|229|3456|HL9962|Android|3|Lucas|Monte|11/25/2018|Porto Alegre|3400|NaN|10200|
|230|3460|HL9962|Android|4|Mayara|Soares|12/13/2018|Porto Alegre|3400|NaN|13600|
|231|3463|HL4379|Televisão|4|Gabriel|Almeida|5/13/2018|Porto Alegre|2500|NaN|10000|
|232|3503|HL1918|iPhone|2|Silvio|Fahrnholz|1/27/2018|Porto Alegre|5300|NaN|10600|
|233|3515|HL1918|iPhone|1|Marina|Correa|2/3/2018|Porto Alegre|5300|NaN|5300|
|234|3520|HL2714|Tablet|5|Victor|Ferreira|4/26/2018|Porto Alegre|1600|NaN|8000|
|235|3527|HL1918|iPhone|4|Michelle|Miura|10/20/2018|Porto Alegre|5300|NaN|21200|
|236|3566|HL1918|iPhone|4|Breno|Costa|11/15/2018|Porto Alegre|5300|NaN|21200|
|237|3578|HL4379|Televisão|5|Bruna|Silva|4/12/2018|Porto Alegre|2500|NaN|12500|
|238|3598|HL8851|Notebook|5|Livia|Codeceira|8/17/2018|Porto Alegre|3500|NaN|17500|
|239|3604|HL1918|iPhone|3|Luíza|Garcia|2/20/2018|Porto Alegre|5300|NaN|15900|
|240|3611|HL2714|Tablet|2|William|Mendonça|11/30/2018|Porto Alegre|1600|NaN|3200|
|241|3620|HL8851|Notebook|5|Vivianne|Rodrigues|9/4/2018|Porto Alegre|3500|NaN|17500|
|242|3632|HL1918|iPhone|2|Alexandre|Dantas|11/30/2018|Porto Alegre|5300|NaN|10600|
|243|3635|HL1918|iPhone|4|Victor|Corrêa|1/9/2018|Porto Alegre|5300|NaN|21200|
|244|3638|HL2714|Tablet|5|Pedro|Rodrigues|3/16/2018|Porto Alegre|1600|NaN|8000|
|245|3649|HL1918|iPhone|4|Vivianne|Rodrigues|3/28/2018|Porto Alegre|5300|NaN|21200|
|246|3678|HL1148|Câmera|5|Jeferson|Costa|3/9/2018|Porto Alegre|2100|NaN|10500|
|247|3685|HL8851|Notebook|5|Larissa|Cruz|3/25/2018|Porto Alegre|3500|NaN|17500|
|248|3702|HL1918|iPhone|2|Giulia|Pessanha|2/21/2018|Porto Alegre|5300|NaN|10600|
|249|3719|HL1918|iPhone|3|Eric|Carvalho|6/4/2018|Porto Alegre|5300|NaN|15900|
|250|3721|HL9962|Android|1|Rilson|Dias|9/20/2018|Porto Alegre|3400|NaN|3400|
|251|3730|HL1148|Câmera|1|Rebeca|Reis|11/11/2018|Porto Alegre|2100|NaN|2100|
|252|3738|HL1918|iPhone|4|Bruna|Silveira|7/9/2018|Porto Alegre|5300|NaN|21200|
|253|3751|HL4379|Televisão|2|Isabella|Scalabrin|12/11/2018|Porto Alegre|2500|NaN|5000|
|254|3762|HL4379|Televisão|1|Antonio|Bernhardt|4/8/2018|Porto Alegre|2500|NaN|2500|
|255|3764|HL1918|iPhone|2|Letícia|Rodrigues|6/2/2018|Porto Alegre|5300|NaN|10600|
|256|3767|HL4379|Televisão|2|Gabrielle|Costa|4/18/2018|Porto Alegre|2500|NaN|5000|
|257|3768|HL1918|iPhone|2|Raphael|Ferman|6/21/2018|Porto Alegre|5300|NaN|10600|
|258|3771|HL8851|Notebook|1|Rafael|Carneiro|11/14/2018|Porto Alegre|3500|NaN|3500|
|259|3780|HL7348|SmartWatch|4|Beatriz|Cavalcanti|7/20/2018|Porto Alegre|1400|NaN|5600|
|260|3820|HL4379|Televisão|1|Ana|Monte|9/26/2018|Porto Alegre|2500|NaN|2500|
|261|3825|HL1918|iPhone|2|João|Júnior|12/11/2018|Porto Alegre|5300|NaN|10600|
|262|3840|HL4379|Televisão|5|Manuela|Ferreira|5/21/2018|Porto Alegre|2500|NaN|12500|
|263|3843|HL1918|iPhone|2|Daniel|Cardoso|8/16/2018|Porto Alegre|5300|NaN|10600|
|264|3854|HL9962|Android|3|Alberto|Silveira|12/30/2018|Porto Alegre|3400|NaN|10200|
|265|3856|HL8851|Notebook|5|Antonio|Manhães|3/24/2018|Porto Alegre|3500|NaN|17500|
|266|3900|HL4379|Televisão|1|Marcos|Nucci|10/13/2018|Porto Alegre|2500|NaN|2500|
|267|3905|HL8851|Notebook|3|Jonas|Gomes|10/7/2018|Porto Alegre|3500|NaN|10500|
|268|3923|HL1918|iPhone|3|Stephanie|Gonçalves|3/20/2018|Porto Alegre|5300|NaN|15900|
|269|3931|HL8851|Notebook|2|Anna|Maia|7/12/2018|Porto Alegre|3500|NaN|7000|
|270|3935|HL1918|iPhone|1|Pedro|Costa|4/14/2018|Porto Alegre|5300|NaN|5300|
|271|3939|HL9962|Android|2|Danilo|Rubim|3/25/2018|Porto Alegre|3400|NaN|6800|
|272|3967|HL1918|iPhone|3|Daniel|Ortiz|5/22/2018|Porto Alegre|5300|NaN|15900|
|273|3987|HL9962|Android|5|Karina|Camara|9/9/2018|Porto Alegre|3400|NaN|17000|
|274|3997|HL1148|Câmera|1|Carlos|Azevedo|12/11/2018|Porto Alegre|2100|NaN|2100|
|275|4011|HL1918|iPhone|2|Sthefeson|Pereira|2/5/2018|Porto Alegre|5300|NaN|10600|
|276|4032|HL1918|iPhone|1|Arthur|Rocha|11/1/2018|Porto Alegre|5300|NaN|5300|
|277|4036|HL4379|Televisão|5|Jorge|Carvalho|5/23/2018|Porto Alegre|2500|NaN|12500|
|278|4039|HL2714|Tablet|5|Júlio|Freire|5/21/2018|Porto Alegre|1600|NaN|8000|
|279|4056|HL4379|Televisão|3|Bruno|Ursulino|5/15/2018|Porto Alegre|2500|NaN|7500|
|280|4066|HL1918|iPhone|5|Fernanda|Silva|8/8/2018|Porto Alegre|5300|NaN|26500|
|281|4076|HL1148|Câmera|2|Matheus|Tostes|10/20/2018|Porto Alegre|2100|NaN|4200|
|282|4121|HL7348|SmartWatch|1|Carlos|Souza|4/22/2018|Porto Alegre|1400|NaN|1400|
|283|4125|HL4379|Televisão|5|Raphael|Kurtz|10/4/2018|Porto Alegre|2500|NaN|12500|
|284|4134|HL7348|SmartWatch|4|Ana|Felippe|3/20/2018|Porto Alegre|1400|NaN|5600|
|285|4135|HL7348|SmartWatch|4|Carla|Zakhm|4/23/2018|Porto Alegre|1400|NaN|5600|
|286|4139|HL8851|Notebook|2|Isabel|Mesquita|1/2/2018|Porto Alegre|3500|NaN|7000|
|287|4159|HL1148|Câmera|3|Thiago|Nóbrega|1/8/2018|Porto Alegre|2100|NaN|6300|
|288|4164|HL2714|Tablet|3|Giovanna|Santos|10/13/2018|Porto Alegre|1600|NaN|4800|
|289|4189|HL1918|iPhone|5|Renan|Ventura|4/11/2018|Porto Alegre|5300|NaN|26500|
|290|4191|HL4379|Televisão|3|Bruno|Barcessat|9/5/2018|Porto Alegre|2500|NaN|7500|
|291|4217|HL2714|Tablet|1|Natália|Appel|7/30/2018|Porto Alegre|1600|NaN|1600|
|292|4224|HL7348|SmartWatch|1|Guilherme|Barbosa|10/21/2018|Porto Alegre|1400|NaN|1400|
|293|4274|HL1148|Câmera|1|Danilo|Alves|5/29/2018|Porto Alegre|2100|NaN|2100|
|294|4297|HL4379|Televisão|1|Débora|Lopes|10/4/2018|Porto Alegre|2500|NaN|2500|
|295|4303|HL4379|Televisão|5|Sandy|Moreira|2/28/2018|Porto Alegre|2500|NaN|12500|
|296|4318|HL9962|Android|4|Milena|Alcoforado|12/1/2018|Porto Alegre|3400|NaN|13600|
|297|4320|HL1918|iPhone|1|Vanessa|Rodrigues|2/23/2018|Porto Alegre|5300|NaN|5300|
|298|4332|HL9962|Android|1|José|Marques|11/21/2018|Porto Alegre|3400|NaN|3400|
|299|4351|HL1148|Câmera|2|Izabel|Miura|2/14/2018|Porto Alegre|2100|NaN|4200|
|300|4359|HL7348|SmartWatch|1|Silvio|Provenzano|11/8/2018|Porto Alegre|1400|NaN|1400|
|301|4372|HL4379|Televisão|3|Luiza|Cabral|5/24/2018|Porto Alegre|2500|NaN|7500|
|302|4380|HL4379|Televisão|2|Bernard|Pedrosa|1/18/2018|Porto Alegre|2500|NaN|5000|
|303|4391|HL1918|iPhone|4|Raul|Junqueira|9/23/2018|Porto Alegre|5300|NaN|21200|
|304|4406|HL4379|Televisão|4|Carlos|Mesquita|12/19/2018|Porto Alegre|2500|NaN|10000|
|305|4422|HL4379|Televisão|4|Clarissa|Santos|12/20/2018|Porto Alegre|2500|NaN|10000|
|306|4453|HL1918|iPhone|2|Gabriella|Lopes|9/29/2018|Porto Alegre|5300|NaN|10600|
|307|4457|HL4379|Televisão|5|Cláudio|Aragão|6/19/2018|Porto Alegre|2500|NaN|12500|
|308|4462|HL7348|SmartWatch|1|Lucas|Monte|7/1/2018|Porto Alegre|1400|NaN|1400|
|309|4473|HL1918|iPhone|3|Tiago|Pereira|5/17/2018|Porto Alegre|5300|NaN|15900|
|310|4502|HL9962|Android|3|Maria|Motta|6/28/2018|Porto Alegre|3400|NaN|10200|
|311|4526|HL7348|SmartWatch|3|Renan|Cunha|7/3/2018|Porto Alegre|1400|NaN|4200|
|312|4533|HL4379|Televisão|1|Guido|Monteiro|3/1/2018|Porto Alegre|2500|NaN|2500|
|313|4554|HL1918|iPhone|3|Caio|Cardoso|9/23/2018|Porto Alegre|5300|NaN|15900|
|314|4556|HL1148|Câmera|3|Gabriel|Azevedo|11/7/2018|Porto Alegre|2100|NaN|6300|
|315|4579|HL7348|SmartWatch|4|Lucas|Freitas|12/30/2018|Porto Alegre|1400|NaN|5600|
|316|4591|HL4379|Televisão|2|Victor|Gomes|10/1/2018|Porto Alegre|2500|NaN|5000|
|317|4597|HL1918|iPhone|5|Luísa|Fonseca|11/29/2018|Porto Alegre|5300|NaN|26500|
|318|4604|HL2714|Tablet|3|Carla|Zakhm|10/12/2018|Porto Alegre|1600|NaN|4800|
|319|4624|HL7348|SmartWatch|1|Rodrigo|Ramos|11/11/2018|Porto Alegre|1400|NaN|1400|
|320|4626|HL4379|Televisão|1|Carolina|Vasconcelos|1/8/2018|Porto Alegre|2500|NaN|2500|
|321|4631|HL8851|Notebook|1|Thiago|Veiga|2/7/2018|Porto Alegre|3500|NaN|3500|
|322|4652|HL9962|Android|1|Victor|Lira|8/23/2018|Porto Alegre|3400|NaN|3400|
|323|4682|HL1918|iPhone|1|Luiz|Mendonça|2/21/2018|Porto Alegre|5300|NaN|5300|
|324|4713|HL4379|Televisão|2|Matheus|Figueiredo|9/7/2018|Porto Alegre|2500|NaN|5000|
|325|4753|HL1918|iPhone|5|Camilla|Cardeman|3/2/2018|Porto Alegre|5300|NaN|26500|
|326|4754|HL9962|Android|2|Amanda|Delgado|5/28/2018|Porto Alegre|3400|NaN|6800|
|327|4797|HL1918|iPhone|3|Bárbara|Lima|6/2/2018|Porto Alegre|5300|NaN|15900|
|328|4825|HL1918|iPhone|2|Luiz|Campista|10/21/2018|Porto Alegre|5300|NaN|10600|
|329|4847|HL4379|Televisão|5|Fernanda|Figueiredo|9/17/2018|Porto Alegre|2500|NaN|12500|
|330|4851|HL7348|SmartWatch|4|Guilherme|Jordao|3/21/2018|Porto Alegre|1400|NaN|5600|
|331|4863|HL4379|Televisão|5|Tainah|Nogueira|7/27/2018|Porto Alegre|2500|NaN|12500|
|332|4866|HL1918|iPhone|3|Catarina|Teixeira|4/13/2018|Porto Alegre|5300|NaN|15900|
|333|4883|HL8851|Notebook|4|Beatriz|Li|12/31/2018|Porto Alegre|3500|NaN|14000|
|334|4940|HL8851|Notebook|4|Lívia|Tanaka|11/30/2018|Porto Alegre|3500|NaN|14000|
|335|4954|HL9962|Android|2|Eduardo|Peluzo|2/24/2018|Porto Alegre|3400|NaN|6800|
|336|4959|HL7348|SmartWatch|4|Pedro|Lyra|1/28/2018|Porto Alegre|1400|NaN|5600|
|337|4975|HL4379|Televisão|4|Adrielle|Gabriel|9/8/2018|Porto Alegre|2500|NaN|10000|
|338|5008|HL4379|Televisão|1|Mariana|Miranda|2/23/2018|Porto Alegre|2500|NaN|2500|
|339|5045|HL1918|iPhone|4|Rogério|Gentile|3/20/2018|Porto Alegre|5300|NaN|21200|
|340|5081|HL1918|iPhone|1|Giuseppe|Borges|12/19/2018|Porto Alegre|5300|NaN|5300|
|341|5084|HL9962|Android|1|Eduardo|Pacheco|4/26/2018|Porto Alegre|3400|NaN|3400|
|342|5088|HL1918|iPhone|5|Eric|Carvalho|8/3/2018|Porto Alegre|5300|NaN|26500|
|343|5106|HL1918|iPhone|1|Lucas|Baptista|2/28/2018|Porto Alegre|5300|NaN|5300|
|344|5107|HL2714|Tablet|3|Bruna|Brandao|12/30/2018|Porto Alegre|1600|NaN|4800|
|345|5111|HL8851|Notebook|1|Gabrielle|Costa|4/17/2018|Porto Alegre|3500|NaN|3500|
|346|5127|HL1918|iPhone|5|Barbara|Procaci|4/23/2018|Porto Alegre|5300|NaN|26500|
|347|5136|HL2714|Tablet|1|Bruna|Soares|9/27/2018|Porto Alegre|1600|NaN|1600|
|348|5137|HL1918|iPhone|1|Gabriel|Rubim|3/25/2018|Porto Alegre|5300|NaN|5300|
|349|5147|HL1148|Câmera|4|Bernard|Pedrosa|3/20/2018|Porto Alegre|2100|NaN|8400|
|350|5148|HL9962|Android|5|Wen|Braga|4/1/2018|Porto Alegre|3400|NaN|17000|
|351|5154|HL1148|Câmera|5|Vitor|Arruda|2/28/2018|Porto Alegre|2100|NaN|10500|
|352|5196|HL1148|Câmera|3|Rogério|Gentile|9/3/2018|Porto Alegre|2100|NaN|6300|
|353|5248|HL2714|Tablet|2|Antônio|Oliveira|2/26/2018|Porto Alegre|1600|NaN|3200|
|354|5267|HL9962|Android|3|Diego|Mello|2/9/2018|Porto Alegre|3400|NaN|10200|
|355|5284|HL4379|Televisão|2|Ana|Almeida|4/22/2018|Porto Alegre|2500|NaN|5000|
|356|5289|HL1918|iPhone|5|Pedro|Xavier|10/6/2018|Porto Alegre|5300|NaN|26500|
|357|5311|HL1918|iPhone|3|José|Carvalho|3/16/2018|Porto Alegre|5300|NaN|15900|
|358|5345|HL1918|iPhone|3|Ruan|Gonçalves|6/13/2018|Porto Alegre|5300|NaN|15900|
|359|5355|HL1918|iPhone|3|João|Júnior|6/27/2018|Porto Alegre|5300|NaN|15900|
|360|5383|HL9962|Android|4|Lázaro|Nascimento|2/28/2018|Porto Alegre|3400|NaN|13600|
|361|5385|HL2714|Tablet|3|Raphael|Guedes|3/16/2018|Porto Alegre|1600|NaN|4800|
|362|5397|HL4379|Televisão|5|Pedro|Martins|7/17/2018|Porto Alegre|2500|NaN|12500|
|363|5412|HL1148|Câmera|2|Barbara|Procaci|6/6/2018|Porto Alegre|2100|NaN|4200|
|364|5426|HL4379|Televisão|2|Arthur|Portela|12/10/2018|Porto Alegre|2500|NaN|5000|
|365|5435|HL2714|Tablet|4|Bruna|Londero|10/12/2018|Porto Alegre|1600|NaN|6400|
|366|5441|HL1918|iPhone|3|Morgana|Correa|2/24/2018|Porto Alegre|5300|NaN|15900|
|367|5443|HL1148|Câmera|5|Luiza|Cavalcanti|12/10/2018|Porto Alegre|2100|NaN|10500|
|368|5467|HL1918|iPhone|2|Wen|Braga|9/2/2018|Porto Alegre|5300|NaN|10600|
|369|5469|HL1148|Câmera|3|Luiza|Johnson|9/8/2018|Porto Alegre|2100|NaN|6300|
|370|5488|HL1918|iPhone|1|Victor|Magalhães|6/17/2018|Porto Alegre|5300|NaN|5300|
|371|5502|HL1918|iPhone|2|Luiz|Almeida|6/13/2018|Porto Alegre|5300|NaN|10600|
|372|5528|HL2714|Tablet|3|Bruno|Freitas|12/17/2018|Porto Alegre|1600|NaN|4800|
|373|5530|HL1918|iPhone|1|Carlos|Galvão|9/26/2018|Porto Alegre|5300|NaN|5300|
|374|5556|HL1148|Câmera|3|Luiz|Almeida|8/17/2018|Porto Alegre|2100|NaN|6300|
|375|5563|HL1918|iPhone|1|Raissa|Sales|9/1/2018|Porto Alegre|5300|NaN|5300|
|376|5583|HL7348|SmartWatch|2|Vitor|Arruda|6/21/2018|Porto Alegre|1400|NaN|2800|
|377|5593|HL4379|Televisão|3|Gabriel|Silva|10/21/2018|Porto Alegre|2500|NaN|7500|
|378|5611|HL4379|Televisão|1|Bianca|Piero|5/7/2018|Porto Alegre|2500|NaN|2500|
|379|5629|HL1918|iPhone|1|Wendela|Mariz|5/14/2018|Porto Alegre|5300|NaN|5300|
|380|5633|HL2714|Tablet|2|Daniel|Felippe|9/9/2018|Porto Alegre|1600|NaN|3200|
|381|5641|HL2714|Tablet|4|Barbara|Procaci|11/14/2018|Porto Alegre|1600|NaN|6400|
|382|5655|HL2714|Tablet|1|José|Fonseca|4/23/2018|Porto Alegre|1600|NaN|1600|
|383|5664|HL1918|iPhone|2|Vitor|Boccaletti|11/28/2018|Porto Alegre|5300|NaN|10600|
|384|5669|HL1918|iPhone|5|Cláudio|Aragão|9/16/2018|Porto Alegre|5300|NaN|26500|
|385|5676|HL4379|Televisão|3|Ives|Pinheiro|2/23/2018|Porto Alegre|2500|NaN|7500|
|386|5691|HL9962|Android|4|Lázaro|Nascimento|1/9/2018|Porto Alegre|3400|NaN|13600|
|387|5694|HL4379|Televisão|2|Matheus|Silva|7/7/2018|Porto Alegre|2500|NaN|5000|
|388|5696|HL1148|Câmera|1|Thiago|Veiga|1/31/2018|Porto Alegre|2100|NaN|2100|
|389|5700|HL2714|Tablet|1|Larissa|Vasconcellos|4/18/2018|Porto Alegre|1600|NaN|1600|
|390|5703|HL1148|Câmera|2|Daniel|Alcoforado|6/9/2018|Porto Alegre|2100|NaN|4200|
|391|5722|HL2714|Tablet|4|Guilherme|Assis|7/10/2018|Porto Alegre|1600|NaN|6400|
|392|5731|HL9962|Android|4|Ulisses|Arruda|9/5/2018|Porto Alegre|3400|NaN|13600|
|393|5737|HL1148|Câmera|5|Bruna|Londero|7/7/2018|Porto Alegre|2100|NaN|10500|
|394|5771|HL8851|Notebook|3|Cícero|Ramos|11/22/2018|Porto Alegre|3500|NaN|10500|
|395|5782|HL8851|Notebook|5|Bernardo|Botelho|4/19/2018|Porto Alegre|3500|NaN|17500|
|396|5787|HL1148|Câmera|2|Bruno|Oliveira|6/21/2018|Porto Alegre|2100|NaN|4200|
|397|5806|HL8851|Notebook|3|Julia|Penteado|5/8/2018|Porto Alegre|3500|NaN|10500|
|398|5814|HL1918|iPhone|5|Eduardo|Veiga|11/5/2018|Porto Alegre|5300|NaN|26500|
|399|5816|HL9962|Android|2|Mateus|Polastri|10/16/2018|Porto Alegre|3400|NaN|6800|
|400|5823|HL1918|iPhone|3|Fernanda|Coutinho|9/19/2018|Porto Alegre|5300|NaN|15900|
|401|5863|HL9962|Android|1|Arthur|Souza|8/3/2018|Porto Alegre|3400|NaN|3400|
|402|5869|HL9962|Android|3|Letícia|Leal|12/18/2018|Porto Alegre|3400|NaN|10200|
|403|5886|HL4379|Televisão|2|Amanda|Gontijo|10/25/2018|Porto Alegre|2500|NaN|5000|
|404|5897|HL1918|iPhone|4|Nina|Magalhães|6/17/2018|Porto Alegre|5300|NaN|21200|
|405|5907|HL9962|Android|1|Carlos|Barbosa|2/15/2018|Porto Alegre|3400|NaN|3400|
|406|5911|HL8851|Notebook|5|Roger|Rosa|8/15/2018|Porto Alegre|3500|NaN|17500|
|407|5926|HL4379|Televisão|2|Daniela|Andrada|12/30/2018|Porto Alegre|2500|NaN|5000|
|408|5930|HL1918|iPhone|2|Carlos|Mesquita|10/23/2018|Porto Alegre|5300|NaN|10600|
|409|5931|HL9962|Android|1|Débora|Lopes|5/18/2018|Porto Alegre|3400|NaN|3400|
|410|5936|HL2714|Tablet|4|Leandro|Ferreira|6/6/2018|Porto Alegre|1600|NaN|6400|
|411|5937|HL7348|SmartWatch|3|Juliana|Goes|3/10/2018|Porto Alegre|1400|NaN|4200|
|412|5969|HL4379|Televisão|1|Rubens|Valente|4/28/2018|Porto Alegre|2500|NaN|2500|
|413|5986|HL1148|Câmera|5|Vivianne|Rodrigues|12/7/2018|Porto Alegre|2100|NaN|10500|
|414|5988|HL4379|Televisão|3|Victor|Firmino|11/9/2018|Porto Alegre|2500|NaN|7500|
|415|6002|HL1148|Câmera|4|Lucas|Rodrigues|9/27/2018|Porto Alegre|2100|NaN|8400|
|416|6026|HL2714|Tablet|3|Júlia|Almeida|11/4/2018|Porto Alegre|1600|NaN|4800|
|417|6034|HL4379|Televisão|2|Pedro|Pereira|8/23/2018|Porto Alegre|2500|NaN|5000|
|418|6046|HL4379|Televisão|4|Thais|Rodrigues|3/30/2018|Porto Alegre|2500|NaN|10000|
|419|6061|HL1918|iPhone|1|Breno|Farias|6/20/2018|Porto Alegre|5300|NaN|5300|
|420|6069|HL4379|Televisão|1|Bruno|Silva|11/19/2018|Porto Alegre|2500|NaN|2500|
|421|6075|HL2714|Tablet|4|Anderson|Barreto|4/14/2018|Porto Alegre|1600|NaN|6400|
|422|6076|HL1918|iPhone|2|Pedro|Macckione|6/30/2018|Porto Alegre|5300|NaN|10600|
|423|6086|HL1918|iPhone|4|Manuela|Merege|1/6/2018|Porto Alegre|5300|NaN|21200|
|424|6089|HL1918|iPhone|1|Beatriz|Almeida|1/9/2018|Porto Alegre|5300|NaN|5300|
|425|6148|HL4379|Televisão|5|Diego|Barros|3/25/2018|Porto Alegre|2500|NaN|12500|
|426|6172|HL1148|Câmera|4|Lucas|Destri|11/15/2018|Porto Alegre|2100|NaN|8400|
|427|6175|HL8851|Notebook|5|Lucas|Almeida|1/27/2018|Porto Alegre|3500|NaN|17500|
|428|6191|HL2714|Tablet|1|Lucas|Costa|9/7/2018|Porto Alegre|1600|NaN|1600|
|429|6199|HL9962|Android|3|Daniel|Araujo|12/29/2018|Porto Alegre|3400|NaN|10200|
|430|6232|HL4379|Televisão|5|Mariana|Rotava|1/12/2018|Porto Alegre|2500|NaN|12500|
|431|6245|HL1918|iPhone|1|Matheus|Gomes|2/27/2018|Porto Alegre|5300|NaN|5300|
|432|6250|HL7348|SmartWatch|4|Gabriel|Silva|5/24/2018|Porto Alegre|1400|NaN|5600|
|433|6253|HL7348|SmartWatch|3|Lunna|Vannier|7/3/2018|Porto Alegre|1400|NaN|4200|
|434|6268|HL7348|SmartWatch|4|Ana|Felippe|4/12/2018|Porto Alegre|1400|NaN|5600|
|435|6277|HL4379|Televisão|1|Lucas|Aragão|12/4/2018|Porto Alegre|2500|NaN|2500|
|436|6282|HL7348|SmartWatch|1|Cézar|Santos|4/14/2018|Porto Alegre|1400|NaN|1400|
|437|6307|HL1918|iPhone|1|Catarina|Teixeira|4/19/2018|Porto Alegre|5300|NaN|5300|
|438|6321|HL1918|iPhone|1|Rafael|Portela|1/23/2018|Porto Alegre|5300|NaN|5300|
|439|6329|HL4379|Televisão|4|Hércules|Júnior|7/4/2018|Porto Alegre|2500|NaN|10000|
|440|6337|HL4379|Televisão|2|Mariana|Rotava|2/5/2018|Porto Alegre|2500|NaN|5000|
|441|6367|HL9962|Android|5|Lenon|Fernandes|5/11/2018|Porto Alegre|3400|NaN|17000|
|442|6388|HL9962|Android|2|Thiago|Veloso|1/28/2018|Porto Alegre|3400|NaN|6800|
|443|6392|HL2714|Tablet|2|Gabriel|Soares|11/20/2018|Porto Alegre|1600|NaN|3200|
|444|6394|HL4379|Televisão|5|Julia|Silva|10/9/2018|Porto Alegre|2500|NaN|12500|
|445|6402|HL4379|Televisão|1|Bernardo|Soares|2/15/2018|Porto Alegre|2500|NaN|2500|
|446|6405|HL1148|Câmera|5|Karina|Camara|7/14/2018|Porto Alegre|2100|NaN|10500|
|447|6424|HL1148|Câmera|1|Juliana|Mesquita|7/12/2018|Porto Alegre|2100|NaN|2100|
|448|6430|HL4379|Televisão|4|Patrícia|Fernandes|9/25/2018|Porto Alegre|2500|NaN|10000|
|449|6433|HL2714|Tablet|2|Beatriz|Perdomo|5/29/2018|Porto Alegre|1600|NaN|3200|
|450|6466|HL4379|Televisão|2|Julia|Leite|3/22/2018|Porto Alegre|2500|NaN|5000|
|451|6496|HL9962|Android|5|Pedro|Santos|7/6/2018|Porto Alegre|3400|NaN|17000|
|452|6502|HL1918|iPhone|1|Ananda|Dias|10/25/2018|Porto Alegre|5300|NaN|5300|
|453|6504|HL7348|SmartWatch|3|Anderson|Martins|12/9/2018|Porto Alegre|1400|NaN|4200|
|454|6506|HL2714|Tablet|5|Caio|Fernandes|7/3/2018|Porto Alegre|1600|NaN|8000|
|455|6521|HL1148|Câmera|2|Roberto|Nogueira|1/22/2018|Porto Alegre|2100|NaN|4200|
|456|6529|HL4379|Televisão|2|Patrícia|Amaral|6/5/2018|Porto Alegre|2500|NaN|5000|
|457|6551|HL1148|Câmera|1|Guilherme|Merotto|11/18/2018|Porto Alegre|2100|NaN|2100|
|458|6559|HL1918|iPhone|2|Ana|Soledade|1/23/2018|Porto Alegre|5300|NaN|10600|
|459|6582|HL1148|Câmera|3|Breno|Varella|6/17/2018|Porto Alegre|2100|NaN|6300|
|460|6600|HL1918|iPhone|5|Gabriela|Cavalcanti|7/31/2018|Porto Alegre|5300|NaN|26500|
|461|6613|HL9962|Android|2|Victoria|Tavares|3/15/2018|Porto Alegre|3400|NaN|6800|
|462|6627|HL1918|iPhone|3|Paula|Calbucci|3/28/2018|Porto Alegre|5300|NaN|15900|
|463|6655|HL9962|Android|1|Luis|Silva|6/3/2018|Porto Alegre|3400|NaN|3400|
|464|6668|HL7348|SmartWatch|5|João|Abraçado|6/22/2018|Porto Alegre|1400|NaN|7000|
|465|6669|HL1148|Câmera|1|Sarah|Souza|12/9/2018|Porto Alegre|2100|NaN|2100|
|466|6674|HL1918|iPhone|1|Carolina|Carneiro|6/29/2018|Porto Alegre|5300|NaN|5300|
|467|6706|HL2714|Tablet|5|José|Carvalho|10/8/2018|Porto Alegre|1600|NaN|8000|
|468|6723|HL4379|Televisão|4|Leonardo|Faria|1/22/2018|Porto Alegre|2500|NaN|10000|
|469|6739|HL1918|iPhone|4|Wen|Santos|4/28/2018|Porto Alegre|5300|NaN|21200|
|470|6784|HL9962|Android|1|Bernardo|Ribeiro|3/17/2018|Porto Alegre|3400|NaN|3400|
|471|6791|HL4379|Televisão|4|Gabrielle|Figueiredo|1/18/2018|Porto Alegre|2500|NaN|10000|
|472|6794|HL4379|Televisão|5|Luiza|Cavalcanti|10/30/2018|Porto Alegre|2500|NaN|12500|
|473|6814|HL7348|SmartWatch|2|Victoria|Mazza|2/26/2018|Porto Alegre|1400|NaN|2800|
|474|6820|HL2714|Tablet|5|Guilherme|Monteiro|4/23/2018|Porto Alegre|1600|NaN|8000|
|475|6907|HL2714|Tablet|5|Ives|Barbosa|3/20/2018|Porto Alegre|1600|NaN|8000|
|476|6923|HL2714|Tablet|3|Hygor|Essaber|6/1/2018|Porto Alegre|1600|NaN|4800|
|477|6959|HL1918|iPhone|1|Rebeca|Taylor|5/1/2018|Porto Alegre|5300|NaN|5300|
|478|6966|HL9962|Android|4|Gustavo|Accardo|8/8/2018|Porto Alegre|3400|NaN|13600|
|479|6971|HL1918|iPhone|2|Julie|Ferreira|9/14/2018|Porto Alegre|5300|NaN|10600|
|480|6973|HL1148|Câmera|2|Felipe|Júnior|5/28/2018|Porto Alegre|2100|NaN|4200|
|481|6987|HL8851|Notebook|4|Elena|Barreto|2/24/2018|Porto Alegre|3500|NaN|14000|
|482|7021|HL2714|Tablet|3|Giulia|Pessanha|9/10/2018|Porto Alegre|1600|NaN|4800|
|483|7024|HL1918|iPhone|5|João|Menezes|8/5/2018|Porto Alegre|5300|NaN|26500|
|484|7028|HL4379|Televisão|5|Carlos|Mesquita|10/22/2018|Porto Alegre|2500|NaN|12500|
|485|7035|HL1918|iPhone|5|Carolina|Alfradique|7/24/2018|Porto Alegre|5300|NaN|26500|
|486|7037|HL1148|Câmera|1|Rogério|Gentile|7/18/2018|Porto Alegre|2100|NaN|2100|
|487|7063|HL9962|Android|4|Manuela|Merege|12/22/2018|Porto Alegre|3400|NaN|13600|
|488|7082|HL1148|Câmera|4|Joao|Pereira|3/23/2018|Porto Alegre|2100|NaN|8400|
|489|7114|HL8851|Notebook|2|Paula|Isbelle|3/4/2018|Porto Alegre|3500|NaN|7000|
|490|7117|HL7348|SmartWatch|2|Caio|Affonso|5/13/2018|Porto Alegre|1400|NaN|2800|
|491|7178|HL8851|Notebook|2|Thiago|Costa|7/6/2018|Porto Alegre|3500|NaN|7000|
|492|7186|HL1148|Câmera|1|Stephanie|Oliveira|10/2/2018|Porto Alegre|2100|NaN|2100|
|493|7195|HL2714|Tablet|5|Lucas|Assunção|10/23/2018|Porto Alegre|1600|NaN|8000|
|494|7205|HL1918|iPhone|3|Mariana|Barrozo|5/24/2018|Porto Alegre|5300|NaN|15900|
|495|7220|HL4379|Televisão|5|Yasmim|Verly|4/6/2018|Porto Alegre|2500|NaN|12500|
|496|7245|HL4379|Televisão|5|Alessandra|Martins|7/26/2018|Porto Alegre|2500|NaN|12500|
|497|7262|HL4379|Televisão|4|Marcos|Nucci|7/27/2018|Porto Alegre|2500|NaN|10000|
|498|7266|HL1918|iPhone|5|Julia|Figueiredo|1/23/2018|Porto Alegre|5300|NaN|26500|
|499|7270|HL9962|Android|5|Pedro|Ronfini|12/28/2018|Porto Alegre|3400|NaN|17000|
|500|7279|HL1148|Câmera|4|Itai|Puntel|5/10/2018|Porto Alegre|2100|NaN|8400|
|501|7336|HL9962|Android|3|Victor|Gomes|9/29/2018|Porto Alegre|3400|NaN|10200|
|502|7358|HL8851|Notebook|2|Breno|Costa|10/13/2018|Porto Alegre|3500|NaN|7000|
|503|7379|HL4379|Televisão|2|Tainah|Nogueira|1/20/2018|Porto Alegre|2500|NaN|5000|
|504|7397|HL7348|SmartWatch|1|Thiago|Veloso|4/29/2018|Porto Alegre|1400|NaN|1400|
|505|7402|HL7348|SmartWatch|5|Adrielle|Vieira|3/14/2018|Porto Alegre|1400|NaN|7000|
|506|7405|HL1918|iPhone|5|Arthur|Pereira|10/26/2018|Porto Alegre|5300|NaN|26500|
|507|7412|HL1918|iPhone|5|Gabriel|Assis|10/12/2018|Porto Alegre|5300|NaN|26500|
|508|7414|HL1918|iPhone|3|Patrick|Silva|1/4/2018|Porto Alegre|5300|NaN|15900|
|509|7418|HL1918|iPhone|2|Jackson|Derossi|7/20/2018|Porto Alegre|5300|NaN|10600|
|510|7430|HL7348|SmartWatch|1|José|Fonseca|5/21/2018|Porto Alegre|1400|NaN|1400|
|511|7441|HL9962|Android|4|Henrique|Villanova|5/13/2018|Porto Alegre|3400|NaN|13600|
|512|7464|HL1918|iPhone|4|Joana|Calmon|7/10/2018|Porto Alegre|5300|NaN|21200|
|513|7467|HL9962|Android|3|Karina|Camara|10/4/2018|Porto Alegre|3400|NaN|10200|
|514|7473|HL9962|Android|2|Karine|Barros|10/30/2018|Porto Alegre|3400|NaN|6800|
|515|7511|HL1918|iPhone|4|Thiago|Nóbrega|4/5/2018|Porto Alegre|5300|NaN|21200|
|516|7534|HL9962|Android|5|Priscila|Vogel|1/7/2018|Porto Alegre|3400|NaN|17000|
|517|7535|HL1918|iPhone|1|Ives|Barbosa|2/23/2018|Porto Alegre|5300|NaN|5300|
|518|7553|HL4379|Televisão|2|Lázaro|Villanova|3/7/2018|Porto Alegre|2500|NaN|5000|
|519|7556|HL9962|Android|5|Caio|Silva|7/1/2018|Porto Alegre|3400|NaN|17000|
|520|7590|HL8851|Notebook|4|Caio|Moraes|9/5/2018|Porto Alegre|3500|NaN|14000|
|521|7597|HL9962|Android|3|Wilson|Farias|11/7/2018|Porto Alegre|3400|NaN|10200|
|522|7633|HL4379|Televisão|2|João|Alves|10/13/2018|Porto Alegre|2500|NaN|5000|
|523|7672|HL1918|iPhone|3|Sandy|Figueiredo|5/21/2018|Porto Alegre|5300|NaN|15900|
|524|7689|HL4379|Televisão|2|Julia|Teixeira|7/6/2018|Porto Alegre|2500|NaN|5000|
|525|7690|HL1918|iPhone|4|Maurício|Dias|6/21/2018|Porto Alegre|5300|NaN|21200|
|526|7732|HL1918|iPhone|2|Paloma|Sperandei|1/7/2018|Porto Alegre|5300|NaN|10600|
|527|7742|HL4379|Televisão|5|Fernanda|Rubim|2/21/2018|Porto Alegre|2500|NaN|12500|
|528|7750|HL8851|Notebook|4|Jessica|Ferreira|6/21/2018|Porto Alegre|3500|NaN|14000|
|529|7751|HL9962|Android|3|Vitor|Boccaletti|10/13/2018|Porto Alegre|3400|NaN|10200|
|530|7759|HL9962|Android|1|Livia|Codeceira|8/14/2018|Porto Alegre|3400|NaN|3400|
|531|7765|HL8851|Notebook|4|Beatriz|Li|1/22/2018|Porto Alegre|3500|NaN|14000|
|532|7768|HL2714|Tablet|5|Camille|Silva|4/5/2018|Porto Alegre|1600|NaN|8000|
|533|7769|HL4379|Televisão|3|Gabrielle|Costa|1/15/2018|Porto Alegre|2500|NaN|7500|
|534|7770|HL7348|SmartWatch|3|Matheus|Gomes|3/6/2018|Porto Alegre|1400|NaN|4200|
|535|7777|HL2714|Tablet|3|Carolina|Santos|4/24/2018|Porto Alegre|1600|NaN|4800|
|536|7783|HL1918|iPhone|5|Larissa|Jesus|6/30/2018|Porto Alegre|5300|NaN|26500|
|537|7791|HL9962|Android|1|Raphael|Mattos|6/27/2018|Porto Alegre|3400|NaN|3400|
|538|7792|HL7348|SmartWatch|2|João|Ribeiro|5/7/2018|Porto Alegre|1400|NaN|2800|
|539|7793|HL8851|Notebook|2|Ana|Gomes|9/12/2018|Porto Alegre|3500|NaN|7000|
|540|7809|HL1148|Câmera|5|Caroline|Aquino|3/14/2018|Porto Alegre|2100|NaN|10500|
|541|7812|HL1148|Câmera|4|Giovanna|Santos|7/17/2018|Porto Alegre|2100|NaN|8400|
|542|7827|HL2714|Tablet|3|José|Seixas|10/19/2018|Porto Alegre|1600|NaN|4800|
|543|7832|HL1918|iPhone|4|Matheus|Miranda|2/18/2018|Porto Alegre|5300|NaN|21200|
|544|7837|HL1918|iPhone|2|Douglas|Rodrigues|8/31/2018|Porto Alegre|5300|NaN|10600|
|545|7838|HL4379|Televisão|4|Rafaela|Gomes|6/24/2018|Porto Alegre|2500|NaN|10000|
|546|7845|HL9962|Android|3|Nina|Magalhães|2/5/2018|Porto Alegre|3400|NaN|10200|
|547|7867|HL8851|Notebook|3|Milena|Alcoforado|1/15/2018|Porto Alegre|3500|NaN|10500|
|548|7871|HL8851|Notebook|5|Barbara|Procaci|1/13/2018|Porto Alegre|3500|NaN|17500|
|549|7886|HL8851|Notebook|5|Raísa|Rodrigues|12/16/2018|Porto Alegre|3500|NaN|17500|
|550|7907|HL1918|iPhone|5|Bruno|Mota|12/12/2018|Porto Alegre|5300|NaN|26500|
|551|7917|HL8851|Notebook|4|Gabriel|Puntel|10/9/2018|Porto Alegre|3500|NaN|14000|
|552|7919|HL1148|Câmera|4|Marina|Correa|8/31/2018|Porto Alegre|2100|NaN|8400|
|553|7923|HL4379|Televisão|1|Luiza|Cabral|7/4/2018|Porto Alegre|2500|NaN|2500|
|554|7930|HL9962|Android|5|Karina|Camara|2/13/2018|Porto Alegre|3400|NaN|17000|
|555|7939|HL1148|Câmera|3|Marina|Correa|3/6/2018|Porto Alegre|2100|NaN|6300|
|556|7947|HL1918|iPhone|3|Daniel|Monteiro|3/9/2018|Porto Alegre|5300|NaN|15900|
|557|7980|HL1148|Câmera|1|Catarina|Teixeira|9/7/2018|Porto Alegre|2100|NaN|2100|
|558|7990|HL1918|iPhone|5|Raul|Silveira|2/18/2018|Porto Alegre|5300|NaN|26500|
|559|7996|HL8851|Notebook|2|David|Campelo|4/30/2018|Porto Alegre|3500|NaN|7000|
|560|8037|HL8851|Notebook|4|Helvio|Pedrosa|12/6/2018|Porto Alegre|3500|NaN|14000|
|561|8045|HL9962|Android|5|Pedro|Dalforne|11/22/2018|Porto Alegre|3400|NaN|17000|
|562|8089|HL1918|iPhone|2|Ana|Fioretti|12/18/2018|Porto Alegre|5300|NaN|10600|
|563|8097|HL4379|Televisão|2|Matheus|Gomes|4/26/2018|Porto Alegre|2500|NaN|5000|
|564|8101|HL8851|Notebook|1|Gustavo|Junior|3/29/2018|Porto Alegre|3500|NaN|3500|
|565|8106|HL4379|Televisão|4|Adrielle|Forte|4/22/2018|Porto Alegre|2500|NaN|10000|
|566|8107|HL4379|Televisão|2|Isabella|Scalabrin|10/11/2018|Porto Alegre|2500|NaN|5000|
|567|8123|HL1918|iPhone|1|Pedro|Martins|1/8/2018|Porto Alegre|5300|NaN|5300|
|568|8133|HL8851|Notebook|5|Pedro|Ronfini|12/31/2018|Porto Alegre|3500|NaN|17500|
|569|8137|HL7348|SmartWatch|2|Rodrigo|Alves|9/24/2018|Porto Alegre|1400|NaN|2800|
|570|8143|HL1148|Câmera|2|Andressa|Chou|12/1/2018|Porto Alegre|2100|NaN|4200|
|571|8156|HL7348|SmartWatch|4|Rafaela|Gonçalves|10/31/2018|Porto Alegre|1400|NaN|5600|
|572|8159|HL7348|SmartWatch|1|Lucas|Villanova|5/14/2018|Porto Alegre|1400|NaN|1400|
|573|8165|HL9962|Android|4|Carlos|Portela|9/10/2018|Porto Alegre|3400|NaN|13600|
|574|8174|HL4379|Televisão|2|Victor|Oliveira|7/26/2018|Porto Alegre|2500|NaN|5000|
|575|8208|HL8851|Notebook|2|Daniel|Sousa|8/6/2018|Porto Alegre|3500|NaN|7000|
|576|8210|HL8851|Notebook|4|Tayla|Lima|6/19/2018|Porto Alegre|3500|NaN|14000|
|577|8218|HL2714|Tablet|1|Fernanda|Bhering|2/10/2018|Porto Alegre|1600|NaN|1600|
|578|8219|HL1918|iPhone|4|Giulia|Lopes|9/10/2018|Porto Alegre|5300|NaN|21200|
|579|8246|HL1918|iPhone|5|Victor|Franco|7/1/2018|Porto Alegre|5300|NaN|26500|
|580|8249|HL7348|SmartWatch|4|Clara|Bruno|11/5/2018|Porto Alegre|1400|NaN|5600|
|581|8259|HL1918|iPhone|2|Lucas|Junior|5/7/2018|Porto Alegre|5300|NaN|10600|
|582|8280|HL9962|Android|1|Giuseppe|Bhering|8/13/2018|Porto Alegre|3400|NaN|3400|
|583|8282|HL1918|iPhone|2|Natália|Appel|4/30/2018|Porto Alegre|5300|NaN|10600|
|584|8287|HL8851|Notebook|3|Breno|Quinto|7/14/2018|Porto Alegre|3500|NaN|10500|
|585|8305|HL1918|iPhone|2|João|Guadagnino|1/8/2018|Porto Alegre|5300|NaN|10600|
|586|8318|HL1918|iPhone|5|Leandro|Ferreira|3/15/2018|Porto Alegre|5300|NaN|26500|
|587|8339|HL7348|SmartWatch|4|Bruno|Souza|1/5/2018|Porto Alegre|1400|NaN|5600|
|588|8348|HL4379|Televisão|3|Ana|Júnior|1/13/2018|Porto Alegre|2500|NaN|7500|
|589|8349|HL1918|iPhone|1|Maria|Junior|8/18/2018|Porto Alegre|5300|NaN|5300|
|590|8372|HL4379|Televisão|2|Caio|Moura|3/24/2018|Porto Alegre|2500|NaN|5000|
|591|8376|HL1918|iPhone|4|Barbara|Procaci|2/23/2018|Porto Alegre|5300|NaN|21200|
|592|8390|HL1918|iPhone|1|Gabriella|Sagrillo|4/26/2018|Porto Alegre|5300|NaN|5300|
|593|8391|HL7348|SmartWatch|4|Pedro|Cardoso|8/19/2018|Porto Alegre|1400|NaN|5600|
|594|8397|HL8851|Notebook|4|Gabrielle|Wanderley|10/13/2018|Porto Alegre|3500|NaN|14000|
|595|8413|HL1918|iPhone|1|Rafaela|Rodrigues|1/18/2018|Porto Alegre|5300|NaN|5300|
|596|8431|HL4379|Televisão|1|Luis|Villanova|7/23/2018|Porto Alegre|2500|NaN|2500|
|597|8458|HL4379|Televisão|3|Sandy|Figueiredo|4/9/2018|Porto Alegre|2500|NaN|7500|
|598|8477|HL9962|Android|1|Debora|Silva|8/13/2018|Porto Alegre|3400|NaN|3400|
|599|8483|HL1148|Câmera|2|Arthur|Souza|1/26/2018|Porto Alegre|2100|NaN|4200|
|600|8485|HL1918|iPhone|4|Viviane|Souza|6/28/2018|Porto Alegre|5300|NaN|21200|
|601|8510|HL1148|Câmera|3|Victor|Lira|3/4/2018|Porto Alegre|2100|NaN|6300|
|602|8518|HL1918|iPhone|1|Laura|Araujo|4/1/2018|Porto Alegre|5300|NaN|5300|
|603|8534|HL8851|Notebook|5|Marina|Correa|9/28/2018|Porto Alegre|3500|NaN|17500|
|604|8546|HL1918|iPhone|1|Ravena|Bhering|11/9/2018|Porto Alegre|5300|NaN|5300|
|605|8551|HL4379|Televisão|2|Joao|Pereira|2/9/2018|Porto Alegre|2500|NaN|5000|
|606|8554|HL1148|Câmera|3|Sarah|Souza|9/15/2018|Porto Alegre|2100|NaN|6300|
|607|8567|HL7348|SmartWatch|4|Isabela|Rodrigues|11/8/2018|Porto Alegre|1400|NaN|5600|
|608|8576|HL4379|Televisão|4|Rafaela|Gonçalves|7/10/2018|Porto Alegre|2500|NaN|10000|
|609|8578|HL4379|Televisão|1|Gabriela|Mello|11/4/2018|Porto Alegre|2500|NaN|2500|
|610|8610|HL4379|Televisão|4|Jorge|Fonseca|12/9/2018|Porto Alegre|2500|NaN|10000|
|611|8615|HL8851|Notebook|5|Giulia|Lopes|7/3/2018|Porto Alegre|3500|NaN|17500|
|612|8621|HL8851|Notebook|2|Mariana|Baptista|3/27/2018|Porto Alegre|3500|NaN|7000|
|613|8653|HL1918|iPhone|2|Carlos|Galvão|11/16/2018|Porto Alegre|5300|NaN|10600|
|614|8656|HL4379|Televisão|5|Lázaro|Villanova|10/26/2018|Porto Alegre|2500|NaN|12500|
|615|8665|HL1918|iPhone|2|Ramon|Araujo|4/9/2018|Porto Alegre|5300|NaN|10600|
|616|8679|HL4379|Televisão|5|Guilherme|Merotto|1/16/2018|Porto Alegre|2500|NaN|12500|
|617|8704|HL7348|SmartWatch|4|Matheus|Santos|3/31/2018|Porto Alegre|1400|NaN|5600|
|618|8707|HL4379|Televisão|4|Lucas|Reis|10/25/2018|Porto Alegre|2500|NaN|10000|
|619|8710|HL1918|iPhone|1|Matheus|Souza|12/5/2018|Porto Alegre|5300|NaN|5300|
|620|8713|HL2714|Tablet|4|Rebeca|Taylor|4/20/2018|Porto Alegre|1600|NaN|6400|
|621|8743|HL9962|Android|2|Pedro|Delgado|9/7/2018|Porto Alegre|3400|NaN|6800|
|622|8787|HL8851|Notebook|4|Bianca|Ferezin|1/18/2018|Porto Alegre|3500|NaN|14000|
|623|8793|HL1148|Câmera|3|Pedro|Conceição|4/16/2018|Porto Alegre|2100|NaN|6300|
|624|8823|HL4379|Televisão|5|Anna|Silva|12/8/2018|Porto Alegre|2500|NaN|12500|
|625|8838|HL1148|Câmera|5|Iuri|Neto|3/12/2018|Porto Alegre|2100|NaN|10500|
|626|8849|HL2714|Tablet|1|Tadeu|Sousa|10/15/2018|Porto Alegre|1600|NaN|1600|
|627|8861|HL1148|Câmera|1|Alexandre|Dantas|12/3/2018|Porto Alegre|2100|NaN|2100|
|628|8878|HL1918|iPhone|2|Jônatas|Soares|2/23/2018|Porto Alegre|5300|NaN|10600|
|629|8880|HL8851|Notebook|4|Jackson|Derossi|9/13/2018|Porto Alegre|3500|NaN|14000|
|630|8886|HL4379|Televisão|2|Luiz|Mendonça|9/3/2018|Porto Alegre|2500|NaN|5000|
|631|8890|HL7348|SmartWatch|3|Isabel|Leite|7/17/2018|Porto Alegre|1400|NaN|4200|
|632|8900|HL1918|iPhone|2|Henrique|Oliveira|6/2/2018|Porto Alegre|5300|NaN|10600|
|633|8902|HL2714|Tablet|3|Victor|Firmino|4/19/2018|Porto Alegre|1600|NaN|4800|
|634|8936|HL7348|SmartWatch|1|Igor|Azevedo|9/21/2018|Porto Alegre|1400|NaN|1400|
|635|8943|HL1918|iPhone|5|Manuela|Ferreira|6/15/2018|Porto Alegre|5300|NaN|26500|
|636|8948|HL1918|iPhone|3|Cícero|Ramos|12/6/2018|Porto Alegre|5300|NaN|15900|
|637|8961|HL4379|Televisão|1|Marina|Aragão|5/28/2018|Porto Alegre|2500|NaN|2500|
|638|8975|HL1918|iPhone|4|Bianca|Paz|10/9/2018|Porto Alegre|5300|NaN|21200|
|639|8988|HL7348|SmartWatch|5|Sandy|Figueiredo|3/26/2018|Porto Alegre|1400|NaN|7000|
|640|8995|HL1918|iPhone|3|Clara|Bruno|2/28/2018|Porto Alegre|5300|NaN|15900|
|641|9014|HL4379|Televisão|2|Joao|Pereira|12/14/2018|Porto Alegre|2500|NaN|5000|
|642|9037|HL1918|iPhone|4|Bernard|Pedrosa|12/27/2018|Porto Alegre|5300|NaN|21200|
|643|9039|HL1918|iPhone|5|Lunna|Vannier|3/31/2018|Porto Alegre|5300|NaN|26500|
|644|9040|HL1918|iPhone|3|Gustavo|Erthal|9/2/2018|Porto Alegre|5300|NaN|15900|
|645|9043|HL7348|SmartWatch|4|Pedro|Macckione|9/13/2018|Porto Alegre|1400|NaN|5600|
|646|9071|HL8851|Notebook|1|Thales|Portillo|10/6/2018|Porto Alegre|3500|NaN|3500|
|647|9087|HL8851|Notebook|4|Gabriel|Assis|5/23/2018|Porto Alegre|3500|NaN|14000|
|648|9096|HL7348|SmartWatch|3|Lucas|Villanova|11/26/2018|Porto Alegre|1400|NaN|4200|
|649|9102|HL9962|Android|3|Gabriela|Mello|12/3/2018|Porto Alegre|3400|NaN|10200|
|650|9117|HL1918|iPhone|3|Juliana|Barreira|4/8/2018|Porto Alegre|5300|NaN|15900|
|651|9154|HL8851|Notebook|3|Nathan|Morelli|2/20/2018|Porto Alegre|3500|NaN|10500|
|652|9155|HL8851|Notebook|3|Patrick|Silva|1/18/2018|Porto Alegre|3500|NaN|10500|
|653|9162|HL1148|Câmera|3|Michelle|Pereira|5/24/2018|Porto Alegre|2100|NaN|6300|
|654|9180|HL1918|iPhone|4|Fernanda|Rubim|6/24/2018|Porto Alegre|5300|NaN|21200|
|655|9185|HL1918|iPhone|3|Fernanda|Silva|5/24/2018|Porto Alegre|5300|NaN|15900|
|656|9224|HL1918|iPhone|2|Myllena|Corrêa|1/16/2018|Porto Alegre|5300|NaN|10600|
|657|9233|HL8851|Notebook|2|Marcelo|Pereira|12/4/2018|Porto Alegre|3500|NaN|7000|
|658|9245|HL4379|Televisão|3|Camilla|Cardeman|3/2/2018|Porto Alegre|2500|NaN|7500|
|659|9249|HL2714|Tablet|2|Izabel|Lopes|5/12/2018|Porto Alegre|1600|NaN|3200|
|660|9255|HL9962|Android|4|Alon|Palmeira|2/23/2018|Porto Alegre|3400|NaN|13600|
|661|9271|HL1918|iPhone|2|Marina|Perdomo|5/31/2018|Porto Alegre|5300|NaN|10600|
|662|9277|HL7348|SmartWatch|2|Gabriel|Brito|5/30/2018|Porto Alegre|1400|NaN|2800|
|663|9299|HL7348|SmartWatch|5|Carolina|Motta|8/27/2018|Porto Alegre|1400|NaN|7000|
|664|9316|HL1918|iPhone|4|Rubens|Valente|3/28/2018|Porto Alegre|5300|NaN|21200|
|665|9349|HL7348|SmartWatch|2|Carolina|Motta|5/24/2018|Porto Alegre|1400|NaN|2800|
|666|9358|HL9962|Android|1|Matheus|Delgado|3/16/2018|Porto Alegre|3400|NaN|3400|
|667|9369|HL1918|iPhone|5|Adrielle|Vieira|12/15/2018|Porto Alegre|5300|NaN|26500|
|668|9376|HL1918|iPhone|5|Amanda|Felippe|10/5/2018|Porto Alegre|5300|NaN|26500|
|669|9392|HL1918|iPhone|5|Jeferson|Costa|1/15/2018|Porto Alegre|5300|NaN|26500|
|670|9405|HL8851|Notebook|4|Camila|Bastazini|3/23/2018|Porto Alegre|3500|NaN|14000|
|671|9406|HL1918|iPhone|1|Paula|Isbelle|6/7/2018|Porto Alegre|5300|NaN|5300|
|672|9426|HL4379|Televisão|2|Livia|Codeceira|7/25/2018|Porto Alegre|2500|NaN|5000|
|673|9447|HL8851|Notebook|2|Vitor|Arruda|1/7/2018|Porto Alegre|3500|NaN|7000|
|674|9450|HL9962|Android|2|Julie|Ferreira|10/8/2018|Porto Alegre|3400|NaN|6800|
|675|9451|HL9962|Android|5|Carolina|Motta|8/22/2018|Porto Alegre|3400|NaN|17000|
|676|9472|HL4379|Televisão|1|Daniel|Cardoso|10/5/2018|Porto Alegre|2500|NaN|2500|
|677|9480|HL1148|Câmera|1|Rodrigo|Bruno|5/14/2018|Porto Alegre|2100|NaN|2100|
|678|9524|HL1918|iPhone|5|Joao|Pereira|1/30/2018|Porto Alegre|5300|NaN|26500|
|679|9530|HL1918|iPhone|5|Stefan|Santos|10/10/2018|Porto Alegre|5300|NaN|26500|
|680|9622|HL1918|iPhone|4|Bernardo|Botelho|10/26/2018|Porto Alegre|5300|NaN|21200|
|681|9624|HL1148|Câmera|3|Luis|Villanova|6/22/2018|Porto Alegre|2100|NaN|6300|
|682|9642|HL8851|Notebook|2|Breno|Farias|11/17/2018|Porto Alegre|3500|NaN|7000|
|683|9662|HL2714|Tablet|5|Stephanie|Novak|1/26/2018|Porto Alegre|1600|NaN|8000|
|684|9693|HL4379|Televisão|2|Letícia|Araujo|6/23/2018|Porto Alegre|2500|NaN|5000|
|685|9695|HL8851|Notebook|2|Maria|Mello|7/4/2018|Porto Alegre|3500|NaN|7000|
|686|9710|HL4379|Televisão|1|Diego|Rodrigues|12/2/2018|Porto Alegre|2500|NaN|2500|
|687|9715|HL1148|Câmera|1|João|Guadagnino|7/16/2018|Porto Alegre|2100|NaN|2100|
|688|9770|HL4379|Televisão|2|Fabio|Sepúlveda|1/15/2018|Porto Alegre|2500|NaN|5000|
|689|9780|HL1918|iPhone|1|Thiago|Veloso|5/4/2018|Porto Alegre|5300|NaN|5300|
|690|9794|HL4379|Televisão|5|João|Guadagnino|2/1/2018|Porto Alegre|2500|NaN|12500|
|691|9819|HL1918|iPhone|2|Brenno|Santos|10/18/2018|Porto Alegre|5300|NaN|10600|
|692|9822|HL1918|iPhone|3|Paula|Cavalcanti|2/14/2018|Porto Alegre|5300|NaN|15900|
|693|9825|HL1918|iPhone|1|Marcos|Nucci|7/24/2018|Porto Alegre|5300|NaN|5300|
|694|9857|HL1148|Câmera|2|Allan|Guedes|8/20/2018|Porto Alegre|2100|NaN|4200|
|695|9866|HL1148|Câmera|2|Paula|Isbelle|6/20/2018|Porto Alegre|2100|NaN|4200|
|696|9880|HL8851|Notebook|5|Pedro|Santana|2/6/2018|Porto Alegre|3500|NaN|17500|
|697|9895|HL8851|Notebook|2|Caio|Ferreira|5/11/2018|Porto Alegre|3500|NaN|7000|
|698|9945|HL1918|iPhone|5|Pedro|Cardoso|12/31/2018|Porto Alegre|5300|NaN|26500|
|699|9947|HL1918|iPhone|2|Gabrielle|Vasconcelos|2/20/2018|Porto Alegre|5300|NaN|10600|
|700|9980|HL1918|iPhone|5|João|Rodrigues|1/21/2018|Porto Alegre|5300|NaN|26500|
|701|9983|HL2714|Tablet|5|Bianca|Tatsch|2/12/2018|Porto Alegre|1600|NaN|8000|
|702|9993|HL1148|Câmera|4|Victor|Lira|7/26/2018|Porto Alegre|2100|NaN|8400|
|703|9997|HL1918|iPhone|4|Norman|Jimbo|6/13/2018|Porto Alegre|5300|NaN|21200|
|0|40|HL1148|Câmera|2|Gabriel|Almeida|11/16/2018|Salvador|2100|NaN|4200|
|1|42|HL2714|Tablet|5|Rodrigo|Alves|2/27/2018|Salvador|1600|NaN|8000|
|2|51|HL1918|iPhone|4|Ulisses|Arruda|5/5/2018|Salvador|5300|NaN|21200|
|3|70|HL9962|Android|3|Raissa|Negrelli|3/10/2018|Salvador|3400|NaN|10200|
|4|94|HL1918|iPhone|2|Breno|Caputo|3/30/2018|Salvador|5300|NaN|10600|
|5|101|HL1918|iPhone|4|Victor|Soares|4/10/2018|Salvador|5300|NaN|21200|
|6|110|HL4379|Televisão|2|Pedro|Rodrigues|4/16/2018|Salvador|2500|NaN|5000|
|7|119|HL9962|Android|3|Wilson|Meirelles|6/8/2018|Salvador|3400|NaN|10200|
|8|128|HL9962|Android|5|Diego|Marchesi|11/27/2018|Salvador|3400|NaN|17000|
|9|129|HL4379|Televisão|5|Bruno|Ursulino|8/2/2018|Salvador|2500|NaN|12500|
|10|150|HL2714|Tablet|4|Kimberly|Sad|5/10/2018|Salvador|1600|NaN|6400|
|11|152|HL1148|Câmera|1|Marina|Marins|1/23/2018|Salvador|2100|NaN|2100|
|12|172|HL7348|SmartWatch|1|Luiza|Farias|7/30/2018|Salvador|1400|NaN|1400|
|13|177|HL4379|Televisão|1|Arthur|Souza|6/18/2018|Salvador|2500|NaN|2500|
|14|180|HL9962|Android|2|Catarina|Teixeira|5/5/2018|Salvador|3400|NaN|6800|
|15|196|HL9962|Android|2|João|Júnior|5/23/2018|Salvador|3400|NaN|6800|
|16|202|HL2714|Tablet|1|Rafaela|Gonçalves|2/1/2018|Salvador|1600|NaN|1600|
|17|210|HL1918|iPhone|4|Matheus|Delgado|3/11/2018|Salvador|5300|NaN|21200|
|18|215|HL2714|Tablet|2|Carlos|Silva|5/1/2018|Salvador|1600|NaN|3200|
|19|216|HL1918|iPhone|2|Matheus|Figueiredo|6/12/2018|Salvador|5300|NaN|10600|
|20|239|HL9962|Android|5|Vinícius|Antunes|1/16/2018|Salvador|3400|NaN|17000|
|21|244|HL9962|Android|4|Thomáz|Bôas|2/2/2018|Salvador|3400|NaN|13600|
|22|248|HL8851|Notebook|2|Isabela|Resende|8/27/2018|Salvador|3500|NaN|7000|
|23|253|HL1918|iPhone|1|Bárbara|Cavalcante|3/1/2018|Salvador|5300|NaN|5300|
|24|254|HL1148|Câmera|4|Breno|Costa|11/17/2018|Salvador|2100|NaN|8400|
|25|255|HL4379|Televisão|5|Sthefeson|Barroso|2/19/2018|Salvador|2500|NaN|12500|
|26|256|HL1918|iPhone|1|Carlos|Azevedo|8/8/2018|Salvador|5300|NaN|5300|
|27|261|HL2714|Tablet|1|Bernardo|Borges|8/12/2018|Salvador|1600|NaN|1600|
|28|270|HL8851|Notebook|5|Matheus|Afonso|2/14/2018|Salvador|3500|NaN|17500|
|29|271|HL1918|iPhone|4|Rafael|Ramos|2/28/2018|Salvador|5300|NaN|21200|
|30|272|HL4379|Televisão|3|Guilherme|Monteiro|10/29/2018|Salvador|2500|NaN|7500|
|31|283|HL7348|SmartWatch|5|Leandro|Rodrigues|9/24/2018|Salvador|1400|NaN|7000|
|32|287|HL8851|Notebook|5|Isabela|Resende|7/4/2018|Salvador|3500|NaN|17500|
|33|289|HL1918|iPhone|4|Raissa|Sales|7/17/2018|Salvador|5300|NaN|21200|
|34|300|HL1918|iPhone|4|Hanna|Fonseca|10/26/2018|Salvador|5300|NaN|21200|
|35|335|HL1148|Câmera|5|Mateus|Franco|10/17/2018|Salvador|2100|NaN|10500|
|36|341|HL1148|Câmera|4|Juliana|Barreira|8/1/2018|Salvador|2100|NaN|8400|
|37|347|HL1918|iPhone|5|Caio|Affonso|3/24/2018|Salvador|5300|NaN|26500|
|38|350|HL1148|Câmera|4|Gabriel|Soares|11/7/2018|Salvador|2100|NaN|8400|
|39|357|HL1918|iPhone|5|Milena|Alcoforado|3/19/2018|Salvador|5300|NaN|26500|
|40|366|HL1918|iPhone|3|Juliana|Mesquita|12/28/2018|Salvador|5300|NaN|15900|
|41|372|HL1148|Câmera|5|Beatriz|Perdomo|9/1/2018|Salvador|2100|NaN|10500|
|42|376|HL9962|Android|1|Andre|Nóbrega|3/7/2018|Salvador|3400|NaN|3400|
|43|377|HL4379|Televisão|3|Adrielle|Gabriel|9/8/2018|Salvador|2500|NaN|7500|
|44|392|HL9962|Android|1|Lívia|Marques|5/26/2018|Salvador|3400|NaN|3400|
|45|407|HL8851|Notebook|3|Fabio|Sepúlveda|3/12/2018|Salvador|3500|NaN|10500|
|46|409|HL7348|SmartWatch|2|Bianca|Allevato|3/20/2018|Salvador|1400|NaN|2800|
|47|410|HL7348|SmartWatch|4|Bruno|Oliveira|3/2/2018|Salvador|1400|NaN|5600|
|48|419|HL1918|iPhone|3|Bruna|Silveira|1/5/2018|Salvador|5300|NaN|15900|
|49|423|HL4379|Televisão|1|João|Rodrigues|5/28/2018|Salvador|2500|NaN|2500|
|50|429|HL8851|Notebook|3|Caio|Vianna|7/21/2018|Salvador|3500|NaN|10500|
|51|438|HL8851|Notebook|5|Diego|Mello|4/2/2018|Salvador|3500|NaN|17500|
|52|439|HL1148|Câmera|2|Hygor|Essaber|5/27/2018|Salvador|2100|NaN|4200|
|53|442|HL1918|iPhone|4|Pedro|Costa|5/21/2018|Salvador|5300|NaN|21200|
|54|445|HL1918|iPhone|2|Lucas|Fontoura|8/31/2018|Salvador|5300|NaN|10600|
|55|454|HL1918|iPhone|5|Ana|Felippe|7/22/2018|Salvador|5300|NaN|26500|
|56|457|HL7348|SmartWatch|1|Letícia|Rodrigues|1/16/2018|Salvador|1400|NaN|1400|
|57|460|HL7348|SmartWatch|2|Daniel|Nauenberg|5/3/2018|Salvador|1400|NaN|2800|
|58|461|HL4379|Televisão|1|Rilson|Guedes|2/16/2018|Salvador|2500|NaN|2500|
|59|463|HL4379|Televisão|2|Lucas|Costa|6/28/2018|Salvador|2500|NaN|5000|
|60|474|HL1918|iPhone|1|Rodrigo|Souza|10/2/2018|Salvador|5300|NaN|5300|
|61|476|HL1148|Câmera|3|Luiza|Johnson|4/21/2018|Salvador|2100|NaN|6300|
|62|478|HL1148|Câmera|1|Julie|Ferreira|12/19/2018|Salvador|2100|NaN|2100|
|63|480|HL4379|Televisão|3|Luíza|Goulart|9/6/2018|Salvador|2500|NaN|7500|
|64|494|HL4379|Televisão|2|Michelle|Pereira|2/10/2018|Salvador|2500|NaN|5000|
|65|502|HL4379|Televisão|1|Joyce|Medina|10/24/2018|Salvador|2500|NaN|2500|
|66|510|HL4379|Televisão|1|Gustavo|Guimarães|12/11/2018|Salvador|2500|NaN|2500|
|67|521|HL9962|Android|2|Fabio|Boccaletti|10/24/2018|Salvador|3400|NaN|6800|
|68|522|HL1918|iPhone|1|Bruno|Oliveira|3/26/2018|Salvador|5300|NaN|5300|
|69|524|HL1148|Câmera|4|Yasser|Calbucci|7/27/2018|Salvador|2100|NaN|8400|
|70|526|HL1918|iPhone|1|Debora|Silva|4/20/2018|Salvador|5300|NaN|5300|
|71|542|HL9962|Android|2|Joyce|Medina|3/3/2018|Salvador|3400|NaN|6800|
|72|559|HL8851|Notebook|2|Lucas|Freitas|3/1/2018|Salvador|3500|NaN|7000|
|73|568|HL1148|Câmera|1|Juliana|Goes|8/8/2018|Salvador|2100|NaN|2100|
|74|570|HL2714|Tablet|4|Fabio|Ramos|5/27/2018|Salvador|1600|NaN|6400|
|75|575|HL8851|Notebook|4|Anna|Silva|6/26/2018|Salvador|3500|NaN|14000|
|76|576|HL8851|Notebook|4|Paulo|Campos|6/19/2018|Salvador|3500|NaN|14000|
|77|578|HL1918|iPhone|1|Diogo|Ressurreição|6/27/2018|Salvador|5300|NaN|5300|
|78|579|HL9962|Android|2|Anderson|Cavalcanti|12/2/2018|Salvador|3400|NaN|6800|
|79|583|HL1918|iPhone|1|Mariana|Sousa|5/7/2018|Salvador|5300|NaN|5300|
|80|592|HL8851|Notebook|3|Isabela|Rodrigues|1/23/2018|Salvador|3500|NaN|10500|
|81|593|HL8851|Notebook|4|Mariane|Ferreira|9/14/2018|Salvador|3500|NaN|14000|
|82|598|HL4379|Televisão|1|Diego|Marchesi|8/3/2018|Salvador|2500|NaN|2500|
|83|614|HL1918|iPhone|4|Isabella|Rodrigues|5/5/2018|Salvador|5300|NaN|21200|
|84|616|HL9962|Android|3|Luiz|Campista|3/1/2018|Salvador|3400|NaN|10200|
|85|618|HL1148|Câmera|2|Raul|Silveira|3/25/2018|Salvador|2100|NaN|4200|
|86|630|HL9962|Android|2|João|Luz|3/18/2018|Salvador|3400|NaN|6800|
|87|631|HL4379|Televisão|5|Danilo|Mendonça|5/21/2018|Salvador|2500|NaN|12500|
|88|632|HL4379|Televisão|1|Adrielle|Vieira|10/7/2018|Salvador|2500|NaN|2500|
|89|648|HL1148|Câmera|3|Caroline|Delgado|11/21/2018|Salvador|2100|NaN|6300|
|90|657|HL7348|SmartWatch|4|Antonio|Manhães|9/20/2018|Salvador|1400|NaN|5600|
|91|662|HL1918|iPhone|1|Henrique|Oliveira|8/19/2018|Salvador|5300|NaN|5300|
|92|679|HL1918|iPhone|4|Rafaela|Ferreira|8/18/2018|Salvador|5300|NaN|21200|
|93|683|HL9962|Android|2|Pedro|Santos|9/5/2018|Salvador|3400|NaN|6800|
|94|685|HL2714|Tablet|2|Bernardo|Botelho|5/17/2018|Salvador|1600|NaN|3200|
|95|699|HL4379|Televisão|4|Maria|Correa|3/25/2018|Salvador|2500|NaN|10000|
|96|704|HL4379|Televisão|5|Lucas|Wanderley|11/26/2018|Salvador|2500|NaN|12500|
|97|705|HL8851|Notebook|2|Milena|Almeida|9/30/2018|Salvador|3500|NaN|7000|
|98|713|HL7348|SmartWatch|2|Bianca|Tatsch|9/25/2018|Salvador|1400|NaN|2800|
|99|723|HL1918|iPhone|2|Guilherme|Lima|6/2/2018|Salvador|5300|NaN|10600|
|100|731|HL7348|SmartWatch|4|Matheus|Figueiredo|4/7/2018|Salvador|1400|NaN|5600|
|101|743|HL2714|Tablet|4|Matheus|Silva|1/14/2018|Salvador|1600|NaN|6400|
|102|751|HL8851|Notebook|1|Carolina|Rocha|1/15/2018|Salvador|3500|NaN|3500|
|103|759|HL4379|Televisão|1|Guilherme|Lima|9/13/2018|Salvador|2500|NaN|2500|
|104|766|HL4379|Televisão|1|Daniel|Araujo|7/20/2018|Salvador|2500|NaN|2500|
|105|768|HL7348|SmartWatch|1|Paula|Calbucci|8/28/2018|Salvador|1400|NaN|1400|
|106|775|HL8851|Notebook|1|Rafaela|Feio|3/17/2018|Salvador|3500|NaN|3500|
|107|781|HL4379|Televisão|5|Michelle|Miura|2/26/2018|Salvador|2500|NaN|12500|
|108|787|HL4379|Televisão|3|Ana|Carvalho|4/24/2018|Salvador|2500|NaN|7500|
|109|792|HL1148|Câmera|2|João|Castilho|12/4/2018|Salvador|2100|NaN|4200|
|110|793|HL7348|SmartWatch|1|Erick|Soares|7/15/2018|Salvador|1400|NaN|1400|
|111|801|HL1918|iPhone|1|Stephanie|Novak|11/7/2018|Salvador|5300|NaN|5300|
|112|806|HL2714|Tablet|5|Mateus|Polastri|1/13/2018|Salvador|1600|NaN|8000|
|113|809|HL9962|Android|4|Marcela|Medeiros|4/8/2018|Salvador|3400|NaN|13600|
|114|820|HL1148|Câmera|4|Pedro|Oliveira|3/10/2018|Salvador|2100|NaN|8400|
|115|833|HL4379|Televisão|2|Ana|Felippe|5/19/2018|Salvador|2500|NaN|5000|
|116|847|HL1918|iPhone|2|Beatriz|Almeida|4/15/2018|Salvador|5300|NaN|10600|
|117|852|HL1148|Câmera|4|Aline|Andrade|4/20/2018|Salvador|2100|NaN|8400|
|118|862|HL2714|Tablet|5|Thayna|Martins|4/27/2018|Salvador|1600|NaN|8000|
|119|864|HL4379|Televisão|3|Ana|Gonzaga|1/12/2018|Salvador|2500|NaN|7500|
|120|876|HL4379|Televisão|3|Gabriel|Almeida|12/1/2018|Salvador|2500|NaN|7500|
|121|888|HL4379|Televisão|5|Fabio|Ramos|1/23/2018|Salvador|2500|NaN|12500|
|122|890|HL9962|Android|3|Henrique|Oliveira|7/28/2018|Salvador|3400|NaN|10200|
|123|905|HL4379|Televisão|2|Cassio|Faria|1/6/2018|Salvador|2500|NaN|5000|
|124|906|HL1918|iPhone|3|Breno|Caputo|6/15/2018|Salvador|5300|NaN|15900|
|125|937|HL2714|Tablet|3|Jeferson|Sone|2/18/2018|Salvador|1600|NaN|4800|
|126|947|HL1918|iPhone|5|Fernanda|Figueiredo|5/26/2018|Salvador|5300|NaN|26500|
|127|957|HL8851|Notebook|3|Marina|Gama|8/30/2018|Salvador|3500|NaN|10500|
|128|960|HL8851|Notebook|5|Daniel|Nauenberg|8/24/2018|Salvador|3500|NaN|17500|
|129|965|HL7348|SmartWatch|4|Luiz|Marinho|9/15/2018|Salvador|1400|NaN|5600|
|130|981|HL9962|Android|1|Helena|Chafin|11/2/2018|Salvador|3400|NaN|3400|
|131|990|HL9962|Android|5|Laura|Araujo|2/13/2018|Salvador|3400|NaN|17000|
|132|1001|HL1918|iPhone|3|Vitor|Campos|4/24/2018|Salvador|5300|NaN|15900|
|133|1004|HL9962|Android|3|Juliana|Mesquita|3/23/2018|Salvador|3400|NaN|10200|
|134|1009|HL8851|Notebook|1|Raissa|Maia|1/24/2018|Salvador|3500|NaN|3500|
|135|1014|HL1918|iPhone|2|Thomaz|Ferreira|5/3/2018|Salvador|5300|NaN|10600|
|136|1018|HL1918|iPhone|5|Hiaiune|Valim|7/6/2018|Salvador|5300|NaN|26500|
|137|1023|HL1918|iPhone|1|Lucas|Fontoura|4/26/2018|Salvador|5300|NaN|5300|
|138|1037|HL7348|SmartWatch|3|Wilson|Vianna|7/14/2018|Salvador|1400|NaN|4200|
|139|1053|HL9962|Android|3|Sthefeson|Kohn|3/31/2018|Salvador|3400|NaN|10200|
|140|1054|HL2714|Tablet|5|Bianca|Piero|10/15/2018|Salvador|1600|NaN|8000|
|141|1056|HL7348|SmartWatch|4|Myllena|Carneiro|5/14/2018|Salvador|1400|NaN|5600|
|142|1057|HL1918|iPhone|2|Stefan|Santos|1/19/2018|Salvador|5300|NaN|10600|
|143|1063|HL1918|iPhone|1|Larissa|Vasconcellos|7/7/2018|Salvador|5300|NaN|5300|
|144|1066|HL2714|Tablet|3|Diego|Barros|5/18/2018|Salvador|1600|NaN|4800|
|145|1076|HL4379|Televisão|5|Karina|Camara|12/26/2018|Salvador|2500|NaN|12500|
|146|1081|HL8851|Notebook|1|Stefan|Santos|12/4/2018|Salvador|3500|NaN|3500|
|147|1084|HL1918|iPhone|2|Matheus|Santos|6/24/2018|Salvador|5300|NaN|10600|
|148|1088|HL4379|Televisão|2|Carolina|Brum|3/1/2018|Salvador|2500|NaN|5000|
|149|1094|HL1148|Câmera|2|Guilherme|Jordao|3/7/2018|Salvador|2100|NaN|4200|
|150|1102|HL8851|Notebook|5|Michelle|Pereira|3/17/2018|Salvador|3500|NaN|17500|
|151|1117|HL7348|SmartWatch|2|Juliana|Guimarães|8/10/2018|Salvador|1400|NaN|2800|
|152|1122|HL1148|Câmera|5|Bernardo|Ribeiro|2/14/2018|Salvador|2100|NaN|10500|
|153|1123|HL1918|iPhone|3|David|Campelo|3/26/2018|Salvador|5300|NaN|15900|
|154|1125|HL1918|iPhone|5|Victor|Magalhães|10/26/2018|Salvador|5300|NaN|26500|
|155|1139|HL4379|Televisão|3|Luíza|Goulart|6/30/2018|Salvador|2500|NaN|7500|
|156|1146|HL4379|Televisão|2|Caio|Vianna|10/21/2018|Salvador|2500|NaN|5000|
|157|1148|HL9962|Android|4|Felipe|Paulo|11/16/2018|Salvador|3400|NaN|13600|
|158|1152|HL2714|Tablet|5|Daniel|Alcoforado|12/19/2018|Salvador|1600|NaN|8000|
|159|1159|HL7348|SmartWatch|3|Julie|Ferreira|12/6/2018|Salvador|1400|NaN|4200|
|160|1183|HL7348|SmartWatch|4|Fernanda|Rubim|9/6/2018|Salvador|1400|NaN|5600|
|161|1194|HL2714|Tablet|3|Luis|Garcia|9/27/2018|Salvador|1600|NaN|4800|
|162|1206|HL9962|Android|1|Isabela|Chagas|11/9/2018|Salvador|3400|NaN|3400|
|163|1219|HL9962|Android|2|Daniel|Ortiz|5/28/2018|Salvador|3400|NaN|6800|
|164|1222|HL1918|iPhone|5|Cícero|Lima|11/27/2018|Salvador|5300|NaN|26500|
|165|1227|HL4379|Televisão|3|Carlos|Galvão|1/16/2018|Salvador|2500|NaN|7500|
|166|1245|HL8851|Notebook|2|Carolina|Figueiredo|2/18/2018|Salvador|3500|NaN|7000|
|167|1247|HL9962|Android|5|Lucas|Costa|5/26/2018|Salvador|3400|NaN|17000|
|168|1252|HL2714|Tablet|3|Marcelo|Rosa|10/8/2018|Salvador|1600|NaN|4800|
|169|1257|HL1918|iPhone|4|Bruna|Brandao|4/13/2018|Salvador|5300|NaN|21200|
|170|1262|HL1148|Câmera|2|João|Bach|1/1/2018|Salvador|2100|NaN|4200|
|171|1265|HL7348|SmartWatch|2|Fabio|Sepúlveda|4/8/2018|Salvador|1400|NaN|2800|
|172|1274|HL4379|Televisão|5|Vanessa|Bach|7/16/2018|Salvador|2500|NaN|12500|
|173|1287|HL2714|Tablet|1|Matheus|Afonso|5/21/2018|Salvador|1600|NaN|1600|
|174|1292|HL9962|Android|4|Barbara|Procaci|6/10/2018|Salvador|3400|NaN|13600|
|175|1298|HL1148|Câmera|5|Bianca|Piero|6/24/2018|Salvador|2100|NaN|10500|
|176|1306|HL1918|iPhone|5|Eduardo|Peluzo|9/20/2018|Salvador|5300|NaN|26500|
|177|1307|HL1918|iPhone|2|Wilson|Meirelles|9/25/2018|Salvador|5300|NaN|10600|
|178|1326|HL1918|iPhone|2|Natália|Appel|11/28/2018|Salvador|5300|NaN|10600|
|179|1337|HL1918|iPhone|4|Itai|Puntel|11/10/2018|Salvador|5300|NaN|21200|
|180|1344|HL8851|Notebook|5|Anna|Figueiredo|4/28/2018|Salvador|3500|NaN|17500|
|181|1346|HL8851|Notebook|3|Brenno|Miranda|6/11/2018|Salvador|3500|NaN|10500|
|182|1357|HL7348|SmartWatch|4|Renan|Melo|5/29/2018|Salvador|1400|NaN|5600|
|183|1368|HL4379|Televisão|3|Bernardo|Souza|6/15/2018|Salvador|2500|NaN|7500|
|184|1369|HL1918|iPhone|5|Andressa|Chou|9/9/2018|Salvador|5300|NaN|26500|
|185|1373|HL1148|Câmera|5|William|Mendonça|7/6/2018|Salvador|2100|NaN|10500|
|186|1377|HL1148|Câmera|5|Beatriz|Cavalcanti|11/16/2018|Salvador|2100|NaN|10500|
|187|1388|HL1918|iPhone|5|William|Mendonça|8/11/2018|Salvador|5300|NaN|26500|
|188|1397|HL7348|SmartWatch|4|João|Ribeiro|12/10/2018|Salvador|1400|NaN|5600|
|189|1399|HL1918|iPhone|1|Lucas|Machado|10/16/2018|Salvador|5300|NaN|5300|
|190|1417|HL1148|Câmera|4|Luã|Sá|9/25/2018|Salvador|2100|NaN|8400|
|191|1422|HL1918|iPhone|4|Matheus|Silva|8/17/2018|Salvador|5300|NaN|21200|
|192|1423|HL1918|iPhone|3|Dykson|Silva|9/30/2018|Salvador|5300|NaN|15900|
|193|1432|HL9962|Android|3|Breno|Costa|3/5/2018|Salvador|3400|NaN|10200|
|194|1434|HL1148|Câmera|1|Lucas|Araújo|3/26/2018|Salvador|2100|NaN|2100|
|195|1436|HL1918|iPhone|2|Luíza|Melo|9/14/2018|Salvador|5300|NaN|10600|
|196|1445|HL7348|SmartWatch|2|Lívia|Marques|7/1/2018|Salvador|1400|NaN|2800|
|197|1450|HL1918|iPhone|1|Lázaro|Villanova|12/21/2018|Salvador|5300|NaN|5300|
|198|1454|HL9962|Android|5|Carolina|Silva|9/7/2018|Salvador|3400|NaN|17000|
|199|1477|HL1148|Câmera|2|Ulisses|Filho|11/1/2018|Salvador|2100|NaN|4200|
|200|1482|HL8851|Notebook|4|Carolina|Santos|12/6/2018|Salvador|3500|NaN|14000|
|201|1489|HL4379|Televisão|2|Eduardo|Vargas|4/7/2018|Salvador|2500|NaN|5000|
|202|1499|HL1918|iPhone|3|Matheus|Gomes|2/10/2018|Salvador|5300|NaN|15900|
|203|1512|HL1918|iPhone|4|Priscila|Suzano|9/2/2018|Salvador|5300|NaN|21200|
|204|1526|HL7348|SmartWatch|2|Julia|Leite|4/9/2018|Salvador|1400|NaN|2800|
|205|1527|HL1918|iPhone|2|Platini|Heimlich|1/20/2018|Salvador|5300|NaN|10600|
|206|1531|HL4379|Televisão|2|Matheus|Moraes|3/11/2018|Salvador|2500|NaN|5000|
|207|1549|HL2714|Tablet|1|Pedro|Ayres|10/6/2018|Salvador|1600|NaN|1600|
|208|1552|HL4379|Televisão|4|Clara|Silveira|11/7/2018|Salvador|2500|NaN|10000|
|209|1554|HL4379|Televisão|2|Gabrielle|Vasconcelos|4/16/2018|Salvador|2500|NaN|5000|
|210|1566|HL2714|Tablet|1|Livia|Corrêa|9/19/2018|Salvador|1600|NaN|1600|
|211|1569|HL7348|SmartWatch|4|Victor|Franco|10/15/2018|Salvador|1400|NaN|5600|
|212|1572|HL4379|Televisão|2|João|Araujo|11/5/2018|Salvador|2500|NaN|5000|
|213|1583|HL7348|SmartWatch|2|Giuseppe|Bhering|2/19/2018|Salvador|1400|NaN|2800|
|214|1584|HL7348|SmartWatch|3|Luísa|Fonseca|10/22/2018|Salvador|1400|NaN|4200|
|215|1594|HL4379|Televisão|3|Gabriel|Puntel|4/22/2018|Salvador|2500|NaN|7500|
|216|1612|HL9962|Android|1|Leandro|Ferreira|5/19/2018|Salvador|3400|NaN|3400|
|217|1617|HL7348|SmartWatch|2|Ana|Gonzaga|1/30/2018|Salvador|1400|NaN|2800|
|218|1621|HL1148|Câmera|5|Lázaro|Nascimento|6/4/2018|Salvador|2100|NaN|10500|
|219|1622|HL4379|Televisão|2|Patrícia|Fernandes|7/20/2018|Salvador|2500|NaN|5000|
|220|1625|HL4379|Televisão|1|Glenda|Santos|10/1/2018|Salvador|2500|NaN|2500|
|221|1627|HL8851|Notebook|1|Antônio|Soares|1/26/2018|Salvador|3500|NaN|3500|
|222|1628|HL1918|iPhone|3|Marina|Aragão|11/17/2018|Salvador|5300|NaN|15900|
|223|1632|HL4379|Televisão|5|Fillipe|Almeida|12/27/2018|Salvador|2500|NaN|12500|
|224|1634|HL7348|SmartWatch|3|Amanda|Gontijo|11/6/2018|Salvador|1400|NaN|4200|
|225|1635|HL8851|Notebook|5|Rafael|Guimarães|9/4/2018|Salvador|3500|NaN|17500|
|226|1643|HL2714|Tablet|3|Rodrigo|Souza|6/4/2018|Salvador|1600|NaN|4800|
|227|1646|HL7348|SmartWatch|2|João|Fonseca|8/18/2018|Salvador|1400|NaN|2800|
|228|1648|HL9962|Android|4|Clarissa|Santos|7/25/2018|Salvador|3400|NaN|13600|
|229|1649|HL8851|Notebook|3|Maurício|Dias|7/9/2018|Salvador|3500|NaN|10500|
|230|1654|HL2714|Tablet|5|Ruan|Lopes|7/15/2018|Salvador|1600|NaN|8000|
|231|1658|HL7348|SmartWatch|1|João|Siqueira|12/25/2018|Salvador|1400|NaN|1400|
|232|1666|HL7348|SmartWatch|4|Bruno|Ferreira|1/25/2018|Salvador|1400|NaN|5600|
|233|1673|HL2714|Tablet|5|Patrícia|Amaral|10/27/2018|Salvador|1600|NaN|8000|
|234|1701|HL7348|SmartWatch|5|Breno|Farias|6/28/2018|Salvador|1400|NaN|7000|
|235|1702|HL1148|Câmera|4|Camila|Sobral|4/27/2018|Salvador|2100|NaN|8400|
|236|1711|HL8851|Notebook|1|Bianca|Procaci|12/19/2018|Salvador|3500|NaN|3500|
|237|1716|HL9962|Android|1|Bernardo|Botelho|3/1/2018|Salvador|3400|NaN|3400|
|238|1729|HL2714|Tablet|1|Juliana|Souza|9/4/2018|Salvador|1600|NaN|1600|
|239|1730|HL7348|SmartWatch|5|Julia|Leite|7/12/2018|Salvador|1400|NaN|7000|
|240|1731|HL4379|Televisão|4|João|Araujo|12/11/2018|Salvador|2500|NaN|10000|
|241|1732|HL1148|Câmera|3|Amanda|Amaral|1/22/2018|Salvador|2100|NaN|6300|
|242|1737|HL4379|Televisão|1|Rogério|Pereira|3/20/2018|Salvador|2500|NaN|2500|
|243|1749|HL9962|Android|3|Rafael|Carneiro|1/14/2018|Salvador|3400|NaN|10200|
|244|1750|HL9962|Android|1|Raíza|Lopes|10/16/2018|Salvador|3400|NaN|3400|
|245|1751|HL9962|Android|4|Isabella|Rodrigues|8/16/2018|Salvador|3400|NaN|13600|
|246|1752|HL9962|Android|5|Michelle|Figueiredo|12/7/2018|Salvador|3400|NaN|17000|
|247|1757|HL7348|SmartWatch|5|Eduardo|Soares|8/23/2018|Salvador|1400|NaN|7000|
|248|1760|HL1148|Câmera|4|Bernardo|Borges|10/5/2018|Salvador|2100|NaN|8400|
|249|1768|HL9962|Android|4|Pedro|Bitencourt|4/23/2018|Salvador|3400|NaN|13600|
|250|1805|HL1918|iPhone|3|Beatriz|Li|6/17/2018|Salvador|5300|NaN|15900|
|251|1815|HL4379|Televisão|4|Marcos|Nucci|2/24/2018|Salvador|2500|NaN|10000|
|252|1817|HL1918|iPhone|2|Leandro|Melo|12/11/2018|Salvador|5300|NaN|10600|
|253|1821|HL4379|Televisão|1|Ruan|Lopes|1/19/2018|Salvador|2500|NaN|2500|
|254|1829|HL8851|Notebook|3|Luiz|Limp|9/19/2018|Salvador|3500|NaN|10500|
|255|1839|HL1918|iPhone|2|Rodrigo|Ramos|4/10/2018|Salvador|5300|NaN|10600|
|256|1842|HL7348|SmartWatch|3|Victor|Gomes|9/6/2018|Salvador|1400|NaN|4200|
|257|1849|HL2714|Tablet|2|Amanda|Machado|9/4/2018|Salvador|1600|NaN|3200|
|258|1873|HL1148|Câmera|2|Mariane|Ferreira|7/25/2018|Salvador|2100|NaN|4200|
|259|1875|HL1918|iPhone|5|Priscila|Carvalho|10/18/2018|Salvador|5300|NaN|26500|
|260|1884|HL1918|iPhone|3|Eduardo|Silva|11/10/2018|Salvador|5300|NaN|15900|
|261|1888|HL2714|Tablet|4|Raphael|Filho|11/11/2018|Salvador|1600|NaN|6400|
|262|1898|HL2714|Tablet|3|Luíza|Garcia|9/28/2018|Salvador|1600|NaN|4800|
|263|1899|HL9962|Android|5|Raissa|Sales|10/26/2018|Salvador|3400|NaN|17000|
|264|1907|HL1918|iPhone|3|Juliana|Guimarães|3/25/2018|Salvador|5300|NaN|15900|
|265|1916|HL1918|iPhone|1|Renan|Melo|9/2/2018|Salvador|5300|NaN|5300|
|266|1919|HL1148|Câmera|4|Juliana|Silva|5/26/2018|Salvador|2100|NaN|8400|
|267|1920|HL1918|iPhone|3|Carlos|Mesquita|10/22/2018|Salvador|5300|NaN|15900|
|268|1927|HL4379|Televisão|4|Raísa|Berto|2/24/2018|Salvador|2500|NaN|10000|
|269|1928|HL1148|Câmera|1|Carla|Zakhm|9/16/2018|Salvador|2100|NaN|2100|
|270|1937|HL7348|SmartWatch|2|Caio|Affonso|12/4/2018|Salvador|1400|NaN|2800|
|271|1950|HL4379|Televisão|4|Amanda|Procaci|4/2/2018|Salvador|2500|NaN|10000|
|272|1952|HL1918|iPhone|3|Leandro|Rodrigues|3/16/2018|Salvador|5300|NaN|15900|
|273|1955|HL9962|Android|3|Lunna|Vannier|12/1/2018|Salvador|3400|NaN|10200|
|274|1963|HL8851|Notebook|3|Rodrigo|Bruno|4/19/2018|Salvador|3500|NaN|10500|
|275|1966|HL1918|iPhone|1|Luis|Silva|4/6/2018|Salvador|5300|NaN|5300|
|276|1972|HL7348|SmartWatch|5|Roberta|Pimenta|2/22/2018|Salvador|1400|NaN|7000|
|277|1981|HL9962|Android|3|Ana|Gomes|6/24/2018|Salvador|3400|NaN|10200|
|278|1987|HL2714|Tablet|2|Bianca|Paz|8/24/2018|Salvador|1600|NaN|3200|
|279|1996|HL9962|Android|2|Mateus|Franco|4/5/2018|Salvador|3400|NaN|6800|
|280|2001|HL1918|iPhone|5|Isabel|Mesquita|10/19/2018|Salvador|5300|NaN|26500|
|281|2002|HL9962|Android|4|Lucas|Reis|3/26/2018|Salvador|3400|NaN|13600|
|282|2006|HL2714|Tablet|1|Bianca|Paz|9/19/2018|Salvador|1600|NaN|1600|
|283|2008|HL1918|iPhone|1|Hércules|Júnior|3/4/2018|Salvador|5300|NaN|5300|
|284|2010|HL1918|iPhone|2|Rebeca|Taylor|6/23/2018|Salvador|5300|NaN|10600|
|285|2011|HL8851|Notebook|4|Rodrigo|Silva|11/12/2018|Salvador|3500|NaN|14000|
|286|2012|HL8851|Notebook|2|Thales|Portillo|8/1/2018|Salvador|3500|NaN|7000|
|287|2017|HL7348|SmartWatch|3|Izabel|Miura|2/26/2018|Salvador|1400|NaN|4200|
|288|2027|HL7348|SmartWatch|4|Michelle|Miura|7/26/2018|Salvador|1400|NaN|5600|
|289|2036|HL9962|Android|3|Ana|Leite|10/18/2018|Salvador|3400|NaN|10200|
|290|2039|HL7348|SmartWatch|1|Ruan|Gonçalves|11/16/2018|Salvador|1400|NaN|1400|
|291|2043|HL9962|Android|2|Lucas|Valim|12/15/2018|Salvador|3400|NaN|6800|
|292|2048|HL1148|Câmera|1|Ruan|Lopes|7/29/2018|Salvador|2100|NaN|2100|
|293|2057|HL4379|Televisão|2|Pedro|Pereira|9/8/2018|Salvador|2500|NaN|5000|
|294|2059|HL7348|SmartWatch|5|Rachel|Silva|7/18/2018|Salvador|1400|NaN|7000|
|295|2062|HL4379|Televisão|5|Leonardo|Faria|9/22/2018|Salvador|2500|NaN|12500|
|296|2063|HL2714|Tablet|1|Pedro|Sena|2/5/2018|Salvador|1600|NaN|1600|
|297|2072|HL2714|Tablet|1|Fernanda|Junior|2/22/2018|Salvador|1600|NaN|1600|
|298|2079|HL1148|Câmera|5|Kim|Ferreira|9/11/2018|Salvador|2100|NaN|10500|
|299|2082|HL2714|Tablet|1|Júlio|Fraga|1/9/2018|Salvador|1600|NaN|1600|
|300|2085|HL1918|iPhone|3|Célio|Xavier|9/11/2018|Salvador|5300|NaN|15900|
|301|2088|HL1918|iPhone|2|Marina|Miranda|7/25/2018|Salvador|5300|NaN|10600|
|302|2092|HL8851|Notebook|1|Pedro|Pereira|11/3/2018|Salvador|3500|NaN|3500|
|303|2102|HL1918|iPhone|2|Lucas|Wanderley|3/10/2018|Salvador|5300|NaN|10600|
|304|2106|HL1918|iPhone|1|Felipe|Freitas|12/27/2018|Salvador|5300|NaN|5300|
|305|2114|HL4379|Televisão|3|Rojane|Lima|9/5/2018|Salvador|2500|NaN|7500|
|306|2128|HL1918|iPhone|4|Eduardo|Nunes|4/26/2018|Salvador|5300|NaN|21200|
|307|2130|HL8851|Notebook|1|Andressa|Rotsztejn|9/15/2018|Salvador|3500|NaN|3500|
|308|2134|HL1918|iPhone|2|Sandy|Ribeiro|6/17/2018|Salvador|5300|NaN|10600|
|309|2136|HL8851|Notebook|3|Rafael|Wajnsztok|7/3/2018|Salvador|3500|NaN|10500|
|310|2145|HL4379|Televisão|5|Guilherme|Barbosa|8/22/2018|Salvador|2500|NaN|12500|
|311|2148|HL4379|Televisão|4|Renan|Melo|12/27/2018|Salvador|2500|NaN|10000|
|312|2159|HL1918|iPhone|4|Paola|Abreu|5/6/2018|Salvador|5300|NaN|21200|
|313|2166|HL7348|SmartWatch|1|Guilherme|Assis|11/17/2018|Salvador|1400|NaN|1400|
|314|2169|HL2714|Tablet|3|Livia|Codeceira|1/30/2018|Salvador|1600|NaN|4800|
|315|2172|HL4379|Televisão|3|Beatriz|Santos|8/9/2018|Salvador|2500|NaN|7500|
|316|2191|HL4379|Televisão|4|Wilson|Farias|12/11/2018|Salvador|2500|NaN|10000|
|317|2196|HL4379|Televisão|4|Lucas|Junior|12/7/2018|Salvador|2500|NaN|10000|
|318|2227|HL1918|iPhone|5|Bernardo|Nauenberg|2/10/2018|Salvador|5300|NaN|26500|
|319|2229|HL2714|Tablet|5|Wellington|Duarte|11/15/2018|Salvador|1600|NaN|8000|
|320|2237|HL4379|Televisão|3|Andressa|Nóbrega|10/23/2018|Salvador|2500|NaN|7500|
|321|2253|HL1918|iPhone|2|Marina|Perdomo|5/3/2018|Salvador|5300|NaN|10600|
|322|2257|HL9962|Android|5|Pedro|Oliveira|3/12/2018|Salvador|3400|NaN|17000|
|323|2258|HL1918|iPhone|2|Renan|Ventura|8/23/2018|Salvador|5300|NaN|10600|
|324|2259|HL1148|Câmera|3|Catarina|Teixeira|8/20/2018|Salvador|2100|NaN|6300|
|325|2271|HL9962|Android|1|Lucas|Valim|4/21/2018|Salvador|3400|NaN|3400|
|326|2276|HL4379|Televisão|3|Isabelle|Firmino|3/3/2018|Salvador|2500|NaN|7500|
|327|2284|HL4379|Televisão|3|Beatriz|Cavalcanti|2/3/2018|Salvador|2500|NaN|7500|
|328|2291|HL1918|iPhone|3|Luiz|Mendonça|6/5/2018|Salvador|5300|NaN|15900|
|329|2298|HL1918|iPhone|2|Ravena|Bhering|7/8/2018|Salvador|5300|NaN|10600|
|330|2309|HL1148|Câmera|2|Raissa|Maia|6/14/2018|Salvador|2100|NaN|4200|
|331|2312|HL4379|Televisão|5|Eric|Carvalho|3/21/2018|Salvador|2500|NaN|12500|
|332|2313|HL4379|Televisão|3|Carolina|Bernardes|2/18/2018|Salvador|2500|NaN|7500|
|333|2328|HL1918|iPhone|2|Lucas|Almeida|12/12/2018|Salvador|5300|NaN|10600|
|334|2332|HL4379|Televisão|3|João|Fonseca|10/1/2018|Salvador|2500|NaN|7500|
|335|2336|HL1148|Câmera|5|Luiz|Almeida|11/30/2018|Salvador|2100|NaN|10500|
|336|2345|HL4379|Televisão|5|Priscila|Garcia|2/7/2018|Salvador|2500|NaN|12500|
|337|2353|HL8851|Notebook|5|João|Luz|5/20/2018|Salvador|3500|NaN|17500|
|338|2356|HL2714|Tablet|5|Carlos|Barbosa|5/21/2018|Salvador|1600|NaN|8000|
|339|2362|HL4379|Televisão|4|Renan|Cunha|2/1/2018|Salvador|2500|NaN|10000|
|340|2363|HL7348|SmartWatch|4|Rodrigo|Ramos|2/25/2018|Salvador|1400|NaN|5600|
|341|2376|HL9962|Android|3|Anna|Silva|11/2/2018|Salvador|3400|NaN|10200|
|342|2381|HL4379|Televisão|2|Caio|Moraes|7/3/2018|Salvador|2500|NaN|5000|
|343|2386|HL7348|SmartWatch|4|Maria|Junior|12/2/2018|Salvador|1400|NaN|5600|
|344|2391|HL7348|SmartWatch|3|Thomáz|Rodriguez|4/19/2018|Salvador|1400|NaN|4200|
|345|2401|HL4379|Televisão|2|Raissa|Maia|2/28/2018|Salvador|2500|NaN|5000|
|346|2402|HL1918|iPhone|3|Laís|Oliveira|12/16/2018|Salvador|5300|NaN|15900|
|347|2405|HL1918|iPhone|2|Rafaela|Ferreira|4/25/2018|Salvador|5300|NaN|10600|
|348|2410|HL1918|iPhone|3|Katharina|Barros|11/24/2018|Salvador|5300|NaN|15900|
|349|2418|HL1918|iPhone|1|Lucas|Junior|11/25/2018|Salvador|5300|NaN|5300|
|350|2422|HL1148|Câmera|1|Maria|Gasperi|12/30/2018|Salvador|2100|NaN|2100|
|351|2426|HL7348|SmartWatch|2|Caroll|Johnson|2/16/2018|Salvador|1400|NaN|2800|
|352|2462|HL2714|Tablet|3|Mariana|Freire|5/22/2018|Salvador|1600|NaN|4800|
|353|2472|HL7348|SmartWatch|2|Daniela|Andrada|6/4/2018|Salvador|1400|NaN|2800|
|354|2481|HL8851|Notebook|4|João|Peçanha|4/25/2018|Salvador|3500|NaN|14000|
|355|2490|HL1918|iPhone|4|Gabrielle|Silva|12/10/2018|Salvador|5300|NaN|21200|
|356|2493|HL1918|iPhone|3|Henrique|Silva|10/13/2018|Salvador|5300|NaN|15900|
|357|2497|HL1148|Câmera|5|Gustavo|Aragão|5/16/2018|Salvador|2100|NaN|10500|
|358|2523|HL1918|iPhone|3|Ana|Leite|2/3/2018|Salvador|5300|NaN|15900|
|359|2528|HL9962|Android|3|Renan|Cunha|10/16/2018|Salvador|3400|NaN|10200|
|360|2542|HL9962|Android|5|Mariana|Barrozo|9/22/2018|Salvador|3400|NaN|17000|
|361|2543|HL8851|Notebook|4|Thomáz|Rodriguez|10/30/2018|Salvador|3500|NaN|14000|
|362|2545|HL1918|iPhone|2|Giselia|Thiele|12/22/2018|Salvador|5300|NaN|10600|
|363|2567|HL4379|Televisão|1|Leandro|Ferreira|1/27/2018|Salvador|2500|NaN|2500|
|364|2575|HL1148|Câmera|3|Marina|Miranda|5/15/2018|Salvador|2100|NaN|6300|
|365|2585|HL1918|iPhone|2|Lucas|Cavalcanti|8/11/2018|Salvador|5300|NaN|10600|
|366|2595|HL8851|Notebook|1|Michelle|Figueiredo|10/4/2018|Salvador|3500|NaN|3500|
|367|2596|HL1918|iPhone|5|Juliana|Huon|11/2/2018|Salvador|5300|NaN|26500|
|368|2599|HL7348|SmartWatch|3|Myllena|Corrêa|8/5/2018|Salvador|1400|NaN|4200|
|369|2624|HL1918|iPhone|3|Matheus|Ramos|1/21/2018|Salvador|5300|NaN|15900|
|370|2625|HL4379|Televisão|4|Lucas|Villanova|6/11/2018|Salvador|2500|NaN|10000|
|371|2627|HL7348|SmartWatch|1|Luíza|Garcia|5/3/2018|Salvador|1400|NaN|1400|
|372|2639|HL1918|iPhone|3|Katharina|Barros|2/16/2018|Salvador|5300|NaN|15900|
|373|2665|HL4379|Televisão|4|Livia|Corrêa|8/9/2018|Salvador|2500|NaN|10000|
|374|2666|HL4379|Televisão|3|Jonatas|Passos|8/8/2018|Salvador|2500|NaN|7500|
|375|2693|HL1918|iPhone|1|Raphael|Rezende|8/11/2018|Salvador|5300|NaN|5300|
|376|2696|HL4379|Televisão|2|Gabriel|Assis|7/21/2018|Salvador|2500|NaN|5000|
|377|2711|HL7348|SmartWatch|4|Gabriel|Thoni|6/27/2018|Salvador|1400|NaN|5600|
|378|2723|HL1918|iPhone|3|Matheus|Silva|9/14/2018|Salvador|5300|NaN|15900|
|379|2727|HL1148|Câmera|1|Gabriel|Thome|4/4/2018|Salvador|2100|NaN|2100|
|380|2729|HL1918|iPhone|5|Gabriela|Mello|3/3/2018|Salvador|5300|NaN|26500|
|381|2754|HL8851|Notebook|1|Jonas|Gomes|1/8/2018|Salvador|3500|NaN|3500|
|382|2759|HL1918|iPhone|2|Ana|Soledade|8/27/2018|Salvador|5300|NaN|10600|
|383|2762|HL9962|Android|3|Michelle|Miura|6/28/2018|Salvador|3400|NaN|10200|
|384|2763|HL1918|iPhone|5|Caio|Caldas|6/11/2018|Salvador|5300|NaN|26500|
|385|2764|HL4379|Televisão|2|Julia|Teixeira|2/1/2018|Salvador|2500|NaN|5000|
|386|2771|HL8851|Notebook|5|João|Matheus|3/27/2018|Salvador|3500|NaN|17500|
|387|2777|HL1918|iPhone|1|Silvio|Fahrnholz|1/26/2018|Salvador|5300|NaN|5300|
|388|2788|HL1918|iPhone|2|Milena|Alcoforado|4/30/2018|Salvador|5300|NaN|10600|
|389|2802|HL1918|iPhone|5|Marina|Perdomo|7/29/2018|Salvador|5300|NaN|26500|
|390|2804|HL1148|Câmera|1|Daniel|Cardoso|9/7/2018|Salvador|2100|NaN|2100|
|391|2806|HL1918|iPhone|1|Fernanda|Bhering|10/10/2018|Salvador|5300|NaN|5300|
|392|2810|HL1918|iPhone|3|Pedro|Santana|7/5/2018|Salvador|5300|NaN|15900|
|393|2813|HL1918|iPhone|4|Ana|Fioretti|5/5/2018|Salvador|5300|NaN|21200|
|394|2825|HL1918|iPhone|4|Raíssa|Oros|1/1/2018|Salvador|5300|NaN|21200|
|395|2826|HL4379|Televisão|4|Danilo|Alves|5/4/2018|Salvador|2500|NaN|10000|
|396|2850|HL4379|Televisão|4|Willian|Albino|6/6/2018|Salvador|2500|NaN|10000|
|397|2866|HL1148|Câmera|4|Ana|Bôas|4/6/2018|Salvador|2100|NaN|8400|
|398|2874|HL4379|Televisão|5|Fabio|Sepúlveda|6/6/2018|Salvador|2500|NaN|12500|
|399|2891|HL2714|Tablet|4|Jessica|Ferreira|10/24/2018|Salvador|1600|NaN|6400|
|400|2893|HL2714|Tablet|5|Thiago|Costa|6/25/2018|Salvador|1600|NaN|8000|
|401|2900|HL4379|Televisão|4|William|Mendonça|6/1/2018|Salvador|2500|NaN|10000|
|402|2901|HL4379|Televisão|1|Maria|Gasperi|10/6/2018|Salvador|2500|NaN|2500|
|403|2917|HL1918|iPhone|5|João|Aires|9/28/2018|Salvador|5300|NaN|26500|
|404|2933|HL4379|Televisão|3|Roberta|Pimenta|1/28/2018|Salvador|2500|NaN|7500|
|405|2934|HL7348|SmartWatch|4|Cláudio|Aragão|6/11/2018|Salvador|1400|NaN|5600|
|406|2952|HL1918|iPhone|4|Priscila|Garcia|8/23/2018|Salvador|5300|NaN|21200|
|407|2954|HL4379|Televisão|3|Caroline|Cavalcanti|2/22/2018|Salvador|2500|NaN|7500|
|408|2964|HL4379|Televisão|1|Mônica|Rotolo|7/16/2018|Salvador|2500|NaN|2500|
|409|2965|HL7348|SmartWatch|4|Vinícius|Antunes|6/30/2018|Salvador|1400|NaN|5600|
|410|2974|HL7348|SmartWatch|3|Vitor|Boccaletti|1/16/2018|Salvador|1400|NaN|4200|
|411|2979|HL1148|Câmera|2|Victor|Oliveira|3/26/2018|Salvador|2100|NaN|4200|
|412|3004|HL1918|iPhone|1|Lucas|Destri|1/12/2018|Salvador|5300|NaN|5300|
|413|3007|HL8851|Notebook|4|Anízio|Carvalho|7/30/2018|Salvador|3500|NaN|14000|
|414|3009|HL2714|Tablet|4|Sandy|Ribeiro|12/2/2018|Salvador|1600|NaN|6400|
|415|3039|HL8851|Notebook|3|Filipe|Barros|1/2/2018|Salvador|3500|NaN|10500|
|416|3046|HL1918|iPhone|3|Itai|Puntel|10/21/2018|Salvador|5300|NaN|15900|
|417|3061|HL4379|Televisão|3|Raissa|Maia|2/14/2018|Salvador|2500|NaN|7500|
|418|3063|HL8851|Notebook|2|Henrique|Silva|11/14/2018|Salvador|3500|NaN|7000|
|419|3066|HL2714|Tablet|5|Victoria|Mazza|8/30/2018|Salvador|1600|NaN|8000|
|420|3072|HL4379|Televisão|4|Igor|Lima|7/19/2018|Salvador|2500|NaN|10000|
|421|3079|HL7348|SmartWatch|5|Paula|Calbucci|9/19/2018|Salvador|1400|NaN|7000|
|422|3086|HL8851|Notebook|3|Ives|Teixeira|3/31/2018|Salvador|3500|NaN|10500|
|423|3087|HL1918|iPhone|5|Norman|Jimbo|8/30/2018|Salvador|5300|NaN|26500|
|424|3088|HL8851|Notebook|4|Priscila|Carvalho|5/21/2018|Salvador|3500|NaN|14000|
|425|3091|HL4379|Televisão|3|Pedro|Ferrari|12/25/2018|Salvador|2500|NaN|7500|
|426|3095|HL1918|iPhone|5|Helena|Chafin|5/19/2018|Salvador|5300|NaN|26500|
|427|3096|HL7348|SmartWatch|2|Raphael|Ferman|12/25/2018|Salvador|1400|NaN|2800|
|428|3112|HL4379|Televisão|5|Renan|Freire|7/15/2018|Salvador|2500|NaN|12500|
|429|3116|HL2714|Tablet|1|Deysiane|Medronho|1/15/2018|Salvador|1600|NaN|1600|
|430|3125|HL4379|Televisão|4|Adriana|Carneiro|1/3/2018|Salvador|2500|NaN|10000|
|431|3131|HL9962|Android|2|Felipe|Freitas|10/1/2018|Salvador|3400|NaN|6800|
|432|3140|HL2714|Tablet|2|Matheus|Silva|8/19/2018|Salvador|1600|NaN|3200|
|433|3142|HL1918|iPhone|5|Bianca|Tatsch|9/19/2018|Salvador|5300|NaN|26500|
|434|3171|HL1918|iPhone|1|Carolina|Vasconcelos|10/8/2018|Salvador|5300|NaN|5300|
|435|3176|HL1918|iPhone|1|Gustavo|Accardo|12/24/2018|Salvador|5300|NaN|5300|
|436|3199|HL4379|Televisão|3|Tainah|Nogueira|12/12/2018|Salvador|2500|NaN|7500|
|437|3207|HL8851|Notebook|5|Stephanie|Gonçalves|5/31/2018|Salvador|3500|NaN|17500|
|438|3225|HL1918|iPhone|4|Alvaro|Kranz|4/10/2018|Salvador|5300|NaN|21200|
|439|3237|HL1918|iPhone|4|Camila|Bastazini|6/26/2018|Salvador|5300|NaN|21200|
|440|3243|HL1918|iPhone|5|Rodrigo|Feijo|10/3/2018|Salvador|5300|NaN|26500|
|441|3248|HL8851|Notebook|3|Luana|Santos|5/21/2018|Salvador|3500|NaN|10500|
|442|3250|HL1918|iPhone|3|Fernanda|Ferreira|8/8/2018|Salvador|5300|NaN|15900|
|443|3251|HL9962|Android|2|João|Capitulo|4/7/2018|Salvador|3400|NaN|6800|
|444|3259|HL7348|SmartWatch|3|Luiz|Freire|9/29/2018|Salvador|1400|NaN|4200|
|445|3265|HL2714|Tablet|1|Carolina|Santos|4/29/2018|Salvador|1600|NaN|1600|
|446|3278|HL1918|iPhone|4|Leandro|Rodrigues|8/31/2018|Salvador|5300|NaN|21200|
|447|3283|HL2714|Tablet|4|Aline|Mello|9/24/2018|Salvador|1600|NaN|6400|
|448|3286|HL2714|Tablet|1|Fernanda|Silva|6/24/2018|Salvador|1600|NaN|1600|
|449|3308|HL4379|Televisão|4|Carlos|Melo|5/22/2018|Salvador|2500|NaN|10000|
|450|3328|HL1918|iPhone|2|Lucas|Wanderley|5/23/2018|Salvador|5300|NaN|10600|
|451|3330|HL1918|iPhone|1|Bruno|Souza|1/19/2018|Salvador|5300|NaN|5300|
|452|3339|HL9962|Android|3|Gabriel|Assis|1/11/2018|Salvador|3400|NaN|10200|
|453|3354|HL7348|SmartWatch|3|Paula|Cavalcanti|8/26/2018|Salvador|1400|NaN|4200|
|454|3357|HL1918|iPhone|3|Lázaro|Nascimento|6/18/2018|Salvador|5300|NaN|15900|
|455|3361|HL1148|Câmera|4|Matheus|Santos|10/13/2018|Salvador|2100|NaN|8400|
|456|3371|HL1918|iPhone|4|Jéssica|Netto|5/18/2018|Salvador|5300|NaN|21200|
|457|3373|HL2714|Tablet|3|Pedro|Oliveira|10/24/2018|Salvador|1600|NaN|4800|
|458|3379|HL8851|Notebook|5|Luis|Silva|12/8/2018|Salvador|3500|NaN|17500|
|459|3384|HL9962|Android|1|Henrique|Silva|2/12/2018|Salvador|3400|NaN|3400|
|460|3436|HL1918|iPhone|2|Gustavo|Thome|10/26/2018|Salvador|5300|NaN|10600|
|461|3440|HL8851|Notebook|4|Julie|Ferreira|12/28/2018|Salvador|3500|NaN|14000|
|462|3446|HL8851|Notebook|5|Yasmim|Verly|7/30/2018|Salvador|3500|NaN|17500|
|463|3451|HL2714|Tablet|4|Guilherme|Jordao|12/12/2018|Salvador|1600|NaN|6400|
|464|3461|HL4379|Televisão|2|Giulia|Pessanha|10/6/2018|Salvador|2500|NaN|5000|
|465|3464|HL2714|Tablet|5|Diego|Mello|6/21/2018|Salvador|1600|NaN|8000|
|466|3468|HL4379|Televisão|4|Guilherme|Seixas|7/24/2018|Salvador|2500|NaN|10000|
|467|3475|HL2714|Tablet|1|Diogo|Peixoto|9/21/2018|Salvador|1600|NaN|1600|
|468|3476|HL2714|Tablet|3|Milena|Alcoforado|4/14/2018|Salvador|1600|NaN|4800|
|469|3482|HL9962|Android|3|Lucas|Coelho|5/1/2018|Salvador|3400|NaN|10200|
|470|3491|HL1148|Câmera|5|Bernard|Pedrosa|3/19/2018|Salvador|2100|NaN|10500|
|471|3496|HL2714|Tablet|5|Aline|Andrade|12/30/2018|Salvador|1600|NaN|8000|
|472|3516|HL7348|SmartWatch|5|Isabela|Rodrigues|1/13/2018|Salvador|1400|NaN|7000|
|473|3517|HL7348|SmartWatch|4|Paula|Isbelle|11/11/2018|Salvador|1400|NaN|5600|
|474|3525|HL9962|Android|4|Glenda|Santos|3/3/2018|Salvador|3400|NaN|13600|
|475|3526|HL1918|iPhone|4|Joao|Silva|4/10/2018|Salvador|5300|NaN|21200|
|476|3537|HL7348|SmartWatch|1|Caroline|Aquino|9/12/2018|Salvador|1400|NaN|1400|
|477|3561|HL1918|iPhone|1|Júlio|Freire|12/4/2018|Salvador|5300|NaN|5300|
|478|3564|HL7348|SmartWatch|2|Amanda|Roberto|9/6/2018|Salvador|1400|NaN|2800|
|479|3565|HL1918|iPhone|2|Nathan|Morelli|7/17/2018|Salvador|5300|NaN|10600|
|480|3568|HL2714|Tablet|4|Marcelo|Rosa|12/5/2018|Salvador|1600|NaN|6400|
|481|3569|HL1148|Câmera|1|Nathalia|Ventura|8/9/2018|Salvador|2100|NaN|2100|
|482|3571|HL4379|Televisão|2|Myllena|Corrêa|5/22/2018|Salvador|2500|NaN|5000|
|483|3576|HL1918|iPhone|1|Vanessa|Bach|5/25/2018|Salvador|5300|NaN|5300|
|484|3581|HL4379|Televisão|1|Julia|Silva|1/18/2018|Salvador|2500|NaN|2500|
|485|3592|HL2714|Tablet|5|Guilherme|Rachide|8/23/2018|Salvador|1600|NaN|8000|
|486|3596|HL1918|iPhone|4|Karina|Camara|7/15/2018|Salvador|5300|NaN|21200|
|487|3606|HL4379|Televisão|3|Carolina|Vasconcelos|4/6/2018|Salvador|2500|NaN|7500|
|488|3607|HL2714|Tablet|4|João|Araujo|6/20/2018|Salvador|1600|NaN|6400|
|489|3618|HL1918|iPhone|1|Daniela|Pereira|10/2/2018|Salvador|5300|NaN|5300|
|490|3631|HL1918|iPhone|2|Andressa|Rotsztejn|2/3/2018|Salvador|5300|NaN|10600|
|491|3640|HL8851|Notebook|1|Pedro|Santana|11/22/2018|Salvador|3500|NaN|3500|
|492|3657|HL8851|Notebook|1|Sthefeson|Kohn|5/20/2018|Salvador|3500|NaN|3500|
|493|3663|HL4379|Televisão|3|Luiz|Conceição|10/19/2018|Salvador|2500|NaN|7500|
|494|3672|HL7348|SmartWatch|5|Rebeca|Manhães|3/1/2018|Salvador|1400|NaN|7000|
|495|3686|HL1148|Câmera|1|Vitor|Campos|10/12/2018|Salvador|2100|NaN|2100|
|496|3699|HL1918|iPhone|2|Mariana|Rotava|9/13/2018|Salvador|5300|NaN|10600|
|497|3711|HL2714|Tablet|2|Joyce|Souza|6/17/2018|Salvador|1600|NaN|3200|
|498|3732|HL1918|iPhone|3|Victor|Franco|12/11/2018|Salvador|5300|NaN|15900|
|499|3735|HL2714|Tablet|1|João|Luz|7/8/2018|Salvador|1600|NaN|1600|
|500|3736|HL2714|Tablet|1|Marina|Mesquita|4/19/2018|Salvador|1600|NaN|1600|
|501|3745|HL8851|Notebook|2|Juan|Barbosa|5/13/2018|Salvador|3500|NaN|7000|
|502|3746|HL1918|iPhone|1|Carlos|Galvão|7/18/2018|Salvador|5300|NaN|5300|
|503|3749|HL1148|Câmera|3|Daniel|Araujo|3/22/2018|Salvador|2100|NaN|6300|
|504|3778|HL8851|Notebook|3|Beatriz|Rocha|11/6/2018|Salvador|3500|NaN|10500|
|505|3788|HL4379|Televisão|1|Leandro|Melo|11/8/2018|Salvador|2500|NaN|2500|
|506|3789|HL1918|iPhone|2|João|Ribeiro|1/22/2018|Salvador|5300|NaN|10600|
|507|3791|HL1918|iPhone|4|João|Pedrazza|8/27/2018|Salvador|5300|NaN|21200|
|508|3798|HL4379|Televisão|3|Camilla|Vieira|7/4/2018|Salvador|2500|NaN|7500|
|509|3802|HL9962|Android|5|Clara|Bruno|2/27/2018|Salvador|3400|NaN|17000|
|510|3811|HL4379|Televisão|5|Sandy|Figueiredo|8/2/2018|Salvador|2500|NaN|12500|
|511|3818|HL9962|Android|3|Felipe|Cavalcanti|6/25/2018|Salvador|3400|NaN|10200|
|512|3824|HL9962|Android|3|Giovanna|Santos|1/10/2018|Salvador|3400|NaN|10200|
|513|3842|HL9962|Android|5|Michelle|Pereira|12/14/2018|Salvador|3400|NaN|17000|
|514|3850|HL1918|iPhone|4|Guilherme|Jordao|6/26/2018|Salvador|5300|NaN|21200|
|515|3859|HL4379|Televisão|4|Matheus|Santos|11/12/2018|Salvador|2500|NaN|10000|
|516|3860|HL4379|Televisão|1|Natali|Rangel|7/12/2018|Salvador|2500|NaN|2500|
|517|3875|HL4379|Televisão|3|David|Assumpção|9/12/2018|Salvador|2500|NaN|7500|
|518|3876|HL4379|Televisão|5|Dandara|Reis|1/3/2018|Salvador|2500|NaN|12500|
|519|3879|HL7348|SmartWatch|3|Carlos|Assis|2/7/2018|Salvador|1400|NaN|4200|
|520|3880|HL4379|Televisão|2|Luã|Sá|2/12/2018|Salvador|2500|NaN|5000|
|521|3884|HL8851|Notebook|2|Raphael|Machado|2/10/2018|Salvador|3500|NaN|7000|
|522|3898|HL1918|iPhone|2|Luiza|Ribeiro|11/22/2018|Salvador|5300|NaN|10600|
|523|3906|HL9962|Android|3|Tayla|Lima|11/7/2018|Salvador|3400|NaN|10200|
|524|3914|HL8851|Notebook|5|Andressa|Rotsztejn|2/7/2018|Salvador|3500|NaN|17500|
|525|3926|HL4379|Televisão|2|Lázaro|Villanova|3/4/2018|Salvador|2500|NaN|5000|
|526|3933|HL1918|iPhone|3|Stefan|Santos|2/7/2018|Salvador|5300|NaN|15900|
|527|3940|HL1918|iPhone|4|Gabriel|Assis|10/3/2018|Salvador|5300|NaN|21200|
|528|3954|HL4379|Televisão|3|Alvaro|Kranz|6/14/2018|Salvador|2500|NaN|7500|
|529|3961|HL1918|iPhone|3|Natalia|Accioly|7/10/2018|Salvador|5300|NaN|15900|
|530|3976|HL8851|Notebook|5|Ana|Monte|7/28/2018|Salvador|3500|NaN|17500|
|531|3977|HL8851|Notebook|3|Lara|Moreira|8/21/2018|Salvador|3500|NaN|10500|
|532|3979|HL1918|iPhone|4|Camila|Bastazini|10/17/2018|Salvador|5300|NaN|21200|
|533|3990|HL1918|iPhone|1|Eduardo|Silva|12/16/2018|Salvador|5300|NaN|5300|
|534|3991|HL4379|Televisão|3|Beatriz|Perdomo|2/20/2018|Salvador|2500|NaN|7500|
|535|3992|HL7348|SmartWatch|3|Felipe|Mendonça|6/30/2018|Salvador|1400|NaN|4200|
|536|4015|HL1918|iPhone|5|Diego|Mello|11/2/2018|Salvador|5300|NaN|26500|
|537|4022|HL1148|Câmera|2|Lucas|Lemos|4/10/2018|Salvador|2100|NaN|4200|
|538|4035|HL1918|iPhone|5|Victor|Lira|9/29/2018|Salvador|5300|NaN|26500|
|539|4045|HL7348|SmartWatch|5|Jéssica|Teixeira|3/13/2018|Salvador|1400|NaN|7000|
|540|4047|HL1918|iPhone|2|Itai|Puntel|9/13/2018|Salvador|5300|NaN|10600|
|541|4051|HL4379|Televisão|4|Camila|Sobral|1/15/2018|Salvador|2500|NaN|10000|
|542|4057|HL9962|Android|1|Dandara|Reis|5/12/2018|Salvador|3400|NaN|3400|
|543|4059|HL1918|iPhone|2|Pedro|Jorge|11/19/2018|Salvador|5300|NaN|10600|
|544|4061|HL1918|iPhone|5|Gabriel|Azevedo|8/24/2018|Salvador|5300|NaN|26500|
|545|4070|HL4379|Televisão|3|Thayane|Resende|12/27/2018|Salvador|2500|NaN|7500|
|546|4073|HL2714|Tablet|1|Rogério|Gentile|10/25/2018|Salvador|1600|NaN|1600|
|547|4083|HL1918|iPhone|2|Bruna|Gomes|6/18/2018|Salvador|5300|NaN|10600|
|548|4084|HL7348|SmartWatch|2|Giulia|Lopes|11/17/2018|Salvador|1400|NaN|2800|
|549|4093|HL4379|Televisão|4|Luiza|Cabral|4/26/2018|Salvador|2500|NaN|10000|
|550|4101|HL1148|Câmera|2|Priscila|Vogel|10/16/2018|Salvador|2100|NaN|4200|
|551|4102|HL2714|Tablet|2|Leonardo|Ferreira|7/2/2018|Salvador|1600|NaN|3200|
|552|4107|HL1918|iPhone|1|Luísa|Fonseca|11/16/2018|Salvador|5300|NaN|5300|
|553|4112|HL7348|SmartWatch|4|Priscila|Carvalho|5/22/2018|Salvador|1400|NaN|5600|
|554|4122|HL4379|Televisão|3|Adriana|Carneiro|7/2/2018|Salvador|2500|NaN|7500|
|555|4126|HL4379|Televisão|2|Thales|Santos|8/6/2018|Salvador|2500|NaN|5000|
|556|4166|HL1918|iPhone|2|Maria|Mello|3/2/2018|Salvador|5300|NaN|10600|
|557|4174|HL1918|iPhone|3|Gustavo|Guimarães|6/12/2018|Salvador|5300|NaN|15900|
|558|4196|HL2714|Tablet|1|Bruno|Salomão|5/5/2018|Salvador|1600|NaN|1600|
|559|4204|HL4379|Televisão|4|Rubens|Netto|11/27/2018|Salvador|2500|NaN|10000|
|560|4205|HL7348|SmartWatch|4|Bruna|Brandao|6/7/2018|Salvador|1400|NaN|5600|
|561|4211|HL4379|Televisão|5|Henrique|Oliveira|8/3/2018|Salvador|2500|NaN|12500|
|562|4227|HL2714|Tablet|2|Joao|Silva|1/30/2018|Salvador|1600|NaN|3200|
|563|4228|HL8851|Notebook|4|Danilo|Mendonça|10/4/2018|Salvador|3500|NaN|14000|
|564|4247|HL4379|Televisão|3|Gabriel|Rubim|10/2/2018|Salvador|2500|NaN|7500|
|565|4251|HL4379|Televisão|2|Victor|Lira|10/29/2018|Salvador|2500|NaN|5000|
|566|4260|HL1918|iPhone|4|Victor|Oliveira|2/21/2018|Salvador|5300|NaN|21200|
|567|4266|HL2714|Tablet|1|Lucas|Reis|10/12/2018|Salvador|1600|NaN|1600|
|568|4275|HL2714|Tablet|3|Wilson|Brandão|11/12/2018|Salvador|1600|NaN|4800|
|569|4292|HL8851|Notebook|2|Júlio|Fraga|2/18/2018|Salvador|3500|NaN|7000|
|570|4296|HL2714|Tablet|5|Cícero|Ramos|10/7/2018|Salvador|1600|NaN|8000|
|571|4305|HL1918|iPhone|3|Bruna|Soares|11/23/2018|Salvador|5300|NaN|15900|
|572|4306|HL1918|iPhone|4|Thayane|Resende|7/26/2018|Salvador|5300|NaN|21200|
|573|4308|HL7348|SmartWatch|4|Gabriel|Thoni|7/31/2018|Salvador|1400|NaN|5600|
|574|4309|HL1918|iPhone|4|Rafaela|Feio|6/4/2018|Salvador|5300|NaN|21200|
|575|4321|HL4379|Televisão|1|Jeferson|Costa|1/2/2018|Salvador|2500|NaN|2500|
|576|4335|HL1918|iPhone|5|Bruna|Ramos|10/11/2018|Salvador|5300|NaN|26500|
|577|4340|HL7348|SmartWatch|2|Guilherme|Monteiro|10/27/2018|Salvador|1400|NaN|2800|
|578|4347|HL2714|Tablet|5|Bruno|Oliveira|2/26/2018|Salvador|1600|NaN|8000|
|579|4348|HL1148|Câmera|5|Bernardo|Botelho|9/24/2018|Salvador|2100|NaN|10500|
|580|4366|HL1918|iPhone|3|Jorge|Carvalho|7/28/2018|Salvador|5300|NaN|15900|
|581|4378|HL1918|iPhone|5|Caio|Ferreira|3/19/2018|Salvador|5300|NaN|26500|
|582|4385|HL9962|Android|3|Eric|Júnior|4/28/2018|Salvador|3400|NaN|10200|
|583|4390|HL9962|Android|1|Fabio|Ramos|8/4/2018|Salvador|3400|NaN|3400|
|584|4397|HL4379|Televisão|4|Luã|Sá|4/16/2018|Salvador|2500|NaN|10000|
|585|4419|HL1918|iPhone|3|Luísa|Fonseca|8/23/2018|Salvador|5300|NaN|15900|
|586|4456|HL8851|Notebook|1|Lucas|Fontoura|12/13/2018|Salvador|3500|NaN|3500|
|587|4459|HL8851|Notebook|3|Lara|Moreira|11/16/2018|Salvador|3500|NaN|10500|
|588|4476|HL2714|Tablet|3|Maike|Pereira|7/2/2018|Salvador|1600|NaN|4800|
|589|4498|HL1918|iPhone|2|Juliana|Barreira|4/19/2018|Salvador|5300|NaN|10600|
|590|4521|HL4379|Televisão|5|Bernardo|Soares|11/23/2018|Salvador|2500|NaN|12500|
|591|4532|HL1918|iPhone|4|Isabelle|Firmino|11/11/2018|Salvador|5300|NaN|21200|
|592|4536|HL1918|iPhone|1|Julia|Silva|8/16/2018|Salvador|5300|NaN|5300|
|593|4547|HL7348|SmartWatch|5|Marcelo|Pereira|12/11/2018|Salvador|1400|NaN|7000|
|594|4555|HL4379|Televisão|5|Bruno|Velucci|10/11/2018|Salvador|2500|NaN|12500|
|595|4564|HL1918|iPhone|4|Itai|Puntel|7/15/2018|Salvador|5300|NaN|21200|
|596|4565|HL1918|iPhone|3|Karina|Camara|8/29/2018|Salvador|5300|NaN|15900|
|597|4566|HL1918|iPhone|4|Rafael|Guimarães|6/1/2018|Salvador|5300|NaN|21200|
|598|4570|HL4379|Televisão|1|Lívia|Marques|9/2/2018|Salvador|2500|NaN|2500|
|599|4578|HL1918|iPhone|3|Juliana|Hollander|10/23/2018|Salvador|5300|NaN|15900|
|600|4580|HL1148|Câmera|5|Thais|Rodrigues|1/13/2018|Salvador|2100|NaN|10500|
|601|4582|HL1918|iPhone|3|Larissa|Cruz|4/10/2018|Salvador|5300|NaN|15900|
|602|4589|HL2714|Tablet|2|Vivianne|Rodrigues|4/23/2018|Salvador|1600|NaN|3200|
|603|4608|HL1918|iPhone|4|Cézar|Santos|4/13/2018|Salvador|5300|NaN|21200|
|604|4611|HL2714|Tablet|3|Beatriz|Biase|9/13/2018|Salvador|1600|NaN|4800|
|605|4616|HL4379|Televisão|2|Gustavo|Aragão|4/7/2018|Salvador|2500|NaN|5000|
|606|4623|HL7348|SmartWatch|5|Antonio|Manhães|9/2/2018|Salvador|1400|NaN|7000|
|607|4628|HL4379|Televisão|4|Guilherme|Castilho|3/17/2018|Salvador|2500|NaN|10000|
|608|4639|HL1148|Câmera|3|Lucas|Baptista|11/17/2018|Salvador|2100|NaN|6300|
|609|4640|HL1918|iPhone|3|Fabio|Ramos|1/29/2018|Salvador|5300|NaN|15900|
|610|4648|HL9962|Android|1|Fernanda|Silva|2/2/2018|Salvador|3400|NaN|3400|
|611|4651|HL9962|Android|5|Natalia|Andrade|5/1/2018|Salvador|3400|NaN|17000|
|612|4653|HL7348|SmartWatch|3|Lucas|Baptista|9/11/2018|Salvador|1400|NaN|4200|
|613|4656|HL7348|SmartWatch|5|Diogo|Peixoto|5/29/2018|Salvador|1400|NaN|7000|
|614|4657|HL2714|Tablet|4|Luiza|Procaci|11/30/2018|Salvador|1600|NaN|6400|
|615|4658|HL1918|iPhone|2|Alex|Fernandes|6/9/2018|Salvador|5300|NaN|10600|
|616|4660|HL1918|iPhone|4|Priscila|Vogel|2/12/2018|Salvador|5300|NaN|21200|
|617|4662|HL8851|Notebook|3|Bruna|Silveira|2/25/2018|Salvador|3500|NaN|10500|
|618|4668|HL8851|Notebook|2|Yasser|Calbucci|4/7/2018|Salvador|3500|NaN|7000|
|619|4669|HL1918|iPhone|4|Stefan|Nunes|8/17/2018|Salvador|5300|NaN|21200|
|620|4671|HL8851|Notebook|3|Luíza|Goulart|12/1/2018|Salvador|3500|NaN|10500|
|621|4672|HL7348|SmartWatch|1|Tadeu|Sousa|2/25/2018|Salvador|1400|NaN|1400|
|622|4694|HL1918|iPhone|5|Bruna|Brandao|9/18/2018|Salvador|5300|NaN|26500|
|623|4702|HL2714|Tablet|3|Amanda|Felippe|3/25/2018|Salvador|1600|NaN|4800|
|624|4704|HL1918|iPhone|5|João|Monteiro|10/14/2018|Salvador|5300|NaN|26500|
|625|4712|HL1918|iPhone|2|Isabela|Resende|12/1/2018|Salvador|5300|NaN|10600|
|626|4736|HL1918|iPhone|2|Raísa|Rodrigues|7/27/2018|Salvador|5300|NaN|10600|
|627|4750|HL1148|Câmera|1|Jéssica|Stefanelli|5/13/2018|Salvador|2100|NaN|2100|
|628|4761|HL4379|Televisão|2|Larissa|Florim|6/19/2018|Salvador|2500|NaN|5000|
|629|4775|HL9962|Android|3|Gabrielle|Silva|5/12/2018|Salvador|3400|NaN|10200|
|630|4777|HL1918|iPhone|1|Yasmim|Bittencourt|7/15/2018|Salvador|5300|NaN|5300|
|631|4783|HL2714|Tablet|5|Pedro|Sena|11/21/2018|Salvador|1600|NaN|8000|
|632|4790|HL7348|SmartWatch|5|Gabrielle|Wanderley|9/11/2018|Salvador|1400|NaN|7000|
|633|4803|HL4379|Televisão|4|Rafaela|Rodrigues|9/8/2018|Salvador|2500|NaN|10000|
|634|4806|HL7348|SmartWatch|2|Isabelle|Gonçalves|11/21/2018|Salvador|1400|NaN|2800|
|635|4815|HL1918|iPhone|4|Maria|Junior|7/12/2018|Salvador|5300|NaN|21200|
|636|4824|HL4379|Televisão|2|Mariana|Sousa|4/24/2018|Salvador|2500|NaN|5000|
|637|4827|HL2714|Tablet|2|Tayla|Lima|9/29/2018|Salvador|1600|NaN|3200|
|638|4837|HL1918|iPhone|1|Paula|Isbelle|11/8/2018|Salvador|5300|NaN|5300|
|639|4854|HL4379|Televisão|5|Mateus|Duque|12/27/2018|Salvador|2500|NaN|12500|
|640|4859|HL7348|SmartWatch|5|Guilherme|Vianna|12/13/2018|Salvador|1400|NaN|7000|
|641|4861|HL9962|Android|2|Leonardo|Faria|6/4/2018|Salvador|3400|NaN|6800|
|642|4865|HL1918|iPhone|5|Renan|Nascimento|6/22/2018|Salvador|5300|NaN|26500|
|643|4876|HL1918|iPhone|2|Jessica|Ferreira|11/7/2018|Salvador|5300|NaN|10600|
|644|4882|HL1918|iPhone|2|Bruno|Souza|8/10/2018|Salvador|5300|NaN|10600|
|645|4888|HL1148|Câmera|1|Isabella|Montanholi|5/8/2018|Salvador|2100|NaN|2100|
|646|4890|HL1918|iPhone|4|Rafaela|Ferreira|11/20/2018|Salvador|5300|NaN|21200|
|647|4897|HL1918|iPhone|1|Jackson|Derossi|12/27/2018|Salvador|5300|NaN|5300|
|648|4900|HL1918|iPhone|4|Clara|Silveira|12/14/2018|Salvador|5300|NaN|21200|
|649|4903|HL2714|Tablet|4|Viviane|Souza|9/16/2018|Salvador|1600|NaN|6400|
|650|4908|HL9962|Android|5|Adriana|Passos|10/14/2018|Salvador|3400|NaN|17000|
|651|4918|HL1918|iPhone|3|Priscila|Suzano|10/9/2018|Salvador|5300|NaN|15900|
|652|4930|HL2714|Tablet|4|Juliana|Correa|12/4/2018|Salvador|1600|NaN|6400|
|653|4941|HL1918|iPhone|5|Luis|Oliveira|2/4/2018|Salvador|5300|NaN|26500|
|654|4952|HL1148|Câmera|1|Isabela|Rodrigues|4/1/2018|Salvador|2100|NaN|2100|
|655|4957|HL2714|Tablet|5|Thaís|Ribeiro|12/25/2018|Salvador|1600|NaN|8000|
|656|4967|HL4379|Televisão|4|Gabriel|Rubim|9/16/2018|Salvador|2500|NaN|10000|
|657|4970|HL8851|Notebook|5|Myllena|Carneiro|1/29/2018|Salvador|3500|NaN|17500|
|658|4984|HL4379|Televisão|3|Paula|Cavalcanti|5/27/2018|Salvador|2500|NaN|7500|
|659|4989|HL7348|SmartWatch|4|Thiago|Costa|1/17/2018|Salvador|1400|NaN|5600|
|660|5001|HL2714|Tablet|4|Matheus|Gomes|6/10/2018|Salvador|1600|NaN|6400|
|661|5020|HL4379|Televisão|5|Juliana|Goes|8/12/2018|Salvador|2500|NaN|12500|
|662|5028|HL2714|Tablet|4|Laura|Araujo|8/7/2018|Salvador|1600|NaN|6400|
|663|5040|HL1148|Câmera|2|Matheus|Gomes|7/10/2018|Salvador|2100|NaN|4200|
|664|5047|HL2714|Tablet|5|Luiz|Freire|9/13/2018|Salvador|1600|NaN|8000|
|665|5050|HL9962|Android|2|Raíssa|Oros|1/2/2018|Salvador|3400|NaN|6800|
|666|5055|HL7348|SmartWatch|2|Deysiane|Medronho|4/9/2018|Salvador|1400|NaN|2800|
|667|5058|HL1918|iPhone|2|Carolina|Alfradique|1/9/2018|Salvador|5300|NaN|10600|
|668|5072|HL9962|Android|1|Lívia|Tanaka|6/23/2018|Salvador|3400|NaN|3400|
|669|5074|HL8851|Notebook|5|Fernanda|Junior|7/16/2018|Salvador|3500|NaN|17500|
|670|5079|HL8851|Notebook|1|Marcelo|Rosa|7/23/2018|Salvador|3500|NaN|3500|
|671|5080|HL1918|iPhone|1|Luiza|Cavalcanti|3/4/2018|Salvador|5300|NaN|5300|
|672|5096|HL9962|Android|2|Yasser|Calbucci|8/13/2018|Salvador|3400|NaN|6800|
|673|5101|HL4379|Televisão|3|Ravena|Bhering|12/16/2018|Salvador|2500|NaN|7500|
|674|5112|HL1918|iPhone|3|Nina|Magalhães|9/4/2018|Salvador|5300|NaN|15900|
|675|5114|HL1918|iPhone|5|Julia|Aliani|7/21/2018|Salvador|5300|NaN|26500|
|676|5120|HL8851|Notebook|5|Alon|Palmeira|8/10/2018|Salvador|3500|NaN|17500|
|677|5124|HL1918|iPhone|4|Rafaela|Ferreira|7/31/2018|Salvador|5300|NaN|21200|
|678|5129|HL1148|Câmera|2|Ramon|Araujo|2/18/2018|Salvador|2100|NaN|4200|
|679|5145|HL7348|SmartWatch|5|Carolina|Santos|12/9/2018|Salvador|1400|NaN|7000|
|680|5156|HL8851|Notebook|2|Ana|Felippe|11/5/2018|Salvador|3500|NaN|7000|
|681|5162|HL1918|iPhone|5|Letícia|Rodrigues|10/21/2018|Salvador|5300|NaN|26500|
|682|5175|HL2714|Tablet|4|Anna|Maia|1/29/2018|Salvador|1600|NaN|6400|
|683|5176|HL9962|Android|1|Aline|Mello|3/26/2018|Salvador|3400|NaN|3400|
|684|5177|HL8851|Notebook|5|Lázaro|Villanova|11/13/2018|Salvador|3500|NaN|17500|
|685|5180|HL1918|iPhone|1|Raissa|Negrelli|7/10/2018|Salvador|5300|NaN|5300|
|686|5183|HL1918|iPhone|4|Guilherme|Lima|2/13/2018|Salvador|5300|NaN|21200|
|687|5189|HL4379|Televisão|5|Patrícia|Amaral|6/4/2018|Salvador|2500|NaN|12500|
|688|5199|HL2714|Tablet|4|Pedro|Ferrari|1/27/2018|Salvador|1600|NaN|6400|
|689|5205|HL1918|iPhone|2|Jessica|Cordovil|6/11/2018|Salvador|5300|NaN|10600|
|690|5206|HL7348|SmartWatch|4|Gabriel|Puntel|2/17/2018|Salvador|1400|NaN|5600|
|691|5208|HL9962|Android|4|Danilo|Rubim|8/27/2018|Salvador|3400|NaN|13600|
|692|5234|HL1918|iPhone|2|Rodrigo|Silva|11/18/2018|Salvador|5300|NaN|10600|
|693|5246|HL2714|Tablet|5|Rilson|Guedes|4/3/2018|Salvador|1600|NaN|8000|
|694|5247|HL4379|Televisão|2|Bernardo|Borges|2/25/2018|Salvador|2500|NaN|5000|
|695|5265|HL1918|iPhone|2|Alon|Pestana|7/5/2018|Salvador|5300|NaN|10600|
|696|5274|HL4379|Televisão|1|Raissa|Sales|6/22/2018|Salvador|2500|NaN|2500|
|697|5276|HL8851|Notebook|1|Arthur|Fernandes|5/24/2018|Salvador|3500|NaN|3500|
|698|5285|HL8851|Notebook|4|Joyce|Souza|11/24/2018|Salvador|3500|NaN|14000|
|699|5328|HL7348|SmartWatch|5|Raphael|Mattos|1/2/2018|Salvador|1400|NaN|7000|
|700|5331|HL2714|Tablet|5|Adrielle|Vieira|3/16/2018|Salvador|1600|NaN|8000|
|701|5335|HL7348|SmartWatch|5|Lázaro|Nascimento|3/22/2018|Salvador|1400|NaN|7000|
|702|5337|HL1918|iPhone|3|Luiz|Almeida|3/20/2018|Salvador|5300|NaN|15900|
|703|5353|HL1918|iPhone|5|Bruna|Silva|3/2/2018|Salvador|5300|NaN|26500|
|704|5365|HL1918|iPhone|1|Thayna|Martins|5/13/2018|Salvador|5300|NaN|5300|
|705|5371|HL1918|iPhone|2|João|Araujo|5/16/2018|Salvador|5300|NaN|10600|
|706|5374|HL1918|iPhone|5|Giulia|Pessanha|3/10/2018|Salvador|5300|NaN|26500|
|707|5384|HL9962|Android|4|Célio|Xavier|3/18/2018|Salvador|3400|NaN|13600|
|708|5390|HL1918|iPhone|1|Michelle|Pereira|12/24/2018|Salvador|5300|NaN|5300|
|709|5395|HL1918|iPhone|1|Ives|Pinheiro|8/22/2018|Salvador|5300|NaN|5300|
|710|5407|HL9962|Android|2|Izabel|Lopes|1/6/2018|Salvador|3400|NaN|6800|
|711|5431|HL1918|iPhone|3|João|Silva|12/20/2018|Salvador|5300|NaN|15900|
|712|5434|HL1918|iPhone|3|Matheus|Afonso|5/15/2018|Salvador|5300|NaN|15900|
|713|5442|HL2714|Tablet|2|Yasmim|Bittencourt|2/6/2018|Salvador|1600|NaN|3200|
|714|5447|HL4379|Televisão|4|Luíza|Garcia|9/16/2018|Salvador|2500|NaN|10000|
|715|5457|HL4379|Televisão|5|Felipe|Cavalcanti|4/11/2018|Salvador|2500|NaN|12500|
|716|5460|HL1148|Câmera|5|Beatriz|Almeida|11/18/2018|Salvador|2100|NaN|10500|
|717|5464|HL1918|iPhone|3|Bruna|Gomes|9/22/2018|Salvador|5300|NaN|15900|
|718|5472|HL1148|Câmera|4|Luiz|Almeida|5/15/2018|Salvador|2100|NaN|8400|
|719|5474|HL8851|Notebook|4|Pedro|Ferrari|4/24/2018|Salvador|3500|NaN|14000|
|720|5484|HL9962|Android|4|José|Jesus|7/9/2018|Salvador|3400|NaN|13600|
|721|5497|HL1918|iPhone|3|Nicolas|Monteiro|3/27/2018|Salvador|5300|NaN|15900|
|722|5500|HL8851|Notebook|1|Camille|Silva|4/17/2018|Salvador|3500|NaN|3500|
|723|5510|HL1918|iPhone|5|Rafael|Ramos|12/24/2018|Salvador|5300|NaN|26500|
|724|5512|HL4379|Televisão|4|Marcelo|Magalhães|7/5/2018|Salvador|2500|NaN|10000|
|725|5513|HL7348|SmartWatch|1|Daniela|Rosa|6/17/2018|Salvador|1400|NaN|1400|
|726|5514|HL4379|Televisão|3|Thiago|Costa|1/25/2018|Salvador|2500|NaN|7500|
|727|5558|HL1918|iPhone|2|Bruna|Gomes|4/28/2018|Salvador|5300|NaN|10600|
|728|5562|HL1918|iPhone|2|José|Seixas|10/25/2018|Salvador|5300|NaN|10600|
|729|5564|HL8851|Notebook|5|Ana|Monte|3/21/2018|Salvador|3500|NaN|17500|
|730|5567|HL1148|Câmera|5|Luana|Santana|12/24/2018|Salvador|2100|NaN|10500|
|731|5571|HL4379|Televisão|1|Maria|Junior|7/30/2018|Salvador|2500|NaN|2500|
|732|5573|HL4379|Televisão|3|Stephanie|Gonçalves|3/26/2018|Salvador|2500|NaN|7500|
|733|5582|HL1148|Câmera|2|Rebeca|Manhães|7/16/2018|Salvador|2100|NaN|4200|
|734|5598|HL2714|Tablet|5|Ana|Gomes|3/5/2018|Salvador|1600|NaN|8000|
|735|5608|HL1918|iPhone|5|Felipe|Freitas|12/20/2018|Salvador|5300|NaN|26500|
|736|5610|HL9962|Android|3|Beatriz|Santos|10/11/2018|Salvador|3400|NaN|10200|
|737|5613|HL1148|Câmera|3|Roberta|Pimenta|9/17/2018|Salvador|2100|NaN|6300|
|738|5627|HL9962|Android|4|Renan|Nucci|7/14/2018|Salvador|3400|NaN|13600|
|739|5630|HL9962|Android|2|Marcelo|Borges|2/15/2018|Salvador|3400|NaN|6800|
|740|5640|HL1918|iPhone|2|Pedro|Sena|3/4/2018|Salvador|5300|NaN|10600|
|741|5645|HL2714|Tablet|2|Gabriel|Almeida|7/9/2018|Salvador|1600|NaN|3200|
|742|5651|HL1918|iPhone|2|Bruno|Silva|11/18/2018|Salvador|5300|NaN|10600|
|743|5653|HL1918|iPhone|3|Eduardo|Ferreira|12/2/2018|Salvador|5300|NaN|15900|
|744|5666|HL7348|SmartWatch|1|Letícia|Rodrigues|4/23/2018|Salvador|1400|NaN|1400|
|745|5677|HL9962|Android|3|Felipe|Paulo|4/10/2018|Salvador|3400|NaN|10200|
|746|5681|HL1148|Câmera|1|Vivianne|Rodrigues|1/28/2018|Salvador|2100|NaN|2100|
|747|5682|HL1918|iPhone|2|Cícero|Lima|11/10/2018|Salvador|5300|NaN|10600|
|748|5686|HL4379|Televisão|4|João|Junior|9/22/2018|Salvador|2500|NaN|10000|
|749|5695|HL1918|iPhone|1|Bianca|Procaci|5/10/2018|Salvador|5300|NaN|5300|
|750|5725|HL4379|Televisão|3|Bruno|Oliveira|9/1/2018|Salvador|2500|NaN|7500|
|751|5727|HL8851|Notebook|5|Eduardo|Peluzo|5/25/2018|Salvador|3500|NaN|17500|
|752|5733|HL9962|Android|5|Eduardo|Vargas|7/17/2018|Salvador|3400|NaN|17000|
|753|5752|HL1918|iPhone|2|Julia|Figueiredo|4/15/2018|Salvador|5300|NaN|10600|
|754|5762|HL9962|Android|4|Eduardo|Ferreira|10/19/2018|Salvador|3400|NaN|13600|
|755|5768|HL9962|Android|3|Guilherme|Merotto|9/3/2018|Salvador|3400|NaN|10200|
|756|5774|HL1918|iPhone|2|Michelle|Pereira|6/6/2018|Salvador|5300|NaN|10600|
|757|5784|HL9962|Android|1|Willian|Albino|7/30/2018|Salvador|3400|NaN|3400|
|758|5793|HL4379|Televisão|2|Lorena|Kohn|5/26/2018|Salvador|2500|NaN|5000|
|759|5799|HL9962|Android|4|Carolina|Costa|6/4/2018|Salvador|3400|NaN|13600|
|760|5803|HL7348|SmartWatch|1|Priscila|Garcia|9/11/2018|Salvador|1400|NaN|1400|
|761|5804|HL8851|Notebook|3|Priscila|Carvalho|6/24/2018|Salvador|3500|NaN|10500|
|762|5805|HL8851|Notebook|5|Caio|Silva|12/1/2018|Salvador|3500|NaN|17500|
|763|5810|HL4379|Televisão|2|Renan|Cunha|11/12/2018|Salvador|2500|NaN|5000|
|764|5811|HL1918|iPhone|1|Lucas|Freitas|6/10/2018|Salvador|5300|NaN|5300|
|765|5819|HL8851|Notebook|2|Carlos|Barbosa|4/23/2018|Salvador|3500|NaN|7000|
|766|5843|HL2714|Tablet|4|Luiza|Farias|8/13/2018|Salvador|1600|NaN|6400|
|767|5858|HL9962|Android|5|Isabela|Resende|3/25/2018|Salvador|3400|NaN|17000|
|768|5861|HL1918|iPhone|2|Pedro|Cardoso|1/10/2018|Salvador|5300|NaN|10600|
|769|5876|HL1918|iPhone|5|Miguel|Carneiro|2/21/2018|Salvador|5300|NaN|26500|
|770|5885|HL8851|Notebook|3|Júlia|Almeida|1/16/2018|Salvador|3500|NaN|10500|
|771|5891|HL4379|Televisão|1|Victor|Gomes|7/20/2018|Salvador|2500|NaN|2500|
|772|5898|HL7348|SmartWatch|1|Pedro|Ronfini|5/5/2018|Salvador|1400|NaN|1400|
|773|5899|HL1918|iPhone|3|Marcela|Gasperi|10/22/2018|Salvador|5300|NaN|15900|
|774|5912|HL7348|SmartWatch|1|Rodrigo|Alves|5/21/2018|Salvador|1400|NaN|1400|
|775|5918|HL1918|iPhone|1|Bruno|Silva|4/9/2018|Salvador|5300|NaN|5300|
|776|5923|HL1148|Câmera|1|Cícero|Ramos|7/3/2018|Salvador|2100|NaN|2100|
|777|5938|HL1918|iPhone|2|Julia|Penteado|9/14/2018|Salvador|5300|NaN|10600|
|778|5941|HL1918|iPhone|1|Elena|Barreto|12/26/2018|Salvador|5300|NaN|5300|
|779|5946|HL2714|Tablet|1|Lucas|Araújo|5/6/2018|Salvador|1600|NaN|1600|
|780|5949|HL9962|Android|1|Chan|Santos|2/1/2018|Salvador|3400|NaN|3400|
|781|5953|HL8851|Notebook|3|Rodrigo|Silva|8/5/2018|Salvador|3500|NaN|10500|
|782|5955|HL4379|Televisão|4|Bruno|Souza|3/5/2018|Salvador|2500|NaN|10000|
|783|5957|HL4379|Televisão|3|Maria|Gasperi|6/5/2018|Salvador|2500|NaN|7500|
|784|5959|HL1918|iPhone|4|Fabio|Ramos|7/28/2018|Salvador|5300|NaN|21200|
|785|5974|HL4379|Televisão|4|Rilson|Guedes|5/17/2018|Salvador|2500|NaN|10000|
|786|5978|HL1918|iPhone|5|Ananda|Dias|8/27/2018|Salvador|5300|NaN|26500|
|787|5989|HL7348|SmartWatch|2|Felipe|Mendonça|11/11/2018|Salvador|1400|NaN|2800|
|788|5992|HL1918|iPhone|4|Fernanda|Bhering|4/16/2018|Salvador|5300|NaN|21200|
|789|5994|HL8851|Notebook|1|Gustavo|Guimarães|8/13/2018|Salvador|3500|NaN|3500|
|790|6003|HL1148|Câmera|4|Marcela|Medeiros|8/2/2018|Salvador|2100|NaN|8400|
|791|6005|HL1918|iPhone|3|Marina|Delgado|9/21/2018|Salvador|5300|NaN|15900|
|792|6017|HL8851|Notebook|2|Lucas|Reis|6/21/2018|Salvador|3500|NaN|7000|
|793|6019|HL1148|Câmera|5|Raíza|Lopes|7/4/2018|Salvador|2100|NaN|10500|
|794|6030|HL4379|Televisão|5|David|Campelo|4/4/2018|Salvador|2500|NaN|12500|
|795|6043|HL1918|iPhone|2|Raphael|Kurtz|8/21/2018|Salvador|5300|NaN|10600|
|796|6045|HL2714|Tablet|5|Carolina|Carneiro|6/13/2018|Salvador|1600|NaN|8000|
|797|6047|HL9962|Android|5|Camila|Bastazini|3/29/2018|Salvador|3400|NaN|17000|
|798|6054|HL9962|Android|2|Maria|Costa|12/9/2018|Salvador|3400|NaN|6800|
|799|6057|HL4379|Televisão|2|Lenon|Fernandes|9/3/2018|Salvador|2500|NaN|5000|
|800|6070|HL4379|Televisão|3|Lucas|Junior|7/1/2018|Salvador|2500|NaN|7500|
|801|6087|HL1148|Câmera|2|Platini|Heimlich|4/3/2018|Salvador|2100|NaN|4200|
|802|6088|HL1918|iPhone|3|Carla|Zakhm|6/27/2018|Salvador|5300|NaN|15900|
|803|6091|HL7348|SmartWatch|4|João|Peçanha|2/3/2018|Salvador|1400|NaN|5600|
|804|6097|HL7348|SmartWatch|3|Allan|Guedes|1/7/2018|Salvador|1400|NaN|4200|
|805|6101|HL8851|Notebook|5|Cassio|Faria|3/21/2018|Salvador|3500|NaN|17500|
|806|6117|HL1918|iPhone|1|Victoria|Mazza|10/30/2018|Salvador|5300|NaN|5300|
|807|6132|HL8851|Notebook|3|Bruno|Silva|3/11/2018|Salvador|3500|NaN|10500|
|808|6142|HL1918|iPhone|5|Tadeu|Nakayama|7/23/2018|Salvador|5300|NaN|26500|
|809|6143|HL2714|Tablet|4|Lucas|Assunção|10/22/2018|Salvador|1600|NaN|6400|
|810|6146|HL1918|iPhone|5|Caio|Fernandes|1/17/2018|Salvador|5300|NaN|26500|
|811|6149|HL1918|iPhone|5|Rafael|Wajnsztok|7/7/2018|Salvador|5300|NaN|26500|
|812|6157|HL1918|iPhone|3|Gabriel|Assis|2/11/2018|Salvador|5300|NaN|15900|
|813|6162|HL1918|iPhone|4|Daniel|Sousa|12/24/2018|Salvador|5300|NaN|21200|
|814|6170|HL7348|SmartWatch|1|Júlio|Freire|3/26/2018|Salvador|1400|NaN|1400|
|815|6173|HL1918|iPhone|5|Julia|Leig|2/27/2018|Salvador|5300|NaN|26500|
|816|6182|HL4379|Televisão|1|João|Monteiro|11/7/2018|Salvador|2500|NaN|2500|
|817|6188|HL4379|Televisão|5|Mariana|Miranda|2/24/2018|Salvador|2500|NaN|12500|
|818|6195|HL1918|iPhone|5|Adrielle|Gabriel|2/17/2018|Salvador|5300|NaN|26500|
|819|6197|HL1918|iPhone|2|Giuseppe|Borges|10/28/2018|Salvador|5300|NaN|10600|
|820|6201|HL9962|Android|1|Wendela|Mariz|10/30/2018|Salvador|3400|NaN|3400|
|821|6209|HL1148|Câmera|5|Khaio|Mesquita|3/5/2018|Salvador|2100|NaN|10500|
|822|6210|HL9962|Android|3|Breno|Costa|8/4/2018|Salvador|3400|NaN|10200|
|823|6212|HL1148|Câmera|2|Ana|Felippe|5/15/2018|Salvador|2100|NaN|4200|
|824|6216|HL1918|iPhone|5|Alon|Pestana|3/9/2018|Salvador|5300|NaN|26500|
|825|6223|HL9962|Android|5|Matheus|Gomes|7/17/2018|Salvador|3400|NaN|17000|
|826|6224|HL8851|Notebook|1|Fabio|Sepúlveda|5/25/2018|Salvador|3500|NaN|3500|
|827|6234|HL1918|iPhone|3|Lívia|Marques|1/15/2018|Salvador|5300|NaN|15900|
|828|6239|HL9962|Android|4|Victor|Ferreira|5/11/2018|Salvador|3400|NaN|13600|
|829|6258|HL8851|Notebook|1|Thomáz|Bôas|1/21/2018|Salvador|3500|NaN|3500|
|830|6261|HL1148|Câmera|2|Raíza|Lopes|3/17/2018|Salvador|2100|NaN|4200|
|831|6264|HL4379|Televisão|5|Amanda|Machado|8/7/2018|Salvador|2500|NaN|12500|
|832|6269|HL1918|iPhone|4|Rafael|Portela|10/20/2018|Salvador|5300|NaN|21200|
|833|6270|HL7348|SmartWatch|1|Michelle|Figueiredo|7/2/2018|Salvador|1400|NaN|1400|
|834|6310|HL1148|Câmera|1|Thomáz|Vannier|2/7/2018|Salvador|2100|NaN|2100|
|835|6312|HL1918|iPhone|4|Maria|Correa|11/14/2018|Salvador|5300|NaN|21200|
|836|6314|HL2714|Tablet|1|Kimberly|Sad|2/9/2018|Salvador|1600|NaN|1600|
|837|6344|HL4379|Televisão|1|Hiaiune|Valim|5/10/2018|Salvador|2500|NaN|2500|
|838|6347|HL2714|Tablet|5|Leandro|Ferreira|2/25/2018|Salvador|1600|NaN|8000|
|839|6362|HL2714|Tablet|4|Beatriz|Nogueira|10/8/2018|Salvador|1600|NaN|6400|
|840|6372|HL7348|SmartWatch|2|Gustavo|Azevedo|5/18/2018|Salvador|1400|NaN|2800|
|841|6383|HL4379|Televisão|1|Wellington|Duarte|11/29/2018|Salvador|2500|NaN|2500|
|842|6389|HL1918|iPhone|5|Maria|Assumpção|8/17/2018|Salvador|5300|NaN|26500|
|843|6390|HL1918|iPhone|1|David|Vasconcelos|7/19/2018|Salvador|5300|NaN|5300|
|844|6395|HL1918|iPhone|1|Ana|Almeida|3/28/2018|Salvador|5300|NaN|5300|
|845|6399|HL1148|Câmera|4|Eduardo|Vargas|7/17/2018|Salvador|2100|NaN|8400|
|846|6429|HL7348|SmartWatch|3|Luiz|Freire|6/21/2018|Salvador|1400|NaN|4200|
|847|6440|HL1918|iPhone|3|Vitor|Arruda|11/27/2018|Salvador|5300|NaN|15900|
|848|6441|HL2714|Tablet|4|Adriane|Gomes|4/12/2018|Salvador|1600|NaN|6400|
|849|6445|HL1918|iPhone|4|Leandro|Melo|11/13/2018|Salvador|5300|NaN|21200|
|850|6451|HL1918|iPhone|4|Amanda|Felippe|12/18/2018|Salvador|5300|NaN|21200|
|851|6458|HL1918|iPhone|2|Carlos|Cardoso|6/17/2018|Salvador|5300|NaN|10600|
|852|6462|HL1918|iPhone|4|Hiaiune|Valim|6/2/2018|Salvador|5300|NaN|21200|
|853|6479|HL2714|Tablet|3|Adriane|Chagas|5/15/2018|Salvador|1600|NaN|4800|
|854|6483|HL1148|Câmera|1|Stephanie|Novak|7/29/2018|Salvador|2100|NaN|2100|
|855|6491|HL4379|Televisão|4|Luis|Villanova|6/8/2018|Salvador|2500|NaN|10000|
|856|6510|HL9962|Android|3|Tadeu|Nakayama|12/13/2018|Salvador|3400|NaN|10200|
|857|6512|HL9962|Android|5|Gabriel|Almeida|5/2/2018|Salvador|3400|NaN|17000|
|858|6514|HL4379|Televisão|1|Beatriz|Silva|12/22/2018|Salvador|2500|NaN|2500|
|859|6520|HL1918|iPhone|5|Thomáz|Bôas|7/2/2018|Salvador|5300|NaN|26500|
|860|6526|HL4379|Televisão|1|João|Costa|1/29/2018|Salvador|2500|NaN|2500|
|861|6527|HL1918|iPhone|1|Luis|Souza|2/1/2018|Salvador|5300|NaN|5300|
|862|6545|HL8851|Notebook|5|Caio|Moraes|6/19/2018|Salvador|3500|NaN|17500|
|863|6549|HL4379|Televisão|4|Karine|Barros|8/30/2018|Salvador|2500|NaN|10000|
|864|6560|HL4379|Televisão|3|Silvio|Provenzano|11/13/2018|Salvador|2500|NaN|7500|
|865|6580|HL9962|Android|3|Carolina|Alfradique|6/12/2018|Salvador|3400|NaN|10200|
|866|6606|HL1148|Câmera|3|Lucas|Valim|7/21/2018|Salvador|2100|NaN|6300|
|867|6617|HL9962|Android|5|Luíza|Garcia|1/24/2018|Salvador|3400|NaN|17000|
|868|6629|HL7348|SmartWatch|4|Júlia|Almeida|4/24/2018|Salvador|1400|NaN|5600|
|869|6641|HL7348|SmartWatch|4|Amanda|Procaci|1/20/2018|Salvador|1400|NaN|5600|
|870|6645|HL8851|Notebook|3|Manuela|Merege|11/14/2018|Salvador|3500|NaN|10500|
|871|6657|HL1148|Câmera|3|Rafael|Wajnsztok|8/26/2018|Salvador|2100|NaN|6300|
|872|6662|HL1148|Câmera|3|Yasmim|Bittencourt|10/30/2018|Salvador|2100|NaN|6300|
|873|6665|HL1918|iPhone|2|Igor|Lima|4/5/2018|Salvador|5300|NaN|10600|
|874|6694|HL1918|iPhone|5|Adrielle|Gabriel|6/3/2018|Salvador|5300|NaN|26500|
|875|6696|HL8851|Notebook|2|Beatriz|Nogueira|12/5/2018|Salvador|3500|NaN|7000|
|876|6708|HL9962|Android|3|Luíza|Melo|4/20/2018|Salvador|3400|NaN|10200|
|877|6710|HL1918|iPhone|5|Gabriel|Rocha|1/28/2018|Salvador|5300|NaN|26500|
|878|6711|HL9962|Android|2|Luiza|Cabral|2/1/2018|Salvador|3400|NaN|6800|
|879|6712|HL2714|Tablet|4|Lucas|Almeida|6/14/2018|Salvador|1600|NaN|6400|
|880|6719|HL2714|Tablet|5|Letícia|Rodrigues|7/4/2018|Salvador|1600|NaN|8000|
|881|6731|HL4379|Televisão|1|Lucas|Assunção|8/29/2018|Salvador|2500|NaN|2500|
|882|6734|HL1918|iPhone|4|Gabriel|Brito|5/20/2018|Salvador|5300|NaN|21200|
|883|6738|HL7348|SmartWatch|3|Wilson|Vianna|5/11/2018|Salvador|1400|NaN|4200|
|884|6750|HL1918|iPhone|1|Lais|Candido|7/8/2018|Salvador|5300|NaN|5300|
|885|6764|HL2714|Tablet|3|Antônio|Soares|4/25/2018|Salvador|1600|NaN|4800|
|886|6768|HL2714|Tablet|4|Pedro|Jorge|12/29/2018|Salvador|1600|NaN|6400|
|887|6770|HL4379|Televisão|5|Wilson|Meirelles|4/24/2018|Salvador|2500|NaN|12500|
|888|6771|HL1918|iPhone|4|Victor|Ferreira|5/19/2018|Salvador|5300|NaN|21200|
|889|6777|HL1148|Câmera|2|Bruna|Gomes|11/22/2018|Salvador|2100|NaN|4200|
|890|6782|HL7348|SmartWatch|5|Guilherme|Seixas|4/19/2018|Salvador|1400|NaN|7000|
|891|6785|HL1918|iPhone|1|Stephanie|Oliveira|4/1/2018|Salvador|5300|NaN|5300|
|892|6787|HL9962|Android|4|Vinícius|Antunes|4/19/2018|Salvador|3400|NaN|13600|
|893|6798|HL7348|SmartWatch|5|Juliana|Silva|3/17/2018|Salvador|1400|NaN|7000|
|894|6806|HL1918|iPhone|4|Mariana|Baptista|8/7/2018|Salvador|5300|NaN|21200|
|895|6808|HL1918|iPhone|4|Alon|Pestana|10/28/2018|Salvador|5300|NaN|21200|
|896|6810|HL2714|Tablet|4|João|Luz|9/6/2018|Salvador|1600|NaN|6400|
|897|6829|HL4379|Televisão|4|Mateus|Franco|8/9/2018|Salvador|2500|NaN|10000|
|898|6833|HL7348|SmartWatch|1|Bruno|Souza|1/2/2018|Salvador|1400|NaN|1400|
|899|6841|HL8851|Notebook|5|Letícia|Rodrigues|10/6/2018|Salvador|3500|NaN|17500|
|900|6846|HL1918|iPhone|5|Marcelo|Guadagnino|4/23/2018|Salvador|5300|NaN|26500|
|901|6848|HL9962|Android|1|João|Bach|10/9/2018|Salvador|3400|NaN|3400|
|902|6851|HL1918|iPhone|5|Carlos|Melo|5/27/2018|Salvador|5300|NaN|26500|
|903|6861|HL7348|SmartWatch|5|Izabel|Miura|12/4/2018|Salvador|1400|NaN|7000|
|904|6862|HL8851|Notebook|4|Lunna|Vannier|4/7/2018|Salvador|3500|NaN|14000|
|905|6869|HL4379|Televisão|5|Lucas|Lacerda|6/28/2018|Salvador|2500|NaN|12500|
|906|6874|HL1918|iPhone|4|Ana|Silva|8/1/2018|Salvador|5300|NaN|21200|
|907|6887|HL1918|iPhone|2|Stefan|Nunes|5/24/2018|Salvador|5300|NaN|10600|
|908|6888|HL1918|iPhone|1|Ana|Soledade|3/1/2018|Salvador|5300|NaN|5300|
|909|6895|HL4379|Televisão|3|Renan|Firmino|8/9/2018|Salvador|2500|NaN|7500|
|910|6904|HL9962|Android|3|Paula|Carneiro|2/18/2018|Salvador|3400|NaN|10200|
|911|6905|HL8851|Notebook|5|Rodrigo|Mendes|12/5/2018|Salvador|3500|NaN|17500|
|912|6908|HL9962|Android|2|Roberto|Tiradentes|8/2/2018|Salvador|3400|NaN|6800|
|913|6913|HL4379|Televisão|4|Jonatas|Passos|7/25/2018|Salvador|2500|NaN|10000|
|914|6916|HL2714|Tablet|2|Matheus|Silva|6/20/2018|Salvador|1600|NaN|3200|
|915|6917|HL2714|Tablet|2|Eduardo|Soares|2/12/2018|Salvador|1600|NaN|3200|
|916|6918|HL7348|SmartWatch|4|Carlos|Barbosa|6/20/2018|Salvador|1400|NaN|5600|
|917|6920|HL1918|iPhone|2|Jéssica|Stefanelli|5/5/2018|Salvador|5300|NaN|10600|
|918|6922|HL2714|Tablet|4|Adriane|Gomes|2/2/2018|Salvador|1600|NaN|6400|
|919|6941|HL1918|iPhone|1|Ulisses|Filho|11/1/2018|Salvador|5300|NaN|5300|
|920|6943|HL7348|SmartWatch|1|Allan|Candido|9/30/2018|Salvador|1400|NaN|1400|
|921|6953|HL2714|Tablet|4|Julia|Leig|9/1/2018|Salvador|1600|NaN|6400|
|922|6962|HL1918|iPhone|5|Caio|Moura|8/11/2018|Salvador|5300|NaN|26500|
|923|6969|HL4379|Televisão|4|Iuri|Neto|10/17/2018|Salvador|2500|NaN|10000|
|924|6979|HL1918|iPhone|5|Livia|Corrêa|11/8/2018|Salvador|5300|NaN|26500|
|925|6980|HL4379|Televisão|5|Pedro|Rodrigues|1/10/2018|Salvador|2500|NaN|12500|
|926|6982|HL7348|SmartWatch|3|Clara|Bruno|3/8/2018|Salvador|1400|NaN|4200|
|927|6983|HL1918|iPhone|5|Sylvio|Bernhardt|2/24/2018|Salvador|5300|NaN|26500|
|928|7005|HL1918|iPhone|1|Natália|Appel|12/4/2018|Salvador|5300|NaN|5300|
|929|7025|HL7348|SmartWatch|4|Helvio|Pedrosa|11/20/2018|Salvador|1400|NaN|5600|
|930|7026|HL8851|Notebook|1|Anna|Maia|1/31/2018|Salvador|3500|NaN|3500|
|931|7030|HL4379|Televisão|1|Gabriel|Azevedo|3/26/2018|Salvador|2500|NaN|2500|
|932|7038|HL2714|Tablet|5|Victor|Magalhães|6/15/2018|Salvador|1600|NaN|8000|
|933|7045|HL1918|iPhone|1|Roberta|Nogueira|2/17/2018|Salvador|5300|NaN|5300|
|934|7046|HL1918|iPhone|4|Célio|Xavier|3/4/2018|Salvador|5300|NaN|21200|
|935|7047|HL1918|iPhone|4|Vivianne|Rodrigues|9/17/2018|Salvador|5300|NaN|21200|
|936|7054|HL9962|Android|4|Rafael|Carneiro|6/16/2018|Salvador|3400|NaN|13600|
|937|7075|HL4379|Televisão|2|Gabriela|Fernandes|3/13/2018|Salvador|2500|NaN|5000|
|938|7077|HL8851|Notebook|4|Bruna|Gomes|10/3/2018|Salvador|3500|NaN|14000|
|939|7086|HL8851|Notebook|2|Marcelo|Magalhães|8/14/2018|Salvador|3500|NaN|7000|
|940|7100|HL1918|iPhone|1|Pedro|Costa|10/16/2018|Salvador|5300|NaN|5300|
|941|7104|HL8851|Notebook|2|Lázaro|Villanova|7/8/2018|Salvador|3500|NaN|7000|
|942|7128|HL4379|Televisão|5|Caroll|Johnson|5/25/2018|Salvador|2500|NaN|12500|
|943|7133|HL4379|Televisão|2|Gustavo|Guimarães|6/7/2018|Salvador|2500|NaN|5000|
|944|7140|HL1148|Câmera|5|Matheus|Souza|2/14/2018|Salvador|2100|NaN|10500|
|945|7146|HL1918|iPhone|3|Ana|Soledade|3/26/2018|Salvador|5300|NaN|15900|
|946|7154|HL4379|Televisão|5|Izabel|Lopes|1/26/2018|Salvador|2500|NaN|12500|
|947|7166|HL8851|Notebook|1|Amanda|Machado|3/29/2018|Salvador|3500|NaN|3500|
|948|7167|HL4379|Televisão|3|Leonardo|Ferreira|6/21/2018|Salvador|2500|NaN|7500|
|949|7176|HL8851|Notebook|1|Gustavo|Junior|5/15/2018|Salvador|3500|NaN|3500|
|950|7182|HL4379|Televisão|4|João|Capitulo|4/13/2018|Salvador|2500|NaN|10000|
|951|7183|HL4379|Televisão|5|Ana|Michetti|7/10/2018|Salvador|2500|NaN|12500|
|952|7188|HL4379|Televisão|2|Juan|Barbosa|4/25/2018|Salvador|2500|NaN|5000|
|953|7200|HL8851|Notebook|3|Bruna|Silveira|11/9/2018|Salvador|3500|NaN|10500|
|954|7215|HL2714|Tablet|2|Patrícia|Amaral|11/3/2018|Salvador|1600|NaN|3200|
|955|7236|HL9962|Android|5|Fernanda|Coutinho|4/1/2018|Salvador|3400|NaN|17000|
|956|7243|HL1918|iPhone|1|Gabrielle|Costa|1/31/2018|Salvador|5300|NaN|5300|
|957|7248|HL7348|SmartWatch|1|Leandro|Ferreira|10/27/2018|Salvador|1400|NaN|1400|
|958|7275|HL4379|Televisão|3|Gabriella|Sagrillo|3/4/2018|Salvador|2500|NaN|7500|
|959|7290|HL1918|iPhone|2|Raíssa|Oros|12/7/2018|Salvador|5300|NaN|10600|
|960|7302|HL1148|Câmera|4|Iuri|Barbosa|7/13/2018|Salvador|2100|NaN|8400|
|961|7311|HL1148|Câmera|2|Bruna|Rosa|3/13/2018|Salvador|2100|NaN|4200|
|962|7318|HL8851|Notebook|2|Samara|Pinto|8/4/2018|Salvador|3500|NaN|7000|
|963|7327|HL4379|Televisão|5|Victor|Lira|12/12/2018|Salvador|2500|NaN|12500|
|964|7331|HL1918|iPhone|5|Yasmim|Verly|9/14/2018|Salvador|5300|NaN|26500|
|965|7334|HL1918|iPhone|3|Marina|Mesquita|10/10/2018|Salvador|5300|NaN|15900|
|966|7337|HL1918|iPhone|5|Bianca|Paz|10/3/2018|Salvador|5300|NaN|26500|
|967|7338|HL1918|iPhone|5|Danilo|Alves|11/2/2018|Salvador|5300|NaN|26500|
|968|7348|HL7348|SmartWatch|3|Natalia|Accioly|6/19/2018|Salvador|1400|NaN|4200|
|969|7352|HL7348|SmartWatch|2|Gabriella|Sagrillo|10/31/2018|Salvador|1400|NaN|2800|
|970|7355|HL7348|SmartWatch|3|Paola|Abreu|3/29/2018|Salvador|1400|NaN|4200|
|971|7361|HL2714|Tablet|5|Wellington|Duarte|5/3/2018|Salvador|1600|NaN|8000|
|972|7381|HL9962|Android|2|Anderson|Martins|8/10/2018|Salvador|3400|NaN|6800|
|973|7387|HL9962|Android|1|Carolina|Motta|10/1/2018|Salvador|3400|NaN|3400|
|974|7391|HL7348|SmartWatch|2|Stefan|Nunes|5/25/2018|Salvador|1400|NaN|2800|
|975|7398|HL7348|SmartWatch|2|Bruna|Silveira|11/22/2018|Salvador|1400|NaN|2800|
|976|7403|HL9962|Android|5|Dandara|Reis|8/20/2018|Salvador|3400|NaN|17000|
|977|7404|HL2714|Tablet|4|Felipe|Cavalcanti|7/27/2018|Salvador|1600|NaN|6400|
|978|7411|HL4379|Televisão|5|Isabelle|Gonçalves|9/13/2018|Salvador|2500|NaN|12500|
|979|7448|HL1148|Câmera|3|Raissa|Pinheiro|9/19/2018|Salvador|2100|NaN|6300|
|980|7458|HL9962|Android|1|Vitor|Campos|2/15/2018|Salvador|3400|NaN|3400|
|981|7466|HL7348|SmartWatch|1|Jonas|Gomes|5/24/2018|Salvador|1400|NaN|1400|
|982|7471|HL7348|SmartWatch|1|Juliana|Hollander|6/17/2018|Salvador|1400|NaN|1400|
|983|7472|HL4379|Televisão|4|Victor|Gomes|7/2/2018|Salvador|2500|NaN|10000|
|984|7487|HL1148|Câmera|3|Lunna|Vannier|8/28/2018|Salvador|2100|NaN|6300|
|985|7488|HL1918|iPhone|5|Gabriel|Pereira|11/17/2018|Salvador|5300|NaN|26500|
|986|7489|HL1918|iPhone|1|Juliana|Mesquita|4/9/2018|Salvador|5300|NaN|5300|
|987|7494|HL1148|Câmera|5|Debora|Silva|2/14/2018|Salvador|2100|NaN|10500|
|988|7506|HL4379|Televisão|5|Carolina|Siqueira|9/26/2018|Salvador|2500|NaN|12500|
|989|7526|HL4379|Televisão|1|Carla|Zakhm|2/17/2018|Salvador|2500|NaN|2500|
|990|7536|HL1148|Câmera|4|Aline|Mello|12/3/2018|Salvador|2100|NaN|8400|
|991|7544|HL4379|Televisão|4|Lázaro|Nascimento|12/16/2018|Salvador|2500|NaN|10000|
|992|7561|HL1918|iPhone|1|Rodrigo|Bruno|4/20/2018|Salvador|5300|NaN|5300|
|993|7572|HL4379|Televisão|2|Gabriella|Sagrillo|2/22/2018|Salvador|2500|NaN|5000|
|994|7579|HL1918|iPhone|1|Juliana|Souza|4/2/2018|Salvador|5300|NaN|5300|
|995|7580|HL4379|Televisão|5|Bernard|Pedrosa|9/24/2018|Salvador|2500|NaN|12500|
|996|7585|HL8851|Notebook|3|Jorge|Fonseca|12/30/2018|Salvador|3500|NaN|10500|
|997|7588|HL2714|Tablet|5|Andre|Nóbrega|9/4/2018|Salvador|1600|NaN|8000|
|998|7594|HL7348|SmartWatch|2|Pedro|Jorge|7/14/2018|Salvador|1400|NaN|2800|
|999|7596|HL9962|Android|2|Ana|Júnior|8/11/2018|Salvador|3400|NaN|6800|
|1000|7600|HL1148|Câmera|2|João|Matheus|8/15/2018|Salvador|2100|NaN|4200|
|1001|7611|HL4379|Televisão|2|Lucas|Araújo|9/20/2018|Salvador|2500|NaN|5000|
|1002|7613|HL7348|SmartWatch|3|Bruna|Brandao|11/16/2018|Salvador|1400|NaN|4200|
|1003|7622|HL9962|Android|5|Jessica|Ferreira|5/15/2018|Salvador|3400|NaN|17000|
|1004|7629|HL1148|Câmera|3|Felipe|Freitas|6/22/2018|Salvador|2100|NaN|6300|
|1005|7641|HL7348|SmartWatch|3|Nina|Magalhães|4/21/2018|Salvador|1400|NaN|4200|
|1006|7652|HL4379|Televisão|1|Felipe|Freitas|4/9/2018|Salvador|2500|NaN|2500|
|1007|7657|HL1918|iPhone|4|Allan|Guedes|1/11/2018|Salvador|5300|NaN|21200|
|1008|7658|HL2714|Tablet|5|Natalia|Guedes|4/16/2018|Salvador|1600|NaN|8000|
|1009|7667|HL1918|iPhone|4|Wellington|Duarte|11/17/2018|Salvador|5300|NaN|21200|
|1010|7674|HL1918|iPhone|4|Juliana|Guimarães|1/12/2018|Salvador|5300|NaN|21200|
|1011|7675|HL2714|Tablet|5|Giulia|Pessanha|3/28/2018|Salvador|1600|NaN|8000|
|1012|7682|HL1918|iPhone|3|Pedro|Xavier|2/15/2018|Salvador|5300|NaN|15900|
|1013|7684|HL8851|Notebook|1|Ana|Fioretti|8/21/2018|Salvador|3500|NaN|3500|
|1014|7685|HL4379|Televisão|3|Bruna|Franco|10/12/2018|Salvador|2500|NaN|7500|
|1015|7702|HL1918|iPhone|2|Platini|Heimlich|2/10/2018|Salvador|5300|NaN|10600|
|1016|7706|HL1148|Câmera|3|Raul|Silveira|1/3/2018|Salvador|2100|NaN|6300|
|1017|7723|HL1918|iPhone|2|Maria|Assumpção|10/2/2018|Salvador|5300|NaN|10600|
|1018|7729|HL2714|Tablet|2|Ana|Gonzaga|11/2/2018|Salvador|1600|NaN|3200|
|1019|7737|HL7348|SmartWatch|3|Renan|Freire|8/16/2018|Salvador|1400|NaN|4200|
|1020|7755|HL1148|Câmera|4|Carolina|Brum|10/29/2018|Salvador|2100|NaN|8400|
|1021|7760|HL9962|Android|4|Luis|Souza|12/11/2018|Salvador|3400|NaN|13600|
|1022|7778|HL8851|Notebook|1|Raphael|Kurtz|10/6/2018|Salvador|3500|NaN|3500|
|1023|7781|HL4379|Televisão|5|Ylana|Teraoka|1/18/2018|Salvador|2500|NaN|12500|
|1024|7784|HL7348|SmartWatch|4|Renan|Nascimento|1/2/2018|Salvador|1400|NaN|5600|
|1025|7788|HL1918|iPhone|4|Beatriz|Perdomo|11/29/2018|Salvador|5300|NaN|21200|
|1026|7795|HL1148|Câmera|1|Bianca|Allevato|3/18/2018|Salvador|2100|NaN|2100|
|1027|7805|HL7348|SmartWatch|1|Julia|Leig|10/22/2018|Salvador|1400|NaN|1400|
|1028|7808|HL4379|Televisão|1|Pedro|Dalforne|4/19/2018|Salvador|2500|NaN|2500|
|1029|7823|HL4379|Televisão|2|Antonio|Manhães|2/25/2018|Salvador|2500|NaN|5000|
|1030|7830|HL1918|iPhone|2|Sthefeson|Kohn|8/9/2018|Salvador|5300|NaN|10600|
|1031|7834|HL1148|Câmera|5|Thiago|Costa|12/16/2018|Salvador|2100|NaN|10500|
|1032|7842|HL4379|Televisão|2|Alon|Palmeira|5/6/2018|Salvador|2500|NaN|5000|
|1033|7857|HL1918|iPhone|5|Rojane|Lima|5/14/2018|Salvador|5300|NaN|26500|
|1034|7866|HL1918|iPhone|3|Alessandra|Martins|10/11/2018|Salvador|5300|NaN|15900|
|1035|7869|HL1918|iPhone|4|Glenda|Santos|10/28/2018|Salvador|5300|NaN|21200|
|1036|7872|HL7348|SmartWatch|4|Leonardo|Ferreira|4/20/2018|Salvador|1400|NaN|5600|
|1037|7876|HL8851|Notebook|5|Ana|Gonzaga|6/15/2018|Salvador|3500|NaN|17500|
|1038|7878|HL4379|Televisão|4|Isabelle|Gonçalves|12/3/2018|Salvador|2500|NaN|10000|
|1039|7884|HL8851|Notebook|5|Lara|Moreira|12/4/2018|Salvador|3500|NaN|17500|
|1040|7893|HL2714|Tablet|5|Adriane|Chagas|9/18/2018|Salvador|1600|NaN|8000|
|1041|7894|HL1918|iPhone|5|Matheus|Ramos|9/15/2018|Salvador|5300|NaN|26500|
|1042|7897|HL4379|Televisão|2|Lucas|Araújo|11/13/2018|Salvador|2500|NaN|5000|
|1043|7898|HL4379|Televisão|5|Fillipe|Almeida|6/24/2018|Salvador|2500|NaN|12500|
|1044|7899|HL7348|SmartWatch|3|Ana|Almeida|5/14/2018|Salvador|1400|NaN|4200|
|1045|7903|HL1918|iPhone|5|Myllena|Corrêa|8/12/2018|Salvador|5300|NaN|26500|
|1046|7921|HL4379|Televisão|5|Victor|Lira|7/26/2018|Salvador|2500|NaN|12500|
|1047|7925|HL1918|iPhone|5|Wen|Santos|12/18/2018|Salvador|5300|NaN|26500|
|1048|7928|HL4379|Televisão|3|Matheus|Sapir|12/16/2018|Salvador|2500|NaN|7500|
|1049|7948|HL8851|Notebook|5|Lucas|Lima|11/1/2018|Salvador|3500|NaN|17500|
|1050|7949|HL1918|iPhone|4|Daniel|Nauenberg|8/23/2018|Salvador|5300|NaN|21200|
|1051|7954|HL1918|iPhone|4|Wilson|Miranda|12/15/2018|Salvador|5300|NaN|21200|
|1052|7965|HL8851|Notebook|3|Ana|Campos|6/6/2018|Salvador|3500|NaN|10500|
|1053|7968|HL1918|iPhone|2|Raissa|Sales|3/27/2018|Salvador|5300|NaN|10600|
|1054|7969|HL1148|Câmera|1|Carlos|Souza|2/27/2018|Salvador|2100|NaN|2100|
|1055|7974|HL1918|iPhone|2|Matheus|Moraes|9/11/2018|Salvador|5300|NaN|10600|
|1056|7985|HL8851|Notebook|4|Gabriela|Aliani|7/23/2018|Salvador|3500|NaN|14000|
|1057|7987|HL1918|iPhone|4|Clarissa|Santos|10/10/2018|Salvador|5300|NaN|21200|
|1058|7988|HL4379|Televisão|4|Carolina|Carneiro|7/10/2018|Salvador|2500|NaN|10000|
|1059|7992|HL2714|Tablet|1|Vitor|Arruda|6/26/2018|Salvador|1600|NaN|1600|
|1060|8006|HL8851|Notebook|2|Luiz|Limp|10/21/2018|Salvador|3500|NaN|7000|
|1061|8013|HL1918|iPhone|3|Marina|Mesquita|2/15/2018|Salvador|5300|NaN|15900|
|1062|8015|HL4379|Televisão|4|Raissa|Maia|1/8/2018|Salvador|2500|NaN|10000|
|1063|8028|HL1918|iPhone|2|Raphael|Ferman|3/17/2018|Salvador|5300|NaN|10600|
|1064|8042|HL1918|iPhone|4|Bruno|Velucci|6/3/2018|Salvador|5300|NaN|21200|
|1065|8043|HL7348|SmartWatch|3|Renan|Cunha|5/1/2018|Salvador|1400|NaN|4200|
|1066|8044|HL8851|Notebook|3|Caio|Fernandes|1/20/2018|Salvador|3500|NaN|10500|
|1067|8054|HL2714|Tablet|1|Hércules|Júnior|3/18/2018|Salvador|1600|NaN|1600|
|1068|8064|HL4379|Televisão|3|Roger|Rosa|12/9/2018|Salvador|2500|NaN|7500|
|1069|8074|HL1148|Câmera|2|Priscila|Suzano|2/27/2018|Salvador|2100|NaN|4200|
|1070|8078|HL8851|Notebook|2|Thales|Portillo|6/13/2018|Salvador|3500|NaN|7000|
|1071|8090|HL1148|Câmera|1|Michelle|Figueiredo|5/23/2018|Salvador|2100|NaN|2100|
|1072|8091|HL4379|Televisão|5|Luiza|Procaci|11/27/2018|Salvador|2500|NaN|12500|
|1073|8093|HL1918|iPhone|4|Joao|Silva|4/15/2018|Salvador|5300|NaN|21200|
|1074|8095|HL8851|Notebook|1|Lucas|Destri|8/4/2018|Salvador|3500|NaN|3500|
|1075|8110|HL9962|Android|4|Manuela|Merege|12/15/2018|Salvador|3400|NaN|13600|
|1076|8111|HL7348|SmartWatch|2|Juliana|Barreira|2/22/2018|Salvador|1400|NaN|2800|
|1077|8115|HL1148|Câmera|2|Victor|Gomes|10/2/2018|Salvador|2100|NaN|4200|
|1078|8124|HL1918|iPhone|5|Daniel|Araujo|3/4/2018|Salvador|5300|NaN|26500|
|1079|8136|HL1918|iPhone|2|Vivianne|Rodrigues|10/9/2018|Salvador|5300|NaN|10600|
|1080|8138|HL4379|Televisão|1|Marina|Miranda|8/11/2018|Salvador|2500|NaN|2500|
|1081|8142|HL7348|SmartWatch|2|Thales|Fanara|11/7/2018|Salvador|1400|NaN|2800|
|1082|8151|HL2714|Tablet|1|Isabel|Lacerda|6/10/2018|Salvador|1600|NaN|1600|
|1083|8176|HL1148|Câmera|1|Caroline|Cavalcanti|10/30/2018|Salvador|2100|NaN|2100|
|1084|8186|HL8851|Notebook|5|Luiza|Johnson|8/27/2018|Salvador|3500|NaN|17500|
|1085|8189|HL1148|Câmera|5|Dandara|Reis|2/19/2018|Salvador|2100|NaN|10500|
|1086|8197|HL1918|iPhone|2|João|Abraçado|6/6/2018|Salvador|5300|NaN|10600|
|1087|8215|HL7348|SmartWatch|1|Caroline|Pinto|1/10/2018|Salvador|1400|NaN|1400|
|1088|8226|HL2714|Tablet|1|Carlos|Galvão|6/16/2018|Salvador|1600|NaN|1600|
|1089|8231|HL7348|SmartWatch|4|Michelle|Miura|2/20/2018|Salvador|1400|NaN|5600|
|1090|8238|HL4379|Televisão|2|Eduardo|Pacheco|6/17/2018|Salvador|2500|NaN|5000|
|1091|8277|HL9962|Android|4|Lucas|Cavalcanti|3/1/2018|Salvador|3400|NaN|13600|
|1092|8286|HL1918|iPhone|4|Victoria|Mazza|11/5/2018|Salvador|5300|NaN|21200|
|1093|8295|HL1918|iPhone|4|Bruna|Londero|8/18/2018|Salvador|5300|NaN|21200|
|1094|8297|HL9962|Android|3|Camille|Silva|3/30/2018|Salvador|3400|NaN|10200|
|1095|8301|HL1918|iPhone|4|Giselia|Thiele|2/9/2018|Salvador|5300|NaN|21200|
|1096|8307|HL9962|Android|4|Rafaela|Gonçalves|2/10/2018|Salvador|3400|NaN|13600|
|1097|8314|HL1918|iPhone|3|Natalia|Andrade|7/2/2018|Salvador|5300|NaN|15900|
|1098|8315|HL9962|Android|3|Beatriz|Cavalcanti|6/29/2018|Salvador|3400|NaN|10200|
|1099|8321|HL9962|Android|1|Lucas|Cavalcanti|6/29/2018|Salvador|3400|NaN|3400|
|1100|8324|HL1918|iPhone|4|Bruna|Rosa|5/13/2018|Salvador|5300|NaN|21200|
|1101|8328|HL1148|Câmera|2|Alon|Palmeira|4/24/2018|Salvador|2100|NaN|4200|
|1102|8333|HL7348|SmartWatch|3|Felipe|Jorge|8/26/2018|Salvador|1400|NaN|4200|
|1103|8337|HL9962|Android|3|Morgana|Correa|5/30/2018|Salvador|3400|NaN|10200|
|1104|8340|HL1918|iPhone|2|Stephanie|Novak|6/19/2018|Salvador|5300|NaN|10600|
|1105|8341|HL4379|Televisão|1|Julia|Leite|7/31/2018|Salvador|2500|NaN|2500|
|1106|8343|HL2714|Tablet|2|Lucas|Rodrigues|6/2/2018|Salvador|1600|NaN|3200|
|1107|8351|HL8851|Notebook|4|Danilo|Alves|4/16/2018|Salvador|3500|NaN|14000|
|1108|8356|HL1918|iPhone|1|Deysiane|Medronho|4/24/2018|Salvador|5300|NaN|5300|
|1109|8370|HL8851|Notebook|3|Gustavo|Accardo|3/17/2018|Salvador|3500|NaN|10500|
|1110|8382|HL2714|Tablet|2|Jéssica|Teixeira|6/22/2018|Salvador|1600|NaN|3200|
|1111|8393|HL7348|SmartWatch|1|Bruno|Mota|12/14/2018|Salvador|1400|NaN|1400|
|1112|8398|HL1918|iPhone|2|Gustavo|Erthal|9/21/2018|Salvador|5300|NaN|10600|
|1113|8400|HL9962|Android|3|Jonatas|Essaber|12/21/2018|Salvador|3400|NaN|10200|
|1114|8426|HL4379|Televisão|1|Anna|Maia|11/27/2018|Salvador|2500|NaN|2500|
|1115|8427|HL4379|Televisão|3|Henrique|Silva|2/25/2018|Salvador|2500|NaN|7500|
|1116|8429|HL2714|Tablet|1|Raíza|Lopes|11/22/2018|Salvador|1600|NaN|1600|
|1117|8430|HL1148|Câmera|1|Daniel|Valente|7/2/2018|Salvador|2100|NaN|2100|
|1118|8434|HL1918|iPhone|5|Thiago|Miura|5/4/2018|Salvador|5300|NaN|26500|
|1119|8442|HL1918|iPhone|4|Lara|Moreira|11/30/2018|Salvador|5300|NaN|21200|
|1120|8452|HL1918|iPhone|3|Wilson|Meirelles|9/21/2018|Salvador|5300|NaN|15900|
|1121|8469|HL4379|Televisão|3|Thays|Castro|8/14/2018|Salvador|2500|NaN|7500|
|1122|8489|HL1918|iPhone|4|Caio|Vianna|12/31/2018|Salvador|5300|NaN|21200|
|1123|8493|HL9962|Android|2|Carolina|Brum|4/23/2018|Salvador|3400|NaN|6800|
|1124|8501|HL4379|Televisão|3|Pedro|Cardoso|8/9/2018|Salvador|2500|NaN|7500|
|1125|8519|HL1918|iPhone|5|Viviane|Souza|7/5/2018|Salvador|5300|NaN|26500|
|1126|8520|HL2714|Tablet|3|Ana|Gomes|11/26/2018|Salvador|1600|NaN|4800|
|1127|8523|HL9962|Android|1|Gabriella|Lopes|4/24/2018|Salvador|3400|NaN|3400|
|1128|8529|HL1918|iPhone|3|Bernard|Pedrosa|6/2/2018|Salvador|5300|NaN|15900|
|1129|8540|HL2714|Tablet|1|Matheus|Delgado|5/9/2018|Salvador|1600|NaN|1600|
|1130|8541|HL1148|Câmera|5|Beatriz|Rodrigues|11/27/2018|Salvador|2100|NaN|10500|
|1131|8559|HL1918|iPhone|1|Jessica|Ferreira|4/20/2018|Salvador|5300|NaN|5300|
|1132|8568|HL1148|Câmera|3|Helena|Chafin|4/28/2018|Salvador|2100|NaN|6300|
|1133|8588|HL8851|Notebook|3|Miguel|Carneiro|8/15/2018|Salvador|3500|NaN|10500|
|1134|8596|HL9962|Android|1|Anízio|Carvalho|2/19/2018|Salvador|3400|NaN|3400|
|1135|8604|HL1918|iPhone|1|Wen|Santos|6/1/2018|Salvador|5300|NaN|5300|
|1136|8611|HL8851|Notebook|4|Daniel|Felippe|12/12/2018|Salvador|3500|NaN|14000|
|1137|8623|HL1918|iPhone|5|Victor|Lira|6/6/2018|Salvador|5300|NaN|26500|
|1138|8624|HL1918|iPhone|2|Alberto|Silveira|10/22/2018|Salvador|5300|NaN|10600|
|1139|8625|HL1918|iPhone|5|Ana|Carvalho|2/13/2018|Salvador|5300|NaN|26500|
|1140|8634|HL4379|Televisão|4|Gabriella|Sagrillo|3/11/2018|Salvador|2500|NaN|10000|
|1141|8639|HL1918|iPhone|1|Rafael|Rocha|11/5/2018|Salvador|5300|NaN|5300|
|1142|8640|HL1918|iPhone|2|Julia|Leig|3/30/2018|Salvador|5300|NaN|10600|
|1143|8641|HL1918|iPhone|3|Gabriel|Brito|12/8/2018|Salvador|5300|NaN|15900|
|1144|8642|HL8851|Notebook|4|Guilherme|Vianna|5/28/2018|Salvador|3500|NaN|14000|
|1145|8645|HL1918|iPhone|1|Henrique|Villanova|9/16/2018|Salvador|5300|NaN|5300|
|1146|8648|HL7348|SmartWatch|4|Mariana|Freire|11/7/2018|Salvador|1400|NaN|5600|
|1147|8650|HL1918|iPhone|5|Vitor|Arruda|3/11/2018|Salvador|5300|NaN|26500|
|1148|8660|HL2714|Tablet|2|Bernardo|Ribeiro|9/24/2018|Salvador|1600|NaN|3200|
|1149|8666|HL8851|Notebook|2|Maria|Mello|11/6/2018|Salvador|3500|NaN|7000|
|1150|8668|HL1918|iPhone|3|José|Fonseca|3/30/2018|Salvador|5300|NaN|15900|
|1151|8670|HL7348|SmartWatch|2|Milena|Pereira|4/17/2018|Salvador|1400|NaN|2800|
|1152|8671|HL4379|Televisão|3|Renan|Ventura|10/18/2018|Salvador|2500|NaN|7500|
|1153|8674|HL4379|Televisão|4|Juliana|Mesquita|8/8/2018|Salvador|2500|NaN|10000|
|1154|8675|HL4379|Televisão|2|Cláudio|Aragão|3/10/2018|Salvador|2500|NaN|5000|
|1155|8683|HL9962|Android|3|Rafael|Wajnsztok|2/6/2018|Salvador|3400|NaN|10200|
|1156|8685|HL9962|Android|3|Mariana|Baptista|8/8/2018|Salvador|3400|NaN|10200|
|1157|8688|HL2714|Tablet|5|Lucas|Lima|8/24/2018|Salvador|1600|NaN|8000|
|1158|8690|HL1918|iPhone|4|Erick|Soares|11/10/2018|Salvador|5300|NaN|21200|
|1159|8693|HL7348|SmartWatch|5|Bianca|Piero|10/17/2018|Salvador|1400|NaN|7000|
|1160|8694|HL1918|iPhone|4|Gustavo|Junior|12/6/2018|Salvador|5300|NaN|21200|
|1161|8702|HL4379|Televisão|3|Paula|Cavalcanti|2/22/2018|Salvador|2500|NaN|7500|
|1162|8711|HL2714|Tablet|1|Eduardo|Lopes|11/23/2018|Salvador|1600|NaN|1600|
|1163|8717|HL7348|SmartWatch|4|Bernardo|Botelho|5/10/2018|Salvador|1400|NaN|5600|
|1164|8720|HL8851|Notebook|3|Anna|Maia|11/30/2018|Salvador|3500|NaN|10500|
|1165|8721|HL4379|Televisão|2|Beatriz|Rocha|5/24/2018|Salvador|2500|NaN|5000|
|1166|8727|HL2714|Tablet|3|Victor|Oliveira|8/10/2018|Salvador|1600|NaN|4800|
|1167|8738|HL9962|Android|4|Cícero|Ramos|11/2/2018|Salvador|3400|NaN|13600|
|1168|8742|HL1918|iPhone|1|Larissa|Vasconcellos|11/14/2018|Salvador|5300|NaN|5300|
|1169|8746|HL2714|Tablet|3|Isabelle|Gonçalves|6/30/2018|Salvador|1600|NaN|4800|
|1170|8748|HL1918|iPhone|5|Ana|Gomes|1/24/2018|Salvador|5300|NaN|26500|
|1171|8751|HL1918|iPhone|2|Pedro|Macckione|5/27/2018|Salvador|5300|NaN|10600|
|1172|8756|HL4379|Televisão|5|Luiza|Marques|1/12/2018|Salvador|2500|NaN|12500|
|1173|8758|HL1918|iPhone|4|Eric|Neves|6/20/2018|Salvador|5300|NaN|21200|
|1174|8763|HL7348|SmartWatch|5|Gabriela|Aliani|4/23/2018|Salvador|1400|NaN|7000|
|1175|8783|HL4379|Televisão|5|Thainá|Binello|6/20/2018|Salvador|2500|NaN|12500|
|1176|8802|HL1148|Câmera|1|Thaís|Pereira|12/11/2018|Salvador|2100|NaN|2100|
|1177|8810|HL1918|iPhone|5|Isabela|Resende|12/14/2018|Salvador|5300|NaN|26500|
|1178|8827|HL8851|Notebook|2|Rogério|Gentile|8/8/2018|Salvador|3500|NaN|7000|
|1179|8830|HL7348|SmartWatch|4|Stefan|Nunes|9/19/2018|Salvador|1400|NaN|5600|
|1180|8834|HL8851|Notebook|2|Gabriel|Brito|1/3/2018|Salvador|3500|NaN|7000|
|1181|8842|HL1918|iPhone|5|Luíza|Garcia|6/26/2018|Salvador|5300|NaN|26500|
|1182|8855|HL2714|Tablet|5|Igor|Lima|3/4/2018|Salvador|1600|NaN|8000|
|1183|8866|HL4379|Televisão|4|Luana|Santos|12/15/2018|Salvador|2500|NaN|10000|
|1184|8867|HL7348|SmartWatch|2|Tiago|Pereira|11/13/2018|Salvador|1400|NaN|2800|
|1185|8870|HL7348|SmartWatch|1|João|Tabet|7/30/2018|Salvador|1400|NaN|1400|
|1186|8872|HL9962|Android|3|Lucas|Fontoura|1/13/2018|Salvador|3400|NaN|10200|
|1187|8893|HL8851|Notebook|2|Célio|Xavier|2/15/2018|Salvador|3500|NaN|7000|
|1188|8898|HL7348|SmartWatch|5|Rodrigo|Bruno|7/8/2018|Salvador|1400|NaN|7000|
|1189|8913|HL9962|Android|3|Paulo|Campos|1/28/2018|Salvador|3400|NaN|10200|
|1190|8920|HL9962|Android|3|Ruan|Lopes|4/23/2018|Salvador|3400|NaN|10200|
|1191|8927|HL1148|Câmera|4|Matheus|Santos|5/14/2018|Salvador|2100|NaN|8400|
|1192|8931|HL1918|iPhone|2|Maria|Mello|2/25/2018|Salvador|5300|NaN|10600|
|1193|8934|HL7348|SmartWatch|3|Felipe|Paulo|10/13/2018|Salvador|1400|NaN|4200|
|1194|8937|HL4379|Televisão|5|Eduardo|Nunes|12/15/2018|Salvador|2500|NaN|12500|
|1195|8944|HL4379|Televisão|4|Carlos|Galvão|8/19/2018|Salvador|2500|NaN|10000|
|1196|8946|HL1918|iPhone|4|Natalia|Andrade|8/19/2018|Salvador|5300|NaN|21200|
|1197|8947|HL8851|Notebook|1|Carolina|Silva|12/3/2018|Salvador|3500|NaN|3500|
|1198|8967|HL1148|Câmera|2|Rebeca|Taylor|8/29/2018|Salvador|2100|NaN|4200|
|1199|8969|HL1918|iPhone|5|Daniel|Nauenberg|5/28/2018|Salvador|5300|NaN|26500|
|1200|8974|HL1918|iPhone|2|Thiago|Costa|6/7/2018|Salvador|5300|NaN|10600|
|1201|8977|HL4379|Televisão|2|Rafael|Rocha|10/31/2018|Salvador|2500|NaN|5000|
|1202|8981|HL1148|Câmera|2|Jonas|Gomes|3/16/2018|Salvador|2100|NaN|4200|
|1203|8984|HL8851|Notebook|2|Isabella|Montanholi|5/2/2018|Salvador|3500|NaN|7000|
|1204|8986|HL4379|Televisão|5|Bruna|Londero|7/18/2018|Salvador|2500|NaN|12500|
|1205|9003|HL1918|iPhone|3|Diego|Marchesi|10/6/2018|Salvador|5300|NaN|15900|
|1206|9008|HL1918|iPhone|1|Rachel|Restum|5/30/2018|Salvador|5300|NaN|5300|
|1207|9013|HL9962|Android|2|Pedro|Oliveira|1/2/2018|Salvador|3400|NaN|6800|
|1208|9015|HL9962|Android|2|Thomáz|Rodriguez|11/28/2018|Salvador|3400|NaN|6800|
|1209|9017|HL1148|Câmera|1|Fernanda|Coutinho|2/14/2018|Salvador|2100|NaN|2100|
|1210|9027|HL7348|SmartWatch|5|Thays|Castro|10/26/2018|Salvador|1400|NaN|7000|
|1211|9036|HL1918|iPhone|1|Thayna|Martins|3/8/2018|Salvador|5300|NaN|5300|
|1212|9044|HL4379|Televisão|3|Bruno|Mota|6/9/2018|Salvador|2500|NaN|7500|
|1213|9045|HL7348|SmartWatch|3|Natali|Rangel|3/9/2018|Salvador|1400|NaN|4200|
|1214|9062|HL8851|Notebook|2|Mariana|Baptista|7/6/2018|Salvador|3500|NaN|7000|
|1215|9074|HL1148|Câmera|1|Juan|Fernandes|5/5/2018|Salvador|2100|NaN|2100|
|1216|9093|HL9962|Android|2|Juliana|Silva|12/6/2018|Salvador|3400|NaN|6800|
|1217|9116|HL2714|Tablet|4|Matheus|Gomes|8/6/2018|Salvador|1600|NaN|6400|
|1218|9132|HL4379|Televisão|4|Jéssica|Netto|2/10/2018|Salvador|2500|NaN|10000|
|1219|9149|HL7348|SmartWatch|5|Tiago|Pereira|11/1/2018|Salvador|1400|NaN|7000|
|1220|9163|HL8851|Notebook|1|Lívia|Marques|1/2/2018|Salvador|3500|NaN|3500|
|1221|9169|HL4379|Televisão|4|Daniel|Terra|2/6/2018|Salvador|2500|NaN|10000|
|1222|9173|HL7348|SmartWatch|5|Ana|Gomes|7/21/2018|Salvador|1400|NaN|7000|
|1223|9188|HL9962|Android|5|Gabriel|Azevedo|10/27/2018|Salvador|3400|NaN|17000|
|1224|9206|HL9962|Android|5|Lívia|Tanaka|8/14/2018|Salvador|3400|NaN|17000|
|1225|9225|HL7348|SmartWatch|3|Julia|Teixeira|6/5/2018|Salvador|1400|NaN|4200|
|1226|9232|HL9962|Android|3|Thomáz|Vannier|4/9/2018|Salvador|3400|NaN|10200|
|1227|9239|HL1918|iPhone|2|Caio|Vianna|3/15/2018|Salvador|5300|NaN|10600|
|1228|9253|HL1918|iPhone|1|Lorena|Kohn|4/28/2018|Salvador|5300|NaN|5300|
|1229|9263|HL1918|iPhone|1|Lucas|Baptista|7/6/2018|Salvador|5300|NaN|5300|
|1230|9273|HL1918|iPhone|1|Bruna|Londero|7/1/2018|Salvador|5300|NaN|5300|
|1231|9274|HL4379|Televisão|5|Thais|Rodrigues|8/7/2018|Salvador|2500|NaN|12500|
|1232|9279|HL4379|Televisão|2|Andreza|Ramos|5/11/2018|Salvador|2500|NaN|5000|
|1233|9280|HL1918|iPhone|5|Guilherme|Seixas|1/8/2018|Salvador|5300|NaN|26500|
|1234|9283|HL4379|Televisão|5|Guilherme|Vianna|4/1/2018|Salvador|2500|NaN|12500|
|1235|9289|HL1148|Câmera|5|Ulisses|Filho|10/4/2018|Salvador|2100|NaN|10500|
|1236|9294|HL1148|Câmera|5|Lucas|Rodrigues|5/27/2018|Salvador|2100|NaN|10500|
|1237|9300|HL1918|iPhone|5|Carolina|Figueiredo|1/13/2018|Salvador|5300|NaN|26500|
|1238|9305|HL1918|iPhone|2|Joana|Calmon|9/29/2018|Salvador|5300|NaN|10600|
|1239|9314|HL8851|Notebook|5|Luiza|Marques|7/6/2018|Salvador|3500|NaN|17500|
|1240|9317|HL4379|Televisão|2|Leandro|Ferreira|4/21/2018|Salvador|2500|NaN|5000|
|1241|9321|HL1918|iPhone|5|Matheus|Miranda|10/2/2018|Salvador|5300|NaN|26500|
|1242|9323|HL1918|iPhone|4|Gabriel|Almeida|12/23/2018|Salvador|5300|NaN|21200|
|1243|9325|HL4379|Televisão|3|José|Marques|11/13/2018|Salvador|2500|NaN|7500|
|1244|9326|HL7348|SmartWatch|4|Sandy|Figueiredo|9/18/2018|Salvador|1400|NaN|5600|
|1245|9329|HL4379|Televisão|1|Platini|Heimlich|7/5/2018|Salvador|2500|NaN|2500|
|1246|9333|HL1918|iPhone|3|Renan|Nascimento|6/25/2018|Salvador|5300|NaN|15900|
|1247|9344|HL4379|Televisão|5|Roger|Rosa|6/7/2018|Salvador|2500|NaN|12500|
|1248|9347|HL7348|SmartWatch|3|Lívia|Tanaka|12/23/2018|Salvador|1400|NaN|4200|
|1249|9356|HL4379|Televisão|3|Thiago|Veloso|5/20/2018|Salvador|2500|NaN|7500|
|1250|9382|HL7348|SmartWatch|1|Wen|Santos|3/8/2018|Salvador|1400|NaN|1400|
|1251|9387|HL1918|iPhone|4|Raíza|Lopes|5/14/2018|Salvador|5300|NaN|21200|
|1252|9434|HL1918|iPhone|1|José|Marques|9/13/2018|Salvador|5300|NaN|5300|
|1253|9442|HL1918|iPhone|2|Victor|Oliveira|4/2/2018|Salvador|5300|NaN|10600|
|1254|9444|HL7348|SmartWatch|5|Felipe|Mendonça|10/31/2018|Salvador|1400|NaN|7000|
|1255|9452|HL4379|Televisão|3|Rafaela|Ferreira|1/17/2018|Salvador|2500|NaN|7500|
|1256|9460|HL1918|iPhone|1|Diego|Rodrigues|2/16/2018|Salvador|5300|NaN|5300|
|1257|9468|HL1918|iPhone|5|Larissa|Jesus|11/25/2018|Salvador|5300|NaN|26500|
|1258|9477|HL1918|iPhone|1|Hércules|Júnior|8/10/2018|Salvador|5300|NaN|5300|
|1259|9479|HL1918|iPhone|1|Caio|Moraes|10/6/2018|Salvador|5300|NaN|5300|
|1260|9486|HL9962|Android|3|Matheus|Silva|5/31/2018|Salvador|3400|NaN|10200|
|1261|9508|HL7348|SmartWatch|4|Luiz|Limp|2/17/2018|Salvador|1400|NaN|5600|
|1262|9509|HL7348|SmartWatch|3|Carolina|Costa|3/6/2018|Salvador|1400|NaN|4200|
|1263|9515|HL8851|Notebook|1|Ulisses|Quinto|11/8/2018|Salvador|3500|NaN|3500|
|1264|9529|HL1918|iPhone|1|Daniel|Nauenberg|11/14/2018|Salvador|5300|NaN|5300|
|1265|9535|HL7348|SmartWatch|1|Carlos|Mesquita|7/12/2018|Salvador|1400|NaN|1400|
|1266|9541|HL4379|Televisão|2|Giselia|Thiele|7/29/2018|Salvador|2500|NaN|5000|
|1267|9549|HL4379|Televisão|1|Ana|Felippe|2/9/2018|Salvador|2500|NaN|2500|
|1268|9558|HL1918|iPhone|4|Bruno|Mota|3/31/2018|Salvador|5300|NaN|21200|
|1269|9563|HL4379|Televisão|5|Eduardo|Ferreira|4/24/2018|Salvador|2500|NaN|12500|
|1270|9566|HL1148|Câmera|3|João|Matheus|11/5/2018|Salvador|2100|NaN|6300|
|1271|9572|HL1148|Câmera|3|Glenda|Santos|3/17/2018|Salvador|2100|NaN|6300|
|1272|9597|HL1148|Câmera|1|Beatriz|Rodrigues|10/29/2018|Salvador|2100|NaN|2100|
|1273|9600|HL4379|Televisão|1|Clarissa|Santos|3/21/2018|Salvador|2500|NaN|2500|
|1274|9602|HL7348|SmartWatch|5|Marina|Marins|4/25/2018|Salvador|1400|NaN|7000|
|1275|9603|HL4379|Televisão|1|Stefan|Nunes|1/18/2018|Salvador|2500|NaN|2500|
|1276|9605|HL8851|Notebook|5|Tadeu|Sousa|6/29/2018|Salvador|3500|NaN|17500|
|1277|9616|HL1918|iPhone|5|Bruno|Silva|2/17/2018|Salvador|5300|NaN|26500|
|1278|9621|HL1148|Câmera|4|Thaís|Ribeiro|10/21/2018|Salvador|2100|NaN|8400|
|1279|9630|HL8851|Notebook|3|Raphael|Rezende|10/11/2018|Salvador|3500|NaN|10500|
|1280|9651|HL8851|Notebook|4|Breno|Godoy|1/23/2018|Salvador|3500|NaN|14000|
|1281|9677|HL4379|Televisão|2|Thiago|Nóbrega|5/25/2018|Salvador|2500|NaN|5000|
|1282|9681|HL4379|Televisão|3|Larissa|Nauenberg|4/16/2018|Salvador|2500|NaN|7500|
|1283|9682|HL1918|iPhone|1|Mariana|Miranda|1/21/2018|Salvador|5300|NaN|5300|
|1284|9684|HL9962|Android|1|Raphael|Mattos|9/19/2018|Salvador|3400|NaN|3400|
|1285|9689|HL1918|iPhone|2|Letícia|Leal|12/24/2018|Salvador|5300|NaN|10600|
|1286|9692|HL1148|Câmera|2|Gabriel|Thome|4/7/2018|Salvador|2100|NaN|4200|
|1287|9721|HL9962|Android|2|Igor|Azevedo|7/23/2018|Salvador|3400|NaN|6800|
|1288|9726|HL4379|Televisão|4|Larissa|Cruz|7/28/2018|Salvador|2500|NaN|10000|
|1289|9735|HL4379|Televisão|3|Mariana|Baptista|12/14/2018|Salvador|2500|NaN|7500|
|1290|9743|HL4379|Televisão|4|Julie|Ferreira|1/21/2018|Salvador|2500|NaN|10000|
|1291|9748|HL8851|Notebook|3|Lucas|Coelho|10/31/2018|Salvador|3500|NaN|10500|
|1292|9754|HL2714|Tablet|1|Vanessa|Neves|4/27/2018|Salvador|1600|NaN|1600|
|1293|9760|HL2714|Tablet|2|Luis|Souza|1/16/2018|Salvador|1600|NaN|3200|
|1294|9761|HL4379|Televisão|3|Sandy|Moreira|5/22/2018|Salvador|2500|NaN|7500|
|1295|9762|HL4379|Televisão|5|Rilson|Dias|8/22/2018|Salvador|2500|NaN|12500|
|1296|9771|HL4379|Televisão|3|Júlia|Almeida|7/6/2018|Salvador|2500|NaN|7500|
|1297|9776|HL7348|SmartWatch|3|Katharina|Barros|1/18/2018|Salvador|1400|NaN|4200|
|1298|9791|HL8851|Notebook|3|Kimberly|Sad|11/4/2018|Salvador|3500|NaN|10500|
|1299|9792|HL1918|iPhone|4|Juliana|Barreira|7/25/2018|Salvador|5300|NaN|21200|
|1300|9796|HL1918|iPhone|4|Lucas|Valim|7/24/2018|Salvador|5300|NaN|21200|
|1301|9798|HL1918|iPhone|1|Rodrigo|Silva|11/1/2018|Salvador|5300|NaN|5300|
|1302|9800|HL8851|Notebook|3|Thales|Gouvêa|9/5/2018|Salvador|3500|NaN|10500|
|1303|9807|HL1918|iPhone|4|Joao|Pereira|12/30/2018|Salvador|5300|NaN|21200|
|1304|9815|HL4379|Televisão|5|Adriana|Passos|1/30/2018|Salvador|2500|NaN|12500|
|1305|9826|HL1148|Câmera|5|Luis|Garcia|3/17/2018|Salvador|2100|NaN|10500|
|1306|9837|HL1918|iPhone|2|Alvaro|Kranz|1/14/2018|Salvador|5300|NaN|10600|
|1307|9842|HL1148|Câmera|5|Bruno|Ferreira|12/17/2018|Salvador|2100|NaN|10500|
|1308|9862|HL9962|Android|1|Helena|Chafin|9/27/2018|Salvador|3400|NaN|3400|
|1309|9863|HL4379|Televisão|2|Eric|Neves|8/31/2018|Salvador|2500|NaN|5000|
|1310|9879|HL1918|iPhone|5|Marcelo|Magalhães|2/27/2018|Salvador|5300|NaN|26500|
|1311|9882|HL9962|Android|4|Lucas|Freitas|9/19/2018|Salvador|3400|NaN|13600|
|1312|9885|HL4379|Televisão|5|Rodrigo|Mendes|7/6/2018|Salvador|2500|NaN|12500|
|1313|9897|HL7348|SmartWatch|5|Maike|Pereira|4/26/2018|Salvador|1400|NaN|7000|
|1314|9898|HL1148|Câmera|5|Lucas|Wanderley|9/3/2018|Salvador|2100|NaN|10500|
|1315|9908|HL2714|Tablet|3|Leandro|Ferreira|3/17/2018|Salvador|1600|NaN|4800|
|1316|9919|HL4379|Televisão|5|Miguel|Carneiro|2/19/2018|Salvador|2500|NaN|12500|
|1317|9924|HL2714|Tablet|1|Lorena|Carvalho|5/8/2018|Salvador|1600|NaN|1600|
|1318|9933|HL1918|iPhone|3|Lucas|Monte|9/13/2018|Salvador|5300|NaN|15900|
|1319|9936|HL1918|iPhone|4|Rojane|Lima|1/6/2018|Salvador|5300|NaN|21200|
|1320|9939|HL7348|SmartWatch|1|Caroline|Cavalcanti|2/5/2018|Salvador|1400|NaN|1400|
|1321|9950|HL1148|Câmera|4|Antonio|Bernhardt|10/27/2018|Salvador|2100|NaN|8400|
|1322|9954|HL4379|Televisão|3|Alon|Palmeira|5/13/2018|Salvador|2500|NaN|7500|
|1323|9962|HL7348|SmartWatch|1|Eduardo|Nunes|7/26/2018|Salvador|1400|NaN|1400|
|1324|9964|HL2714|Tablet|1|Caroline|Delgado|3/30/2018|Salvador|1600|NaN|1600|
|1325|9965|HL1148|Câmera|4|Samara|Pinto|3/11/2018|Salvador|2100|NaN|8400|
|1326|9970|HL9962|Android|1|Fernanda|Junior|9/12/2018|Salvador|3400|NaN|3400|
|1327|9972|HL1918|iPhone|4|Helena|Chafin|8/10/2018|Salvador|5300|NaN|21200|
|1328|9988|HL1918|iPhone|1|Aline|Morais|5/23/2018|Salvador|5300|NaN|5300|
|1329|9990|HL8851|Notebook|2|Raíssa|Oros|5/20/2018|Salvador|3500|NaN|7000|
|0|0|HL4379|Televisão|5|Gabriel|Thoni|6/30/2018|Curitiba|2500|NaN|12500|
|1|7|HL2714|Tablet|2|Thays|Castro|3/7/2018|Curitiba|1600|NaN|3200|
|2|22|HL1918|iPhone|3|Lucas|Rodrigues|10/8/2018|Curitiba|5300|NaN|15900|
|3|28|HL1918|iPhone|3|Gabriel|Silva|8/21/2018|Curitiba|5300|NaN|15900|
|4|59|HL4379|Televisão|3|Pedro|Conceição|5/16/2018|Curitiba|2500|NaN|7500|
|5|61|HL2714|Tablet|3|Sandy|Ribeiro|5/4/2018|Curitiba|1600|NaN|4800|
|6|64|HL7348|SmartWatch|4|Isabela|Teixeira|8/31/2018|Curitiba|1400|NaN|5600|
|7|66|HL1918|iPhone|3|Carolina|Costa|3/28/2018|Curitiba|5300|NaN|15900|
|8|79|HL8851|Notebook|2|Victor|Gomes|3/23/2018|Curitiba|3500|NaN|7000|
|9|83|HL4379|Televisão|3|João|Alves|5/7/2018|Curitiba|2500|NaN|7500|
|10|85|HL9962|Android|5|Thales|Fanara|4/14/2018|Curitiba|3400|NaN|17000|
|11|89|HL4379|Televisão|3|Jonatas|Essaber|2/3/2018|Curitiba|2500|NaN|7500|
|12|109|HL1918|iPhone|3|Beatriz|Cavalcanti|10/30/2018|Curitiba|5300|NaN|15900|
|13|114|HL1918|iPhone|4|Bianca|Ferezin|6/2/2018|Curitiba|5300|NaN|21200|
|14|122|HL1148|Câmera|2|Laura|Araujo|12/18/2018|Curitiba|2100|NaN|4200|
|15|140|HL4379|Televisão|3|Bernardo|Souza|9/23/2018|Curitiba|2500|NaN|7500|
|16|151|HL7348|SmartWatch|1|João|Capitulo|2/26/2018|Curitiba|1400|NaN|1400|
|17|194|HL8851|Notebook|3|Renan|Melo|12/2/2018|Curitiba|3500|NaN|10500|
|18|224|HL4379|Televisão|5|Sthefeson|Pereira|3/30/2018|Curitiba|2500|NaN|12500|
|19|225|HL7348|SmartWatch|1|Guilherme|Lima|7/16/2018|Curitiba|1400|NaN|1400|
|20|226|HL1918|iPhone|4|Eduardo|Pacheco|12/28/2018|Curitiba|5300|NaN|21200|
|21|235|HL1918|iPhone|1|Anna|Silva|7/20/2018|Curitiba|5300|NaN|5300|
|22|240|HL7348|SmartWatch|4|Giuseppe|Borges|7/11/2018|Curitiba|1400|NaN|5600|
|23|250|HL1918|iPhone|4|Victor|Oliveira|1/30/2018|Curitiba|5300|NaN|21200|
|24|251|HL2714|Tablet|3|João|Menezes|8/3/2018|Curitiba|1600|NaN|4800|
|25|263|HL4379|Televisão|5|Carlos|Melo|8/5/2018|Curitiba|2500|NaN|12500|
|26|266|HL1918|iPhone|5|Roberto|Mattos|2/8/2018|Curitiba|5300|NaN|26500|
|27|277|HL7348|SmartWatch|4|Matheus|Gomes|6/26/2018|Curitiba|1400|NaN|5600|
|28|302|HL8851|Notebook|5|Clara|Silveira|5/15/2018|Curitiba|3500|NaN|17500|
|29|322|HL1148|Câmera|5|Antonio|Bernhardt|1/17/2018|Curitiba|2100|NaN|10500|
|30|326|HL9962|Android|2|Jonatas|Passos|9/18/2018|Curitiba|3400|NaN|6800|
|31|354|HL1918|iPhone|1|Bruno|Ursulino|9/11/2018|Curitiba|5300|NaN|5300|
|32|361|HL8851|Notebook|2|Alon|Guedes|2/25/2018|Curitiba|3500|NaN|7000|
|33|365|HL2714|Tablet|3|Victor|Lira|5/16/2018|Curitiba|1600|NaN|4800|
|34|373|HL1148|Câmera|5|Beatriz|Rocha|12/28/2018|Curitiba|2100|NaN|10500|
|35|413|HL8851|Notebook|5|Luíza|Goulart|3/1/2018|Curitiba|3500|NaN|17500|
|36|415|HL2714|Tablet|2|Carolina|Alfradique|6/9/2018|Curitiba|1600|NaN|3200|
|37|436|HL8851|Notebook|4|Lucas|Monte|9/27/2018|Curitiba|3500|NaN|14000|
|38|440|HL1918|iPhone|5|Marcos|Nucci|5/11/2018|Curitiba|5300|NaN|26500|
|39|444|HL8851|Notebook|5|Alvaro|Kranz|7/21/2018|Curitiba|3500|NaN|17500|
|40|466|HL1918|iPhone|4|Isabella|Santos|9/28/2018|Curitiba|5300|NaN|21200|
|41|468|HL1918|iPhone|4|Vanessa|Neves|8/28/2018|Curitiba|5300|NaN|21200|
|42|481|HL4379|Televisão|5|Ruan|Gonçalves|3/5/2018|Curitiba|2500|NaN|12500|
|43|493|HL1918|iPhone|4|Paulo|Campos|10/6/2018|Curitiba|5300|NaN|21200|
|44|513|HL4379|Televisão|1|Ana|Felippe|11/18/2018|Curitiba|2500|NaN|2500|
|45|536|HL7348|SmartWatch|4|Sthefeson|Barroso|7/21/2018|Curitiba|1400|NaN|5600|
|46|545|HL1918|iPhone|3|Rachel|Silva|8/28/2018|Curitiba|5300|NaN|15900|
|47|553|HL8851|Notebook|4|Mariana|Freire|8/29/2018|Curitiba|3500|NaN|14000|
|48|582|HL1918|iPhone|2|Mayara|Soares|5/3/2018|Curitiba|5300|NaN|10600|
|49|594|HL4379|Televisão|1|Bianca|Paz|12/16/2018|Curitiba|2500|NaN|2500|
|50|607|HL2714|Tablet|4|Mariana|Miranda|9/13/2018|Curitiba|1600|NaN|6400|
|51|612|HL1148|Câmera|3|João|Abraçado|5/27/2018|Curitiba|2100|NaN|6300|
|52|624|HL4379|Televisão|3|Matheus|Delgado|10/16/2018|Curitiba|2500|NaN|7500|
|53|633|HL4379|Televisão|5|Carlos|Silva|2/17/2018|Curitiba|2500|NaN|12500|
|54|634|HL2714|Tablet|5|Clara|Bruno|12/16/2018|Curitiba|1600|NaN|8000|
|55|652|HL1918|iPhone|3|Caroline|Aquino|6/17/2018|Curitiba|5300|NaN|15900|
|56|663|HL1918|iPhone|1|Karine|Barros|6/24/2018|Curitiba|5300|NaN|5300|
|57|666|HL4379|Televisão|4|Maurício|Dias|11/14/2018|Curitiba|2500|NaN|10000|
|58|700|HL8851|Notebook|1|Jéssica|Teixeira|12/26/2018|Curitiba|3500|NaN|3500|
|59|744|HL1918|iPhone|3|Pedro|Sena|1/27/2018|Curitiba|5300|NaN|15900|
|60|758|HL4379|Televisão|1|Alexandre|Rodriguez|6/30/2018|Curitiba|2500|NaN|2500|
|61|764|HL2714|Tablet|4|Anna|Silva|1/18/2018|Curitiba|1600|NaN|6400|
|62|765|HL1148|Câmera|5|Bernardo|Botelho|7/19/2018|Curitiba|2100|NaN|10500|
|63|767|HL9962|Android|5|Filipe|Barros|4/28/2018|Curitiba|3400|NaN|17000|
|64|799|HL4379|Televisão|3|Carlos|Assis|3/16/2018|Curitiba|2500|NaN|7500|
|65|821|HL4379|Televisão|2|Renan|Nascimento|3/22/2018|Curitiba|2500|NaN|5000|
|66|832|HL1148|Câmera|4|Ana|Gomes|7/31/2018|Curitiba|2100|NaN|8400|
|67|836|HL1148|Câmera|3|Adrielle|Vieira|11/3/2018|Curitiba|2100|NaN|6300|
|68|839|HL8851|Notebook|1|Deysiane|Medronho|6/25/2018|Curitiba|3500|NaN|3500|
|69|843|HL1148|Câmera|1|Jeferson|Costa|12/14/2018|Curitiba|2100|NaN|2100|
|70|849|HL1918|iPhone|5|Willian|Albino|8/2/2018|Curitiba|5300|NaN|26500|
|71|851|HL4379|Televisão|2|Luis|Silva|4/18/2018|Curitiba|2500|NaN|5000|
|72|859|HL4379|Televisão|4|Matheus|Tostes|7/20/2018|Curitiba|2500|NaN|10000|
|73|863|HL1918|iPhone|1|Gustavo|Aragão|11/13/2018|Curitiba|5300|NaN|5300|
|74|866|HL9962|Android|3|Ana|Carvalho|12/31/2018|Curitiba|3400|NaN|10200|
|75|870|HL1148|Câmera|1|Wen|Braga|10/5/2018|Curitiba|2100|NaN|2100|
|76|895|HL4379|Televisão|2|Luísa|Fonseca|6/9/2018|Curitiba|2500|NaN|5000|
|77|901|HL1148|Câmera|4|Amanda|Machado|9/2/2018|Curitiba|2100|NaN|8400|
|78|911|HL1918|iPhone|3|Carlos|Souza|2/13/2018|Curitiba|5300|NaN|15900|
|79|928|HL1918|iPhone|4|João|Alves|1/5/2018|Curitiba|5300|NaN|21200|
|80|940|HL2714|Tablet|1|João|Matheus|7/27/2018|Curitiba|1600|NaN|1600|
|81|969|HL1918|iPhone|1|Izabel|Lopes|3/10/2018|Curitiba|5300|NaN|5300|
|82|972|HL8851|Notebook|3|Bernardo|Botelho|12/24/2018|Curitiba|3500|NaN|10500|
|83|982|HL8851|Notebook|5|Hiaiune|Valim|9/20/2018|Curitiba|3500|NaN|17500|
|84|993|HL1918|iPhone|4|Daniela|Rosa|5/1/2018|Curitiba|5300|NaN|21200|
|85|995|HL2714|Tablet|3|Ana|Felippe|9/27/2018|Curitiba|1600|NaN|4800|
|86|999|HL8851|Notebook|5|Raissa|Maia|3/20/2018|Curitiba|3500|NaN|17500|
|87|1002|HL2714|Tablet|4|Adrielle|Vieira|12/26/2018|Curitiba|1600|NaN|6400|
|88|1017|HL4379|Televisão|1|Sandy|Moreira|10/16/2018|Curitiba|2500|NaN|2500|
|89|1020|HL4379|Televisão|2|Fernanda|Rubim|9/29/2018|Curitiba|2500|NaN|5000|
|90|1021|HL1148|Câmera|1|Matheus|Moraes|12/20/2018|Curitiba|2100|NaN|2100|
|91|1031|HL9962|Android|2|Thomaz|Ferreira|12/18/2018|Curitiba|3400|NaN|6800|
|92|1042|HL4379|Televisão|1|Ravena|Bhering|9/29/2018|Curitiba|2500|NaN|2500|
|93|1072|HL9962|Android|3|Alex|Fernandes|6/20/2018|Curitiba|3400|NaN|10200|
|94|1080|HL1918|iPhone|4|Carolina|Siqueira|10/25/2018|Curitiba|5300|NaN|21200|
|95|1093|HL1148|Câmera|3|Stephanie|Novak|12/11/2018|Curitiba|2100|NaN|6300|
|96|1095|HL1148|Câmera|2|Paula|Isbelle|12/27/2018|Curitiba|2100|NaN|4200|
|97|1097|HL4379|Televisão|1|Juliana|Huon|1/3/2018|Curitiba|2500|NaN|2500|
|98|1101|HL2714|Tablet|1|Alex|Fernandes|3/9/2018|Curitiba|1600|NaN|1600|
|99|1105|HL1918|iPhone|3|Izabel|Lopes|2/26/2018|Curitiba|5300|NaN|15900|
|100|1109|HL4379|Televisão|4|Maria|Moita|2/13/2018|Curitiba|2500|NaN|10000|
|101|1113|HL1918|iPhone|4|João|Siqueira|5/10/2018|Curitiba|5300|NaN|21200|
|102|1131|HL1918|iPhone|5|Pedro|Ayres|12/16/2018|Curitiba|5300|NaN|26500|
|103|1158|HL1918|iPhone|5|Catarina|Teixeira|7/19/2018|Curitiba|5300|NaN|26500|
|104|1184|HL2714|Tablet|1|Thomáz|Bôas|7/31/2018|Curitiba|1600|NaN|1600|
|105|1195|HL8851|Notebook|2|Anna|Maia|12/4/2018|Curitiba|3500|NaN|7000|
|106|1215|HL4379|Televisão|5|Erick|Soares|3/15/2018|Curitiba|2500|NaN|12500|
|107|1250|HL7348|SmartWatch|1|Roberto|Nogueira|4/24/2018|Curitiba|1400|NaN|1400|
|108|1254|HL2714|Tablet|4|Giselia|Thiele|9/28/2018|Curitiba|1600|NaN|6400|
|109|1255|HL1918|iPhone|4|Luiz|Mendonça|5/3/2018|Curitiba|5300|NaN|21200|
|110|1260|HL7348|SmartWatch|1|Sylvio|Bernhardt|1/8/2018|Curitiba|1400|NaN|1400|
|111|1268|HL1918|iPhone|3|Vivianne|Rodrigues|7/3/2018|Curitiba|5300|NaN|15900|
|112|1275|HL2714|Tablet|1|Matheus|Moraes|5/14/2018|Curitiba|1600|NaN|1600|
|113|1279|HL9962|Android|2|Mateus|Maia|6/17/2018|Curitiba|3400|NaN|6800|
|114|1285|HL8851|Notebook|2|Ananda|Dias|3/19/2018|Curitiba|3500|NaN|7000|
|115|1295|HL1148|Câmera|1|Isabella|Rodrigues|6/14/2018|Curitiba|2100|NaN|2100|
|116|1310|HL4379|Televisão|4|Larissa|Florim|9/21/2018|Curitiba|2500|NaN|10000|
|117|1313|HL4379|Televisão|5|Andressa|Chou|8/31/2018|Curitiba|2500|NaN|12500|
|118|1318|HL1148|Câmera|3|João|Araujo|2/5/2018|Curitiba|2100|NaN|6300|
|119|1327|HL7348|SmartWatch|2|Renan|Nascimento|5/2/2018|Curitiba|1400|NaN|2800|
|120|1330|HL1918|iPhone|4|Juliana|Silva|1/26/2018|Curitiba|5300|NaN|21200|
|121|1364|HL9962|Android|2|Caroline|Cavalcanti|4/15/2018|Curitiba|3400|NaN|6800|
|122|1366|HL4379|Televisão|5|Isabelle|Firmino|3/10/2018|Curitiba|2500|NaN|12500|
|123|1393|HL1148|Câmera|1|Jonatas|Passos|7/25/2018|Curitiba|2100|NaN|2100|
|124|1402|HL1918|iPhone|4|Wellington|Duarte|12/2/2018|Curitiba|5300|NaN|21200|
|125|1410|HL4379|Televisão|2|Allan|Guedes|8/18/2018|Curitiba|2500|NaN|5000|
|126|1446|HL7348|SmartWatch|5|Gustavo|Aragão|12/31/2018|Curitiba|1400|NaN|7000|
|127|1452|HL1918|iPhone|4|Rafael|Carneiro|5/8/2018|Curitiba|5300|NaN|21200|
|128|1457|HL8851|Notebook|3|Lucas|Valim|10/18/2018|Curitiba|3500|NaN|10500|
|129|1460|HL9962|Android|5|Joyce|Medina|4/21/2018|Curitiba|3400|NaN|17000|
|130|1462|HL1918|iPhone|1|Renan|Freire|2/7/2018|Curitiba|5300|NaN|5300|
|131|1518|HL9962|Android|1|Dykson|Silva|8/31/2018|Curitiba|3400|NaN|3400|
|132|1521|HL8851|Notebook|4|Marcelo|Rosa|12/23/2018|Curitiba|3500|NaN|14000|
|133|1534|HL4379|Televisão|4|Breno|Quinto|12/1/2018|Curitiba|2500|NaN|10000|
|134|1545|HL4379|Televisão|5|Pedro|Conceição|10/19/2018|Curitiba|2500|NaN|12500|
|135|1553|HL4379|Televisão|2|Danilo|Mendonça|3/23/2018|Curitiba|2500|NaN|5000|
|136|1555|HL8851|Notebook|3|Thomáz|Bôas|6/19/2018|Curitiba|3500|NaN|10500|
|137|1571|HL8851|Notebook|2|Diogo|Peixoto|10/12/2018|Curitiba|3500|NaN|7000|
|138|1573|HL1918|iPhone|2|Raul|Junqueira|10/27/2018|Curitiba|5300|NaN|10600|
|139|1577|HL9962|Android|1|Raphael|Kurtz|8/19/2018|Curitiba|3400|NaN|3400|
|140|1587|HL1918|iPhone|3|Luana|Santana|6/3/2018|Curitiba|5300|NaN|15900|
|141|1593|HL1918|iPhone|1|Thaís|Pereira|5/28/2018|Curitiba|5300|NaN|5300|
|142|1650|HL1918|iPhone|4|Gabriel|Puntel|1/17/2018|Curitiba|5300|NaN|21200|
|143|1656|HL8851|Notebook|5|Rafael|Rocha|10/22/2018|Curitiba|3500|NaN|17500|
|144|1661|HL8851|Notebook|4|Cícero|Ramos|8/7/2018|Curitiba|3500|NaN|14000|
|145|1679|HL2714|Tablet|2|Lucas|Monte|6/27/2018|Curitiba|1600|NaN|3200|
|146|1691|HL2714|Tablet|4|Lara|Moreira|7/7/2018|Curitiba|1600|NaN|6400|
|147|1694|HL1918|iPhone|5|Bárbara|Lima|11/14/2018|Curitiba|5300|NaN|26500|
|148|1775|HL1918|iPhone|1|Viviane|Cunha|3/8/2018|Curitiba|5300|NaN|5300|
|149|1795|HL1918|iPhone|4|Rafaela|Gomes|12/11/2018|Curitiba|5300|NaN|21200|
|150|1825|HL2714|Tablet|1|Rilson|Dias|3/31/2018|Curitiba|1600|NaN|1600|
|151|1837|HL7348|SmartWatch|3|Gabriel|Silva|12/23/2018|Curitiba|1400|NaN|4200|
|152|1840|HL9962|Android|5|Marcelo|Pereira|10/25/2018|Curitiba|3400|NaN|17000|
|153|1851|HL9962|Android|3|Rafaela|Ferreira|3/7/2018|Curitiba|3400|NaN|10200|
|154|1863|HL1918|iPhone|3|Anderson|Martins|5/29/2018|Curitiba|5300|NaN|15900|
|155|1869|HL1918|iPhone|2|Mariana|Sousa|7/3/2018|Curitiba|5300|NaN|10600|
|156|1885|HL4379|Televisão|3|Larissa|Jesus|3/8/2018|Curitiba|2500|NaN|7500|
|157|1897|HL1918|iPhone|2|Renan|Melo|6/23/2018|Curitiba|5300|NaN|10600|
|158|1921|HL8851|Notebook|5|Larissa|Jesus|10/12/2018|Curitiba|3500|NaN|17500|
|159|1926|HL4379|Televisão|2|Lucas|Lima|11/2/2018|Curitiba|2500|NaN|5000|
|160|1947|HL4379|Televisão|3|Glenda|Santos|9/3/2018|Curitiba|2500|NaN|7500|
|161|1958|HL7348|SmartWatch|2|Rafaella|Mello|5/20/2018|Curitiba|1400|NaN|2800|
|162|1985|HL1148|Câmera|2|Caroll|Johnson|9/8/2018|Curitiba|2100|NaN|4200|
|163|2004|HL1148|Câmera|1|Pedro|Oliveira|1/17/2018|Curitiba|2100|NaN|2100|
|164|2024|HL8851|Notebook|5|Caio|Moraes|3/25/2018|Curitiba|3500|NaN|17500|
|165|2029|HL1148|Câmera|4|Carlos|Galvão|12/21/2018|Curitiba|2100|NaN|8400|
|166|2046|HL1918|iPhone|4|José|Carvalho|9/15/2018|Curitiba|5300|NaN|21200|
|167|2050|HL8851|Notebook|4|Lucas|Destri|9/10/2018|Curitiba|3500|NaN|14000|
|168|2056|HL8851|Notebook|1|Caio|Moura|12/12/2018|Curitiba|3500|NaN|3500|
|169|2058|HL1918|iPhone|3|Lucas|Freitas|4/19/2018|Curitiba|5300|NaN|15900|
|170|2060|HL4379|Televisão|1|Raphael|Guedes|10/23/2018|Curitiba|2500|NaN|2500|
|171|2084|HL9962|Android|5|Luiza|Cabral|3/4/2018|Curitiba|3400|NaN|17000|
|172|2093|HL9962|Android|1|Rodrigo|Silva|10/7/2018|Curitiba|3400|NaN|3400|
|173|2096|HL1918|iPhone|5|Roberta|Pimenta|3/21/2018|Curitiba|5300|NaN|26500|
|174|2133|HL1918|iPhone|1|Sthefeson|Barroso|8/12/2018|Curitiba|5300|NaN|5300|
|175|2137|HL4379|Televisão|4|Danilo|Mendonça|2/3/2018|Curitiba|2500|NaN|10000|
|176|2138|HL4379|Televisão|3|Carolina|Alfradique|1/10/2018|Curitiba|2500|NaN|7500|
|177|2139|HL7348|SmartWatch|3|Victor|Zakhm|11/13/2018|Curitiba|1400|NaN|4200|
|178|2150|HL8851|Notebook|2|Sarah|Souza|1/21/2018|Curitiba|3500|NaN|7000|
|179|2168|HL8851|Notebook|3|Carlos|Assis|8/5/2018|Curitiba|3500|NaN|10500|
|180|2236|HL9962|Android|1|Eduardo|Vargas|7/29/2018|Curitiba|3400|NaN|3400|
|181|2241|HL7348|SmartWatch|3|Gabriel|Thoni|2/24/2018|Curitiba|1400|NaN|4200|
|182|2249|HL8851|Notebook|5|Alexandre|Dantas|6/7/2018|Curitiba|3500|NaN|17500|
|183|2250|HL1148|Câmera|1|Hygor|Essaber|1/26/2018|Curitiba|2100|NaN|2100|
|184|2274|HL7348|SmartWatch|2|Lucas|Machado|7/30/2018|Curitiba|1400|NaN|2800|
|185|2289|HL4379|Televisão|3|Diego|Rodrigues|8/9/2018|Curitiba|2500|NaN|7500|
|186|2296|HL4379|Televisão|5|Jessica|Cordovil|12/7/2018|Curitiba|2500|NaN|12500|
|187|2300|HL1918|iPhone|4|Caio|Fernandes|12/2/2018|Curitiba|5300|NaN|21200|
|188|2304|HL9962|Android|2|João|Capitulo|6/21/2018|Curitiba|3400|NaN|6800|
|189|2317|HL2714|Tablet|2|Isabela|Resende|2/16/2018|Curitiba|1600|NaN|3200|
|190|2329|HL1918|iPhone|3|Carolina|Abrahão|10/25/2018|Curitiba|5300|NaN|15900|
|191|2360|HL4379|Televisão|3|Gabriel|Azevedo|5/1/2018|Curitiba|2500|NaN|7500|
|192|2361|HL1918|iPhone|2|Caio|Cardoso|10/3/2018|Curitiba|5300|NaN|10600|
|193|2364|HL1918|iPhone|2|Miguel|Carneiro|11/7/2018|Curitiba|5300|NaN|10600|
|194|2371|HL8851|Notebook|1|Raissa|Pinheiro|6/12/2018|Curitiba|3500|NaN|3500|
|195|2387|HL1918|iPhone|4|Nicolas|Monteiro|3/1/2018|Curitiba|5300|NaN|21200|
|196|2403|HL9962|Android|4|Gabriel|Soares|4/11/2018|Curitiba|3400|NaN|13600|
|197|2425|HL1918|iPhone|3|Pedro|Pereira|11/11/2018|Curitiba|5300|NaN|15900|
|198|2427|HL7348|SmartWatch|1|Bianca|Ferezin|12/24/2018|Curitiba|1400|NaN|1400|
|199|2434|HL9962|Android|3|Camilla|Guimarães|11/5/2018|Curitiba|3400|NaN|10200|
|200|2437|HL2714|Tablet|5|Lucas|Rodrigues|5/23/2018|Curitiba|1600|NaN|8000|
|201|2440|HL8851|Notebook|4|Rafaella|Mello|1/12/2018|Curitiba|3500|NaN|14000|
|202|2467|HL1148|Câmera|2|Vanessa|Bach|4/14/2018|Curitiba|2100|NaN|4200|
|203|2475|HL2714|Tablet|5|Breno|Farias|5/29/2018|Curitiba|1600|NaN|8000|
|204|2492|HL9962|Android|5|Caroline|Pinto|9/4/2018|Curitiba|3400|NaN|17000|
|205|2503|HL7348|SmartWatch|3|Victor|Franco|1/25/2018|Curitiba|1400|NaN|4200|
|206|2510|HL1918|iPhone|2|Jeferson|Sone|10/16/2018|Curitiba|5300|NaN|10600|
|207|2512|HL1918|iPhone|4|Kim|Ferreira|4/18/2018|Curitiba|5300|NaN|21200|
|208|2514|HL1918|iPhone|5|Débora|Lopes|6/17/2018|Curitiba|5300|NaN|26500|
|209|2527|HL4379|Televisão|3|Izabel|Lopes|5/18/2018|Curitiba|2500|NaN|7500|
|210|2536|HL1918|iPhone|5|Diego|Rodrigues|3/18/2018|Curitiba|5300|NaN|26500|
|211|2544|HL1148|Câmera|5|Cícero|Lima|5/5/2018|Curitiba|2100|NaN|10500|
|212|2549|HL2714|Tablet|4|Philipe|Morete|8/19/2018|Curitiba|1600|NaN|6400|
|213|2552|HL2714|Tablet|3|Izabel|Miura|8/30/2018|Curitiba|1600|NaN|4800|
|214|2594|HL1148|Câmera|1|Cézar|Santos|6/5/2018|Curitiba|2100|NaN|2100|
|215|2597|HL8851|Notebook|2|Luis|Souza|5/26/2018|Curitiba|3500|NaN|7000|
|216|2606|HL4379|Televisão|4|Adrielle|Forte|2/9/2018|Curitiba|2500|NaN|10000|
|217|2608|HL1148|Câmera|4|Célio|Xavier|12/30/2018|Curitiba|2100|NaN|8400|
|218|2642|HL1918|iPhone|2|Nathalia|Ventura|8/6/2018|Curitiba|5300|NaN|10600|
|219|2652|HL4379|Televisão|5|Lucas|Rodrigues|2/14/2018|Curitiba|2500|NaN|12500|
|220|2659|HL1918|iPhone|4|Priscila|Carvalho|4/26/2018|Curitiba|5300|NaN|21200|
|221|2661|HL7348|SmartWatch|3|Helena|Chafin|10/14/2018|Curitiba|1400|NaN|4200|
|222|2670|HL7348|SmartWatch|2|Anna|Maia|2/1/2018|Curitiba|1400|NaN|2800|
|223|2684|HL4379|Televisão|1|Wen|Santos|7/2/2018|Curitiba|2500|NaN|2500|
|224|2697|HL4379|Televisão|3|Carlos|Portela|6/23/2018|Curitiba|2500|NaN|7500|
|225|2733|HL1918|iPhone|5|Gabriel|Rubim|11/7/2018|Curitiba|5300|NaN|26500|
|226|2750|HL7348|SmartWatch|3|Júlio|Freire|5/12/2018|Curitiba|1400|NaN|4200|
|227|2757|HL7348|SmartWatch|2|Cícero|Lima|3/6/2018|Curitiba|1400|NaN|2800|
|228|2785|HL1918|iPhone|4|Kimberly|Sad|2/10/2018|Curitiba|5300|NaN|21200|
|229|2789|HL1918|iPhone|3|Guilherme|Vianna|2/8/2018|Curitiba|5300|NaN|15900|
|230|2803|HL1918|iPhone|1|Jonatas|Passos|8/3/2018|Curitiba|5300|NaN|5300|
|231|2807|HL1918|iPhone|3|João|Peçanha|6/18/2018|Curitiba|5300|NaN|15900|
|232|2816|HL1918|iPhone|3|Gustavo|Gomes|11/11/2018|Curitiba|5300|NaN|15900|
|233|2848|HL4379|Televisão|1|Thayna|Martins|12/28/2018|Curitiba|2500|NaN|2500|
|234|2849|HL4379|Televisão|3|João|Castilho|3/9/2018|Curitiba|2500|NaN|7500|
|235|2852|HL4379|Televisão|2|Tiago|Pereira|10/26/2018|Curitiba|2500|NaN|5000|
|236|2856|HL4379|Televisão|4|Raul|Junqueira|5/7/2018|Curitiba|2500|NaN|10000|
|237|2870|HL1918|iPhone|3|Carlos|Souza|10/24/2018|Curitiba|5300|NaN|15900|
|238|2872|HL7348|SmartWatch|3|Luiza|Cavalcanti|8/18/2018|Curitiba|1400|NaN|4200|
|239|2882|HL7348|SmartWatch|5|Glenda|Santos|5/29/2018|Curitiba|1400|NaN|7000|
|240|2883|HL8851|Notebook|4|Juliana|Goes|9/20/2018|Curitiba|3500|NaN|14000|
|241|2902|HL8851|Notebook|5|Ana|Campos|3/3/2018|Curitiba|3500|NaN|17500|
|242|2936|HL9962|Android|3|Sylvio|Bernhardt|3/14/2018|Curitiba|3400|NaN|10200|
|243|2943|HL1918|iPhone|1|Camilla|Cardeman|5/16/2018|Curitiba|5300|NaN|5300|
|244|2950|HL1918|iPhone|4|Alon|Pestana|2/20/2018|Curitiba|5300|NaN|21200|
|245|2953|HL1918|iPhone|2|Anna|Maia|3/25/2018|Curitiba|5300|NaN|10600|
|246|2957|HL1918|iPhone|2|Thales|Santos|6/24/2018|Curitiba|5300|NaN|10600|
|247|3032|HL4379|Televisão|5|Clara|Silveira|9/9/2018|Curitiba|2500|NaN|12500|
|248|3047|HL4379|Televisão|2|Isabel|Mesquita|1/3/2018|Curitiba|2500|NaN|5000|
|249|3070|HL1918|iPhone|3|Pedro|Jorge|1/11/2018|Curitiba|5300|NaN|15900|
|250|3152|HL1918|iPhone|1|Renan|Freire|5/21/2018|Curitiba|5300|NaN|5300|
|251|3153|HL2714|Tablet|2|Isabella|Scalabrin|11/29/2018|Curitiba|1600|NaN|3200|
|252|3196|HL4379|Televisão|2|Leonardo|Ferreira|3/25/2018|Curitiba|2500|NaN|5000|
|253|3197|HL4379|Televisão|4|Daniel|Terra|5/29/2018|Curitiba|2500|NaN|10000|
|254|3201|HL1918|iPhone|3|Rodrigo|Feijo|2/6/2018|Curitiba|5300|NaN|15900|
|255|3206|HL7348|SmartWatch|2|Igor|Lima|12/21/2018|Curitiba|1400|NaN|2800|
|256|3242|HL7348|SmartWatch|2|Luana|Santana|9/23/2018|Curitiba|1400|NaN|2800|
|257|3261|HL4379|Televisão|4|Bruno|Barcessat|6/19/2018|Curitiba|2500|NaN|10000|
|258|3268|HL9962|Android|5|João|Silva|2/14/2018|Curitiba|3400|NaN|17000|
|259|3279|HL9962|Android|3|Matheus|Sapir|8/20/2018|Curitiba|3400|NaN|10200|
|260|3289|HL1148|Câmera|1|Caio|Silva|8/8/2018|Curitiba|2100|NaN|2100|
|261|3310|HL1918|iPhone|1|William|Mendonça|10/16/2018|Curitiba|5300|NaN|5300|
|262|3338|HL1918|iPhone|3|Matheus|Ramos|1/7/2018|Curitiba|5300|NaN|15900|
|263|3341|HL4379|Televisão|4|Norman|Jimbo|7/12/2018|Curitiba|2500|NaN|10000|
|264|3350|HL7348|SmartWatch|4|Maria|Motta|2/27/2018|Curitiba|1400|NaN|5600|
|265|3353|HL8851|Notebook|2|Mariane|Ferreira|3/13/2018|Curitiba|3500|NaN|7000|
|266|3359|HL8851|Notebook|4|Marcelo|Borges|9/28/2018|Curitiba|3500|NaN|14000|
|267|3372|HL4379|Televisão|4|Giselia|Thiele|3/30/2018|Curitiba|2500|NaN|10000|
|268|3396|HL4379|Televisão|3|Vanessa|Bach|4/15/2018|Curitiba|2500|NaN|7500|
|269|3398|HL8851|Notebook|5|João|Júnior|8/27/2018|Curitiba|3500|NaN|17500|
|270|3402|HL1918|iPhone|5|Mariana|Baptista|8/11/2018|Curitiba|5300|NaN|26500|
|271|3412|HL2714|Tablet|4|Amanda|Delgado|7/11/2018|Curitiba|1600|NaN|6400|
|272|3425|HL9962|Android|5|Gabriel|Silva|8/29/2018|Curitiba|3400|NaN|17000|
|273|3432|HL1918|iPhone|5|Eduardo|Nunes|4/2/2018|Curitiba|5300|NaN|26500|
|274|3443|HL1918|iPhone|3|Rafael|Rocha|10/21/2018|Curitiba|5300|NaN|15900|
|275|3452|HL1918|iPhone|2|Anna|Maia|11/13/2018|Curitiba|5300|NaN|10600|
|276|3469|HL1148|Câmera|5|João|Alves|5/7/2018|Curitiba|2100|NaN|10500|
|277|3483|HL1148|Câmera|2|Luis|Garcia|8/16/2018|Curitiba|2100|NaN|4200|
|278|3505|HL9962|Android|5|João|Siqueira|2/22/2018|Curitiba|3400|NaN|17000|
|279|3508|HL4379|Televisão|3|Breno|Farias|1/24/2018|Curitiba|2500|NaN|7500|
|280|3509|HL4379|Televisão|1|Carolina|Santos|6/12/2018|Curitiba|2500|NaN|2500|
|281|3510|HL9962|Android|5|Pedro|Oliveira|11/15/2018|Curitiba|3400|NaN|17000|
|282|3532|HL2714|Tablet|4|Stephanie|Oliveira|3/3/2018|Curitiba|1600|NaN|6400|
|283|3538|HL8851|Notebook|3|Julia|Leite|1/12/2018|Curitiba|3500|NaN|10500|
|284|3541|HL8851|Notebook|3|Pedro|Santana|8/21/2018|Curitiba|3500|NaN|10500|
|285|3546|HL1148|Câmera|5|Patrícia|Ferreira|2/20/2018|Curitiba|2100|NaN|10500|
|286|3552|HL8851|Notebook|3|Renan|Firmino|10/21/2018|Curitiba|3500|NaN|10500|
|287|3558|HL2714|Tablet|3|Anna|Silva|7/1/2018|Curitiba|1600|NaN|4800|
|288|3573|HL1918|iPhone|2|Daniel|Cardoso|7/13/2018|Curitiba|5300|NaN|10600|
|289|3582|HL9962|Android|2|Raphael|Kurtz|7/25/2018|Curitiba|3400|NaN|6800|
|290|3619|HL4379|Televisão|3|Raissa|Negrelli|7/18/2018|Curitiba|2500|NaN|7500|
|291|3624|HL2714|Tablet|2|Eduardo|Nunes|7/24/2018|Curitiba|1600|NaN|3200|
|292|3668|HL4379|Televisão|2|Ana|Campos|8/27/2018|Curitiba|2500|NaN|5000|
|293|3705|HL8851|Notebook|1|Gabriela|Cavalcanti|7/28/2018|Curitiba|3500|NaN|3500|
|294|3715|HL1148|Câmera|1|Ana|Silva|12/29/2018|Curitiba|2100|NaN|2100|
|295|3722|HL8851|Notebook|2|Gabriela|Aliani|6/2/2018|Curitiba|3500|NaN|7000|
|296|3747|HL4379|Televisão|2|Alvaro|Kranz|6/28/2018|Curitiba|2500|NaN|5000|
|297|3759|HL4379|Televisão|5|Rebeca|Reis|11/8/2018|Curitiba|2500|NaN|12500|
|298|3765|HL9962|Android|2|Rafaela|Ferreira|9/14/2018|Curitiba|3400|NaN|6800|
|299|3774|HL4379|Televisão|5|Isabela|Chagas|11/3/2018|Curitiba|2500|NaN|12500|
|300|3803|HL4379|Televisão|1|Roberta|Nogueira|1/29/2018|Curitiba|2500|NaN|2500|
|301|3810|HL8851|Notebook|1|Raphael|Guedes|12/10/2018|Curitiba|3500|NaN|3500|
|302|3814|HL9962|Android|5|Rafaela|Feio|12/8/2018|Curitiba|3400|NaN|17000|
|303|3826|HL1148|Câmera|1|Rogério|Gentile|5/2/2018|Curitiba|2100|NaN|2100|
|304|3829|HL4379|Televisão|4|Desirée|Heimlich|11/8/2018|Curitiba|2500|NaN|10000|
|305|3848|HL7348|SmartWatch|4|Luana|Santos|7/12/2018|Curitiba|1400|NaN|5600|
|306|3865|HL4379|Televisão|4|Lucas|Baptista|3/10/2018|Curitiba|2500|NaN|10000|
|307|3877|HL7348|SmartWatch|5|Eduardo|Soares|7/11/2018|Curitiba|1400|NaN|7000|
|308|3888|HL1918|iPhone|4|Natali|Rangel|10/30/2018|Curitiba|5300|NaN|21200|
|309|3897|HL1918|iPhone|1|Natalia|Andrade|8/13/2018|Curitiba|5300|NaN|5300|
|310|3904|HL4379|Televisão|4|Jonatas|Essaber|8/19/2018|Curitiba|2500|NaN|10000|
|311|3938|HL9962|Android|2|Gabrielle|Wanderley|7/27/2018|Curitiba|3400|NaN|6800|
|312|3944|HL4379|Televisão|1|Gustavo|Junior|9/1/2018|Curitiba|2500|NaN|2500|
|313|3956|HL8851|Notebook|5|Mayara|Soares|10/31/2018|Curitiba|3500|NaN|17500|
|314|3963|HL7348|SmartWatch|1|Camilla|Cardeman|12/1/2018|Curitiba|1400|NaN|1400|
|315|3964|HL2714|Tablet|2|Norman|Jimbo|8/25/2018|Curitiba|1600|NaN|3200|
|316|3994|HL1918|iPhone|1|Rafael|Guimarães|5/24/2018|Curitiba|5300|NaN|5300|
|317|3998|HL7348|SmartWatch|5|Isabella|Scalabrin|11/12/2018|Curitiba|1400|NaN|7000|
|318|4012|HL8851|Notebook|1|Guilherme|Seixas|6/8/2018|Curitiba|3500|NaN|3500|
|319|4064|HL1918|iPhone|1|Carolina|Motta|10/16/2018|Curitiba|5300|NaN|5300|
|320|4065|HL9962|Android|4|Rubens|Valente|6/28/2018|Curitiba|3400|NaN|13600|
|321|4068|HL4379|Televisão|5|Philipe|Morete|12/3/2018|Curitiba|2500|NaN|12500|
|322|4092|HL4379|Televisão|3|Rafael|Rocha|12/17/2018|Curitiba|2500|NaN|7500|
|323|4095|HL1918|iPhone|4|Myllena|Carneiro|1/27/2018|Curitiba|5300|NaN|21200|
|324|4116|HL2714|Tablet|2|Luiz|Limp|5/7/2018|Curitiba|1600|NaN|3200|
|325|4141|HL4379|Televisão|4|Matheus|Santos|5/30/2018|Curitiba|2500|NaN|10000|
|326|4144|HL2714|Tablet|3|Ana|Felippe|10/24/2018|Curitiba|1600|NaN|4800|
|327|4176|HL1918|iPhone|5|Caroline|Aquino|6/30/2018|Curitiba|5300|NaN|26500|
|328|4199|HL4379|Televisão|3|Lais|Candido|8/10/2018|Curitiba|2500|NaN|7500|
|329|4203|HL2714|Tablet|1|Eduardo|Soares|6/14/2018|Curitiba|1600|NaN|1600|
|330|4210|HL1148|Câmera|3|Júlio|Fraga|5/4/2018|Curitiba|2100|NaN|6300|
|331|4221|HL1918|iPhone|1|Amanda|Amaral|4/12/2018|Curitiba|5300|NaN|5300|
|332|4222|HL1918|iPhone|1|Stela|Mendonça|8/23/2018|Curitiba|5300|NaN|5300|
|333|4246|HL1918|iPhone|5|Tayla|Lima|5/16/2018|Curitiba|5300|NaN|26500|
|334|4298|HL4379|Televisão|2|Juliana|Hollander|4/15/2018|Curitiba|2500|NaN|5000|
|335|4312|HL1918|iPhone|5|Anderson|Martins|4/20/2018|Curitiba|5300|NaN|26500|
|336|4344|HL8851|Notebook|3|Alessandra|Martins|6/20/2018|Curitiba|3500|NaN|10500|
|337|4345|HL2714|Tablet|5|Priscila|Carvalho|2/23/2018|Curitiba|1600|NaN|8000|
|338|4346|HL9962|Android|3|Juliana|Silva|8/2/2018|Curitiba|3400|NaN|10200|
|339|4387|HL1148|Câmera|3|Luis|Garcia|5/16/2018|Curitiba|2100|NaN|6300|
|340|4394|HL1918|iPhone|5|Adriana|Passos|4/16/2018|Curitiba|5300|NaN|26500|
|341|4398|HL1918|iPhone|2|Julia|Figueiredo|1/30/2018|Curitiba|5300|NaN|10600|
|342|4424|HL4379|Televisão|5|Victor|Lira|3/12/2018|Curitiba|2500|NaN|12500|
|343|4425|HL1918|iPhone|5|Marina|Delgado|12/7/2018|Curitiba|5300|NaN|26500|
|344|4432|HL1918|iPhone|3|Daniel|Felippe|1/3/2018|Curitiba|5300|NaN|15900|
|345|4442|HL4379|Televisão|2|Marina|Marins|2/23/2018|Curitiba|2500|NaN|5000|
|346|4467|HL4379|Televisão|1|Renan|Melo|1/24/2018|Curitiba|2500|NaN|2500|
|347|4479|HL9962|Android|2|Cláudio|Aragão|10/13/2018|Curitiba|3400|NaN|6800|
|348|4482|HL8851|Notebook|4|Caio|Moraes|7/25/2018|Curitiba|3500|NaN|14000|
|349|4489|HL1918|iPhone|1|Isabelle|Gonçalves|9/8/2018|Curitiba|5300|NaN|5300|
|350|4500|HL4379|Televisão|4|Luis|Villanova|10/23/2018|Curitiba|2500|NaN|10000|
|351|4505|HL4379|Televisão|4|Renan|Nascimento|3/25/2018|Curitiba|2500|NaN|10000|
|352|4539|HL9962|Android|3|Hygor|Essaber|6/28/2018|Curitiba|3400|NaN|10200|
|353|4569|HL8851|Notebook|4|Lívia|Tanaka|1/8/2018|Curitiba|3500|NaN|14000|
|354|4601|HL1918|iPhone|5|Daniel|Sousa|4/17/2018|Curitiba|5300|NaN|26500|
|355|4603|HL1918|iPhone|5|Bruno|Ferreira|5/7/2018|Curitiba|5300|NaN|26500|
|356|4617|HL4379|Televisão|2|Gabriel|Pereira|11/17/2018|Curitiba|2500|NaN|5000|
|357|4621|HL1918|iPhone|4|Jonatas|Essaber|1/21/2018|Curitiba|5300|NaN|21200|
|358|4633|HL7348|SmartWatch|4|Daniel|Costa|8/26/2018|Curitiba|1400|NaN|5600|
|359|4664|HL2714|Tablet|3|Vanessa|Bach|7/14/2018|Curitiba|1600|NaN|4800|
|360|4675|HL1918|iPhone|1|Pedro|Martins|1/20/2018|Curitiba|5300|NaN|5300|
|361|4703|HL1918|iPhone|2|Carolina|Motta|2/13/2018|Curitiba|5300|NaN|10600|
|362|4708|HL8851|Notebook|5|Anízio|Carvalho|2/11/2018|Curitiba|3500|NaN|17500|
|363|4729|HL7348|SmartWatch|1|Katharina|Barros|1/3/2018|Curitiba|1400|NaN|1400|
|364|4743|HL8851|Notebook|3|Arthur|Portela|2/27/2018|Curitiba|3500|NaN|10500|
|365|4752|HL9962|Android|2|Rodrigo|Feijo|1/16/2018|Curitiba|3400|NaN|6800|
|366|4762|HL1918|iPhone|2|David|Vasconcelos|3/21/2018|Curitiba|5300|NaN|10600|
|367|4772|HL8851|Notebook|3|Adrielle|Gabriel|6/22/2018|Curitiba|3500|NaN|10500|
|368|4773|HL4379|Televisão|1|Gustavo|Erthal|9/8/2018|Curitiba|2500|NaN|2500|
|369|4786|HL7348|SmartWatch|4|João|Araujo|1/13/2018|Curitiba|1400|NaN|5600|
|370|4798|HL4379|Televisão|1|Breno|Quinto|11/21/2018|Curitiba|2500|NaN|2500|
|371|4802|HL2714|Tablet|2|Juliana|Guimarães|12/31/2018|Curitiba|1600|NaN|3200|
|372|4807|HL2714|Tablet|1|Anderson|Martins|2/23/2018|Curitiba|1600|NaN|1600|
|373|4828|HL1918|iPhone|4|Gabriela|Cavalcanti|6/12/2018|Curitiba|5300|NaN|21200|
|374|4834|HL1918|iPhone|2|Alberto|Silveira|10/25/2018|Curitiba|5300|NaN|10600|
|375|4838|HL2714|Tablet|3|Debora|Silva|12/19/2018|Curitiba|1600|NaN|4800|
|376|4846|HL4379|Televisão|3|Ana|Carvalho|10/6/2018|Curitiba|2500|NaN|7500|
|377|4867|HL8851|Notebook|4|Deysiane|Medronho|11/11/2018|Curitiba|3500|NaN|14000|
|378|4868|HL7348|SmartWatch|4|Luiz|Almeida|4/2/2018|Curitiba|1400|NaN|5600|
|379|4895|HL8851|Notebook|3|Arthur|Souza|2/10/2018|Curitiba|3500|NaN|10500|
|380|4921|HL1918|iPhone|4|Bernardo|Botelho|7/25/2018|Curitiba|5300|NaN|21200|
|381|4932|HL1148|Câmera|4|Breno|Britto|10/24/2018|Curitiba|2100|NaN|8400|
|382|4933|HL1148|Câmera|1|Vanessa|Rodrigues|11/28/2018|Curitiba|2100|NaN|2100|
|383|4948|HL1918|iPhone|1|Miguel|Carneiro|7/19/2018|Curitiba|5300|NaN|5300|
|384|4951|HL1918|iPhone|5|Juliana|Silva|2/18/2018|Curitiba|5300|NaN|26500|
|385|4958|HL1918|iPhone|4|Carolina|Bernardes|3/2/2018|Curitiba|5300|NaN|21200|
|386|4965|HL8851|Notebook|5|Marcelo|Magalhães|11/8/2018|Curitiba|3500|NaN|17500|
|387|4976|HL2714|Tablet|4|Isabela|Resende|7/4/2018|Curitiba|1600|NaN|6400|
|388|4990|HL4379|Televisão|3|João|Bach|2/2/2018|Curitiba|2500|NaN|7500|
|389|4997|HL2714|Tablet|4|Mayara|Soares|10/27/2018|Curitiba|1600|NaN|6400|
|390|5009|HL1918|iPhone|5|Sylvio|Bernhardt|5/21/2018|Curitiba|5300|NaN|26500|
|391|5030|HL4379|Televisão|4|Renan|Firmino|1/10/2018|Curitiba|2500|NaN|10000|
|392|5064|HL4379|Televisão|2|Hiaiune|Valim|3/19/2018|Curitiba|2500|NaN|5000|
|393|5065|HL7348|SmartWatch|5|Henrique|Lencastre|12/20/2018|Curitiba|1400|NaN|7000|
|394|5089|HL7348|SmartWatch|1|Juan|Fernandes|7/16/2018|Curitiba|1400|NaN|1400|
|395|5098|HL4379|Televisão|3|João|Aires|2/4/2018|Curitiba|2500|NaN|7500|
|396|5104|HL1918|iPhone|5|Diego|Mello|4/15/2018|Curitiba|5300|NaN|26500|
|397|5191|HL1918|iPhone|2|Caio|Affonso|5/12/2018|Curitiba|5300|NaN|10600|
|398|5195|HL9962|Android|2|Raissa|Sales|11/19/2018|Curitiba|3400|NaN|6800|
|399|5213|HL4379|Televisão|2|Philipe|Morete|8/20/2018|Curitiba|2500|NaN|5000|
|400|5217|HL4379|Televisão|4|Arthur|Souza|12/26/2018|Curitiba|2500|NaN|10000|
|401|5220|HL4379|Televisão|5|Mariana|Rotava|1/26/2018|Curitiba|2500|NaN|12500|
|402|5262|HL1918|iPhone|5|Adriane|Chagas|9/7/2018|Curitiba|5300|NaN|26500|
|403|5270|HL8851|Notebook|3|João|Bach|1/7/2018|Curitiba|3500|NaN|10500|
|404|5279|HL1918|iPhone|3|Andressa|Chou|3/15/2018|Curitiba|5300|NaN|15900|
|405|5292|HL1148|Câmera|1|Marina|Gama|6/21/2018|Curitiba|2100|NaN|2100|
|406|5310|HL4379|Televisão|4|Beatriz|Cavalcanti|5/21/2018|Curitiba|2500|NaN|10000|
|407|5319|HL7348|SmartWatch|4|Pedro|Dalforne|2/8/2018|Curitiba|1400|NaN|5600|
|408|5327|HL9962|Android|2|Daniel|Costa|10/7/2018|Curitiba|3400|NaN|6800|
|409|5339|HL1918|iPhone|4|Isabela|Resende|9/29/2018|Curitiba|5300|NaN|21200|
|410|5344|HL2714|Tablet|2|Wen|Santos|4/12/2018|Curitiba|1600|NaN|3200|
|411|5378|HL8851|Notebook|2|Mariana|Freire|8/4/2018|Curitiba|3500|NaN|7000|
|412|5386|HL2714|Tablet|1|Bárbara|Lima|4/12/2018|Curitiba|1600|NaN|1600|
|413|5393|HL7348|SmartWatch|4|Beatriz|Nogueira|3/24/2018|Curitiba|1400|NaN|5600|
|414|5399|HL1918|iPhone|3|Helena|Chafin|2/23/2018|Curitiba|5300|NaN|15900|
|415|5404|HL4379|Televisão|3|Fernanda|Junior|6/29/2018|Curitiba|2500|NaN|7500|
|416|5406|HL1148|Câmera|1|Luiz|Freire|3/12/2018|Curitiba|2100|NaN|2100|
|417|5416|HL1918|iPhone|4|Isabel|Mesquita|7/5/2018|Curitiba|5300|NaN|21200|
|418|5417|HL8851|Notebook|1|Amanda|Gontijo|5/26/2018|Curitiba|3500|NaN|3500|
|419|5446|HL8851|Notebook|4|Raul|Junqueira|11/20/2018|Curitiba|3500|NaN|14000|
|420|5459|HL4379|Televisão|2|Daniel|Cardoso|10/2/2018|Curitiba|2500|NaN|5000|
|421|5461|HL1918|iPhone|4|Mariane|Ferreira|2/19/2018|Curitiba|5300|NaN|21200|
|422|5470|HL7348|SmartWatch|1|Ives|Barbosa|3/18/2018|Curitiba|1400|NaN|1400|
|423|5477|HL1918|iPhone|2|Paula|Calbucci|7/6/2018|Curitiba|5300|NaN|10600|
|424|5478|HL7348|SmartWatch|2|Roberto|Tiradentes|4/8/2018|Curitiba|1400|NaN|2800|
|425|5483|HL1918|iPhone|3|Rodrigo|Feijo|10/7/2018|Curitiba|5300|NaN|15900|
|426|5489|HL7348|SmartWatch|5|Gabriel|Assis|12/28/2018|Curitiba|1400|NaN|7000|
|427|5491|HL8851|Notebook|4|Bernardo|Botelho|7/23/2018|Curitiba|3500|NaN|14000|
|428|5533|HL8851|Notebook|2|Felipe|Paulo|2/22/2018|Curitiba|3500|NaN|7000|
|429|5576|HL1918|iPhone|4|Ana|Felippe|9/21/2018|Curitiba|5300|NaN|21200|
|430|5590|HL1918|iPhone|2|Diego|Marchesi|3/24/2018|Curitiba|5300|NaN|10600|
|431|5626|HL4379|Televisão|2|Clara|Silveira|9/9/2018|Curitiba|2500|NaN|5000|
|432|5638|HL4379|Televisão|1|Lucas|Chagas|2/14/2018|Curitiba|2500|NaN|2500|
|433|5658|HL1918|iPhone|1|Jéssica|Stefanelli|2/7/2018|Curitiba|5300|NaN|5300|
|434|5690|HL9962|Android|5|Daniel|Terra|1/27/2018|Curitiba|3400|NaN|17000|
|435|5723|HL1918|iPhone|3|Livia|Cozendey|5/13/2018|Curitiba|5300|NaN|15900|
|436|5734|HL1148|Câmera|4|José|Marques|10/6/2018|Curitiba|2100|NaN|8400|
|437|5747|HL1918|iPhone|4|Jônatas|Castro|12/17/2018|Curitiba|5300|NaN|21200|
|438|5758|HL7348|SmartWatch|3|Gabriel|Rubim|2/15/2018|Curitiba|1400|NaN|4200|
|439|5780|HL1918|iPhone|2|Cícero|Ramos|7/24/2018|Curitiba|5300|NaN|10600|
|440|5783|HL1918|iPhone|5|Rubens|Valente|3/10/2018|Curitiba|5300|NaN|26500|
|441|5785|HL7348|SmartWatch|1|Gustavo|Aragão|4/5/2018|Curitiba|1400|NaN|1400|
|442|5786|HL2714|Tablet|4|Lucas|Rocha|2/10/2018|Curitiba|1600|NaN|6400|
|443|5795|HL4379|Televisão|5|Luiz|Almeida|3/23/2018|Curitiba|2500|NaN|12500|
|444|5850|HL4379|Televisão|3|Rachel|Restum|2/9/2018|Curitiba|2500|NaN|7500|
|445|5921|HL1918|iPhone|2|Luiza|Johnson|4/23/2018|Curitiba|5300|NaN|10600|
|446|5939|HL1918|iPhone|2|Gabrielle|Wanderley|7/3/2018|Curitiba|5300|NaN|10600|
|447|5940|HL1918|iPhone|3|Milena|Alcoforado|5/27/2018|Curitiba|5300|NaN|15900|
|448|5950|HL9962|Android|1|Victor|Soares|12/19/2018|Curitiba|3400|NaN|3400|
|449|5951|HL1918|iPhone|5|Caroline|Pinto|9/17/2018|Curitiba|5300|NaN|26500|
|450|5956|HL4379|Televisão|4|Silvio|Provenzano|3/4/2018|Curitiba|2500|NaN|10000|
|451|5960|HL1148|Câmera|3|João|Junior|4/10/2018|Curitiba|2100|NaN|6300|
|452|5962|HL8851|Notebook|1|Carolina|Alfradique|1/6/2018|Curitiba|3500|NaN|3500|
|453|5967|HL1148|Câmera|5|Bruno|Barcessat|9/28/2018|Curitiba|2100|NaN|10500|
|454|5980|HL1148|Câmera|2|Tadeu|Nakayama|10/28/2018|Curitiba|2100|NaN|4200|
|455|6008|HL8851|Notebook|2|Fernanda|Junior|11/5/2018|Curitiba|3500|NaN|7000|
|456|6018|HL4379|Televisão|4|Eduardo|Soares|5/7/2018|Curitiba|2500|NaN|10000|
|457|6022|HL4379|Televisão|5|Joyce|Medina|8/9/2018|Curitiba|2500|NaN|12500|
|458|6027|HL1918|iPhone|3|Adriana|Carneiro|6/7/2018|Curitiba|5300|NaN|15900|
|459|6051|HL1918|iPhone|1|Raphael|Coelho|7/12/2018|Curitiba|5300|NaN|5300|
|460|6052|HL1918|iPhone|4|Wendela|Mariz|11/22/2018|Curitiba|5300|NaN|21200|
|461|6063|HL8851|Notebook|3|Mônica|Rotolo|2/23/2018|Curitiba|3500|NaN|10500|
|462|6074|HL9962|Android|1|Daniela|Rosa|6/3/2018|Curitiba|3400|NaN|3400|
|463|6083|HL1918|iPhone|1|Daniela|Pereira|4/20/2018|Curitiba|5300|NaN|5300|
|464|6085|HL1918|iPhone|4|Lucas|Machado|7/3/2018|Curitiba|5300|NaN|21200|
|465|6093|HL1148|Câmera|3|Fernanda|Bhering|7/12/2018|Curitiba|2100|NaN|6300|
|466|6106|HL1918|iPhone|5|Maria|Gasperi|5/30/2018|Curitiba|5300|NaN|26500|
|467|6145|HL1918|iPhone|4|Carla|Zakhm|4/26/2018|Curitiba|5300|NaN|21200|
|468|6167|HL9962|Android|4|Antonio|Bernhardt|9/27/2018|Curitiba|3400|NaN|13600|
|469|6174|HL4379|Televisão|2|Ana|Felippe|4/24/2018|Curitiba|2500|NaN|5000|
|470|6237|HL8851|Notebook|4|Gabriela|Cavalcanti|6/23/2018|Curitiba|3500|NaN|14000|
|471|6252|HL4379|Televisão|5|Eric|Júnior|9/16/2018|Curitiba|2500|NaN|12500|
|472|6262|HL9962|Android|5|Maike|Pereira|7/20/2018|Curitiba|3400|NaN|17000|
|473|6272|HL8851|Notebook|2|Daniel|Alcoforado|7/29/2018|Curitiba|3500|NaN|7000|
|474|6293|HL7348|SmartWatch|5|Adriane|Chagas|7/1/2018|Curitiba|1400|NaN|7000|
|475|6300|HL8851|Notebook|3|Joyce|Souza|9/17/2018|Curitiba|3500|NaN|10500|
|476|6309|HL4379|Televisão|3|Maria|Cardoso|9/3/2018|Curitiba|2500|NaN|7500|
|477|6320|HL8851|Notebook|4|Caio|Vianna|5/21/2018|Curitiba|3500|NaN|14000|
|478|6331|HL1918|iPhone|2|Tainah|Nogueira|1/11/2018|Curitiba|5300|NaN|10600|
|479|6340|HL1918|iPhone|3|Thais|Rodrigues|9/2/2018|Curitiba|5300|NaN|15900|
|480|6348|HL4379|Televisão|5|Lucas|Neto|7/3/2018|Curitiba|2500|NaN|12500|
|481|6350|HL8851|Notebook|5|Eduardo|Ferreira|4/5/2018|Curitiba|3500|NaN|17500|
|482|6363|HL8851|Notebook|5|Wellington|Duarte|1/10/2018|Curitiba|3500|NaN|17500|
|483|6376|HL1148|Câmera|3|Maria|Mello|1/12/2018|Curitiba|2100|NaN|6300|
|484|6393|HL1148|Câmera|3|Ulisses|Filho|3/8/2018|Curitiba|2100|NaN|6300|
|485|6397|HL1918|iPhone|4|Bernard|Pedrosa|10/7/2018|Curitiba|5300|NaN|21200|
|486|6413|HL4379|Televisão|4|Pedro|Pereira|10/28/2018|Curitiba|2500|NaN|10000|
|487|6414|HL8851|Notebook|2|Raíza|Lopes|8/26/2018|Curitiba|3500|NaN|7000|
|488|6416|HL7348|SmartWatch|3|Rilson|Guedes|6/1/2018|Curitiba|1400|NaN|4200|
|489|6473|HL4379|Televisão|3|Carolina|Brum|2/26/2018|Curitiba|2500|NaN|7500|
|490|6487|HL1918|iPhone|1|Fernanda|Rubim|3/1/2018|Curitiba|5300|NaN|5300|
|491|6489|HL1918|iPhone|1|Ravena|Bhering|6/2/2018|Curitiba|5300|NaN|5300|
|492|6509|HL4379|Televisão|2|Andressa|Rotsztejn|1/7/2018|Curitiba|2500|NaN|5000|
|493|6519|HL1918|iPhone|2|Carolina|Santos|5/17/2018|Curitiba|5300|NaN|10600|
|494|6567|HL1148|Câmera|5|Bruna|Silveira|1/23/2018|Curitiba|2100|NaN|10500|
|495|6571|HL7348|SmartWatch|4|Gabriel|Garcia|5/8/2018|Curitiba|1400|NaN|5600|
|496|6577|HL8851|Notebook|3|Caroll|Johnson|12/15/2018|Curitiba|3500|NaN|10500|
|497|6579|HL1148|Câmera|4|Caroline|Pinto|4/17/2018|Curitiba|2100|NaN|8400|
|498|6586|HL1918|iPhone|2|Rafael|Rocha|1/12/2018|Curitiba|5300|NaN|10600|
|499|6589|HL8851|Notebook|1|Thiago|Costa|5/6/2018|Curitiba|3500|NaN|3500|
|500|6608|HL7348|SmartWatch|4|Audir|Franco|12/2/2018|Curitiba|1400|NaN|5600|
|501|6643|HL7348|SmartWatch|2|Mariana|Miranda|12/13/2018|Curitiba|1400|NaN|2800|
|502|6666|HL4379|Televisão|5|Vanessa|Bach|11/10/2018|Curitiba|2500|NaN|12500|
|503|6673|HL4379|Televisão|5|Thiago|Costa|7/22/2018|Curitiba|2500|NaN|12500|
|504|6682|HL4379|Televisão|1|Raul|Silveira|7/30/2018|Curitiba|2500|NaN|2500|
|505|6684|HL4379|Televisão|2|João|Monteiro|6/4/2018|Curitiba|2500|NaN|5000|
|506|6713|HL9962|Android|4|Marcelo|Pereira|11/13/2018|Curitiba|3400|NaN|13600|
|507|6726|HL7348|SmartWatch|5|Juliana|Goes|5/30/2018|Curitiba|1400|NaN|7000|
|508|6741|HL7348|SmartWatch|5|Lucas|Freire|4/23/2018|Curitiba|1400|NaN|7000|
|509|6755|HL1918|iPhone|4|Myllena|Corrêa|5/17/2018|Curitiba|5300|NaN|21200|
|510|6774|HL1918|iPhone|2|Joyce|Medina|10/22/2018|Curitiba|5300|NaN|10600|
|511|6780|HL4379|Televisão|1|Carlos|Portela|4/28/2018|Curitiba|2500|NaN|2500|
|512|6800|HL4379|Televisão|4|Lorena|Carvalho|1/29/2018|Curitiba|2500|NaN|10000|
|513|6803|HL9962|Android|4|Guilherme|Vianna|12/5/2018|Curitiba|3400|NaN|13600|
|514|6821|HL8851|Notebook|5|Lázaro|Villanova|6/12/2018|Curitiba|3500|NaN|17500|
|515|6824|HL9962|Android|5|Andre|Sampaio|11/17/2018|Curitiba|3400|NaN|17000|
|516|6838|HL9962|Android|4|Luiza|Johnson|4/17/2018|Curitiba|3400|NaN|13600|
|517|6858|HL9962|Android|5|David|Vasconcelos|10/11/2018|Curitiba|3400|NaN|17000|
|518|6865|HL1148|Câmera|1|Beatriz|Biase|5/11/2018|Curitiba|2100|NaN|2100|
|519|6884|HL4379|Televisão|4|Giuseppe|Bhering|10/30/2018|Curitiba|2500|NaN|10000|
|520|6886|HL1918|iPhone|2|Priscila|Carvalho|2/6/2018|Curitiba|5300|NaN|10600|
|521|6890|HL4379|Televisão|3|Diego|Rodrigues|2/15/2018|Curitiba|2500|NaN|7500|
|522|6900|HL9962|Android|5|Livia|Corrêa|10/17/2018|Curitiba|3400|NaN|17000|
|523|6937|HL7348|SmartWatch|4|Rodrigo|Mendes|12/12/2018|Curitiba|1400|NaN|5600|
|524|6944|HL7348|SmartWatch|1|Raíza|Lopes|3/11/2018|Curitiba|1400|NaN|1400|
|525|6954|HL4379|Televisão|3|Luiza|Farias|10/14/2018|Curitiba|2500|NaN|7500|
|526|7000|HL7348|SmartWatch|4|João|Peçanha|8/5/2018|Curitiba|1400|NaN|5600|
|527|7001|HL8851|Notebook|1|Carlos|Araujo|9/12/2018|Curitiba|3500|NaN|3500|
|528|7007|HL1918|iPhone|3|Lívia|Marques|2/15/2018|Curitiba|5300|NaN|15900|
|529|7015|HL4379|Televisão|2|Matheus|Santos|11/21/2018|Curitiba|2500|NaN|5000|
|530|7019|HL4379|Televisão|1|Luiza|Ribeiro|8/24/2018|Curitiba|2500|NaN|2500|
|531|7042|HL1148|Câmera|2|Douglas|Rodrigues|2/15/2018|Curitiba|2100|NaN|4200|
|532|7043|HL4379|Televisão|1|Stela|Mendonça|9/5/2018|Curitiba|2500|NaN|2500|
|533|7052|HL1918|iPhone|2|Nathalia|Ventura|11/26/2018|Curitiba|5300|NaN|10600|
|534|7062|HL1918|iPhone|5|Priscila|Suzano|9/6/2018|Curitiba|5300|NaN|26500|
|535|7064|HL9962|Android|5|Hércules|Júnior|3/24/2018|Curitiba|3400|NaN|17000|
|536|7089|HL1918|iPhone|2|Michelle|Miura|10/9/2018|Curitiba|5300|NaN|10600|
|537|7095|HL4379|Televisão|1|Marina|Miranda|10/18/2018|Curitiba|2500|NaN|2500|
|538|7098|HL1148|Câmera|2|Nathalia|Ventura|7/19/2018|Curitiba|2100|NaN|4200|
|539|7137|HL9962|Android|4|Cícero|Lima|7/14/2018|Curitiba|3400|NaN|13600|
|540|7139|HL7348|SmartWatch|1|Antônio|Oliveira|9/10/2018|Curitiba|1400|NaN|1400|
|541|7149|HL4379|Televisão|5|Amanda|Procaci|5/22/2018|Curitiba|2500|NaN|12500|
|542|7150|HL7348|SmartWatch|4|Raphael|Filho|2/22/2018|Curitiba|1400|NaN|5600|
|543|7151|HL1148|Câmera|4|Luiza|Farias|5/5/2018|Curitiba|2100|NaN|8400|
|544|7153|HL1918|iPhone|3|Luã|Sá|1/21/2018|Curitiba|5300|NaN|15900|
|545|7158|HL4379|Televisão|1|Miguel|Carneiro|8/9/2018|Curitiba|2500|NaN|2500|
|546|7192|HL1918|iPhone|2|Thales|Portillo|2/2/2018|Curitiba|5300|NaN|10600|
|547|7218|HL1918|iPhone|1|Paula|Carneiro|9/3/2018|Curitiba|5300|NaN|5300|
|548|7230|HL7348|SmartWatch|3|Bruna|Silveira|10/6/2018|Curitiba|1400|NaN|4200|
|549|7235|HL4379|Televisão|2|Bárbara|Cavalcante|12/1/2018|Curitiba|2500|NaN|5000|
|550|7237|HL8851|Notebook|5|Alon|Fahrnholz|11/24/2018|Curitiba|3500|NaN|17500|
|551|7261|HL1918|iPhone|1|Lucas|Lacerda|6/27/2018|Curitiba|5300|NaN|5300|
|552|7271|HL4379|Televisão|5|Andressa|Chou|2/19/2018|Curitiba|2500|NaN|12500|
|553|7305|HL1918|iPhone|1|Jessica|Cordovil|9/20/2018|Curitiba|5300|NaN|5300|
|554|7306|HL4379|Televisão|2|Rebeca|Taylor|4/25/2018|Curitiba|2500|NaN|5000|
|555|7316|HL1148|Câmera|1|Myllena|Carneiro|10/25/2018|Curitiba|2100|NaN|2100|
|556|7326|HL1918|iPhone|3|Vitor|Campos|9/14/2018|Curitiba|5300|NaN|15900|
|557|7359|HL1148|Câmera|4|Maurício|Dias|8/27/2018|Curitiba|2100|NaN|8400|
|558|7368|HL1918|iPhone|4|Bruna|Soares|2/16/2018|Curitiba|5300|NaN|21200|
|559|7419|HL1148|Câmera|4|Katharina|Barros|5/12/2018|Curitiba|2100|NaN|8400|
|560|7425|HL4379|Televisão|1|Raísa|Rodrigues|12/30/2018|Curitiba|2500|NaN|2500|
|561|7432|HL1918|iPhone|4|Myllena|Carneiro|8/11/2018|Curitiba|5300|NaN|21200|
|562|7446|HL4379|Televisão|2|Manuela|Ferreira|9/16/2018|Curitiba|2500|NaN|5000|
|563|7447|HL4379|Televisão|1|Arthur|Portela|12/29/2018|Curitiba|2500|NaN|2500|
|564|7478|HL1918|iPhone|5|Thiago|Veiga|8/27/2018|Curitiba|5300|NaN|26500|
|565|7496|HL8851|Notebook|5|Clara|Bruno|8/29/2018|Curitiba|3500|NaN|17500|
|566|7499|HL4379|Televisão|1|Anna|Maia|10/12/2018|Curitiba|2500|NaN|2500|
|567|7501|HL9962|Android|5|Marina|Gama|8/3/2018|Curitiba|3400|NaN|17000|
|568|7508|HL1918|iPhone|1|Caroll|Johnson|10/13/2018|Curitiba|5300|NaN|5300|
|569|7514|HL1148|Câmera|2|Bruna|Ramos|3/27/2018|Curitiba|2100|NaN|4200|
|570|7543|HL1918|iPhone|1|Antônio|Soares|6/12/2018|Curitiba|5300|NaN|5300|
|571|7554|HL1918|iPhone|4|Juliana|Huon|12/27/2018|Curitiba|5300|NaN|21200|
|572|7558|HL1918|iPhone|4|Victor|Ferreira|6/19/2018|Curitiba|5300|NaN|21200|
|573|7560|HL1148|Câmera|2|Eduardo|Ferreira|10/23/2018|Curitiba|2100|NaN|4200|
|574|7581|HL9962|Android|5|Lucas|Assunção|4/4/2018|Curitiba|3400|NaN|17000|
|575|7592|HL8851|Notebook|3|Luiza|Cabral|7/15/2018|Curitiba|3500|NaN|10500|
|576|7599|HL7348|SmartWatch|2|Giovana|Vilela|12/15/2018|Curitiba|1400|NaN|2800|
|577|7625|HL4379|Televisão|4|Leandro|Ferreira|4/24/2018|Curitiba|2500|NaN|10000|
|578|7627|HL1918|iPhone|1|Breno|Quinto|2/9/2018|Curitiba|5300|NaN|5300|
|579|7636|HL9962|Android|1|Natalia|Guedes|2/11/2018|Curitiba|3400|NaN|3400|
|580|7656|HL1148|Câmera|3|Jonatas|Essaber|11/3/2018|Curitiba|2100|NaN|6300|
|581|7681|HL1918|iPhone|5|Beatriz|Nogueira|1/24/2018|Curitiba|5300|NaN|26500|
|582|7699|HL8851|Notebook|4|Juliana|Guimarães|1/7/2018|Curitiba|3500|NaN|14000|
|583|7716|HL1918|iPhone|5|Alexandre|Dantas|12/1/2018|Curitiba|5300|NaN|26500|
|584|7735|HL1918|iPhone|1|Lorena|Carvalho|8/23/2018|Curitiba|5300|NaN|5300|
|585|7738|HL7348|SmartWatch|3|Thiago|Lima|4/1/2018|Curitiba|1400|NaN|4200|
|586|7756|HL1148|Câmera|2|Pedro|Bitencourt|7/28/2018|Curitiba|2100|NaN|4200|
|587|7764|HL1918|iPhone|2|Daniel|Alcoforado|2/15/2018|Curitiba|5300|NaN|10600|
|588|7774|HL1148|Câmera|3|Amanda|Procaci|6/14/2018|Curitiba|2100|NaN|6300|
|589|7775|HL4379|Televisão|3|Julie|Ferreira|2/1/2018|Curitiba|2500|NaN|7500|
|590|7785|HL1148|Câmera|1|Mateus|Franco|10/3/2018|Curitiba|2100|NaN|2100|
|591|7798|HL1918|iPhone|3|Lucas|Freire|12/2/2018|Curitiba|5300|NaN|15900|
|592|7851|HL1148|Câmera|3|Michelle|Miura|1/31/2018|Curitiba|2100|NaN|6300|
|593|7859|HL4379|Televisão|2|Jonas|Gomes|5/20/2018|Curitiba|2500|NaN|5000|
|594|7901|HL2714|Tablet|4|João|Peçanha|8/22/2018|Curitiba|1600|NaN|6400|
|595|7911|HL7348|SmartWatch|3|Paula|Calbucci|2/26/2018|Curitiba|1400|NaN|4200|
|596|7920|HL8851|Notebook|4|Raissa|Pinheiro|8/27/2018|Curitiba|3500|NaN|14000|
|597|7935|HL7348|SmartWatch|2|Breno|Quinto|4/22/2018|Curitiba|1400|NaN|2800|
|598|7938|HL1148|Câmera|3|João|Araujo|8/22/2018|Curitiba|2100|NaN|6300|
|599|7970|HL1148|Câmera|3|Priscila|Carvalho|1/6/2018|Curitiba|2100|NaN|6300|
|600|7975|HL4379|Televisão|1|Khaio|Mesquita|7/1/2018|Curitiba|2500|NaN|2500|
|601|7986|HL2714|Tablet|2|Ana|Monte|9/19/2018|Curitiba|1600|NaN|3200|
|602|7991|HL4379|Televisão|1|Michelle|Pereira|1/18/2018|Curitiba|2500|NaN|2500|
|603|8012|HL1918|iPhone|3|Guilherme|Marchesi|9/15/2018|Curitiba|5300|NaN|15900|
|604|8027|HL4379|Televisão|3|João|Tabet|11/16/2018|Curitiba|2500|NaN|7500|
|605|8038|HL1918|iPhone|5|Mônica|Rotolo|3/8/2018|Curitiba|5300|NaN|26500|
|606|8080|HL9962|Android|4|Fabio|Boccaletti|7/9/2018|Curitiba|3400|NaN|13600|
|607|8158|HL7348|SmartWatch|4|Juliana|Silva|12/3/2018|Curitiba|1400|NaN|5600|
|608|8180|HL7348|SmartWatch|1|Caio|Moraes|6/10/2018|Curitiba|1400|NaN|1400|
|609|8195|HL7348|SmartWatch|5|Deysiane|Medronho|11/14/2018|Curitiba|1400|NaN|7000|
|610|8214|HL7348|SmartWatch|3|Marina|Gama|1/16/2018|Curitiba|1400|NaN|4200|
|611|8245|HL4379|Televisão|5|Gabriela|Mello|6/2/2018|Curitiba|2500|NaN|12500|
|612|8262|HL4379|Televisão|5|William|Mendonça|2/7/2018|Curitiba|2500|NaN|12500|
|613|8265|HL1918|iPhone|3|Raphael|Rezende|7/23/2018|Curitiba|5300|NaN|15900|
|614|8300|HL9962|Android|1|Luis|Silva|8/17/2018|Curitiba|3400|NaN|3400|
|615|8309|HL4379|Televisão|5|Beatriz|Rocha|12/18/2018|Curitiba|2500|NaN|12500|
|616|8317|HL4379|Televisão|5|Pedro|Cardoso|11/17/2018|Curitiba|2500|NaN|12500|
|617|8332|HL9962|Android|2|Pedro|Cardoso|11/8/2018|Curitiba|3400|NaN|6800|
|618|8345|HL9962|Android|3|Bruno|Velucci|7/25/2018|Curitiba|3400|NaN|10200|
|619|8377|HL1918|iPhone|4|Thomaz|Ferreira|10/2/2018|Curitiba|5300|NaN|21200|
|620|8395|HL9962|Android|3|Beatriz|Perdomo|4/20/2018|Curitiba|3400|NaN|10200|
|621|8403|HL8851|Notebook|3|Thaís|Pereira|2/21/2018|Curitiba|3500|NaN|10500|
|622|8412|HL8851|Notebook|2|Felipe|Freitas|4/26/2018|Curitiba|3500|NaN|7000|
|623|8424|HL4379|Televisão|1|Stefan|Santos|1/17/2018|Curitiba|2500|NaN|2500|
|624|8453|HL7348|SmartWatch|4|Ana|Silva|8/4/2018|Curitiba|1400|NaN|5600|
|625|8468|HL1918|iPhone|1|Wilson|Meirelles|9/23/2018|Curitiba|5300|NaN|5300|
|626|8474|HL4379|Televisão|4|Priscila|Vogel|10/30/2018|Curitiba|2500|NaN|10000|
|627|8478|HL4379|Televisão|4|Gustavo|Aragão|11/26/2018|Curitiba|2500|NaN|10000|
|628|8484|HL2714|Tablet|5|Roberto|Nogueira|2/6/2018|Curitiba|1600|NaN|8000|
|629|8497|HL4379|Televisão|5|Thaís|Moura|5/8/2018|Curitiba|2500|NaN|12500|
|630|8498|HL2714|Tablet|3|Carolina|Vasconcelos|12/21/2018|Curitiba|1600|NaN|4800|
|631|8524|HL1918|iPhone|3|Alon|Pestana|1/22/2018|Curitiba|5300|NaN|15900|
|632|8537|HL1148|Câmera|1|João|Capitulo|9/20/2018|Curitiba|2100|NaN|2100|
|633|8580|HL4379|Televisão|3|Lucas|Lemos|10/19/2018|Curitiba|2500|NaN|7500|
|634|8600|HL1918|iPhone|2|Gabriella|Sagrillo|3/8/2018|Curitiba|5300|NaN|10600|
|635|8676|HL4379|Televisão|1|Andressa|Rotsztejn|10/13/2018|Curitiba|2500|NaN|2500|
|636|8687|HL4379|Televisão|1|João|Fonseca|8/15/2018|Curitiba|2500|NaN|2500|
|637|8715|HL7348|SmartWatch|1|Fabio|Boccaletti|10/23/2018|Curitiba|1400|NaN|1400|
|638|8718|HL4379|Televisão|1|Iuri|Neto|12/15/2018|Curitiba|2500|NaN|2500|
|639|8736|HL1918|iPhone|1|Guilherme|Lima|4/20/2018|Curitiba|5300|NaN|5300|
|640|8761|HL4379|Televisão|1|Lázaro|Villanova|5/24/2018|Curitiba|2500|NaN|2500|
|641|8773|HL9962|Android|2|Gabriela|Fernandes|11/30/2018|Curitiba|3400|NaN|6800|
|642|8800|HL2714|Tablet|1|Giovana|Vilela|6/2/2018|Curitiba|1600|NaN|1600|
|643|8801|HL1918|iPhone|5|Mateus|Polastri|12/27/2018|Curitiba|5300|NaN|26500|
|644|8817|HL4379|Televisão|1|Maria|Motta|8/30/2018|Curitiba|2500|NaN|2500|
|645|8819|HL8851|Notebook|1|Raísa|Rodrigues|7/7/2018|Curitiba|3500|NaN|3500|
|646|8824|HL1148|Câmera|5|Felipe|Júnior|8/16/2018|Curitiba|2100|NaN|10500|
|647|8848|HL9962|Android|5|Matheus|Gomes|7/30/2018|Curitiba|3400|NaN|17000|
|648|8859|HL1918|iPhone|2|Ian|Almeida|12/14/2018|Curitiba|5300|NaN|10600|
|649|8868|HL8851|Notebook|3|Marcelo|Pereira|6/21/2018|Curitiba|3500|NaN|10500|
|650|8887|HL8851|Notebook|3|Michelle|Pereira|2/15/2018|Curitiba|3500|NaN|10500|
|651|8892|HL2714|Tablet|4|Wen|Santos|1/24/2018|Curitiba|1600|NaN|6400|
|652|8905|HL9962|Android|2|Jorge|Carvalho|5/31/2018|Curitiba|3400|NaN|6800|
|653|8921|HL2714|Tablet|3|Mariana|Miranda|1/25/2018|Curitiba|1600|NaN|4800|
|654|8922|HL2714|Tablet|1|Maike|Pereira|2/18/2018|Curitiba|1600|NaN|1600|
|655|8926|HL1148|Câmera|3|Gabriella|Lopes|11/14/2018|Curitiba|2100|NaN|6300|
|656|8949|HL4379|Televisão|2|Victor|Magalhães|2/16/2018|Curitiba|2500|NaN|5000|
|657|8956|HL1918|iPhone|4|Júlio|Freire|8/18/2018|Curitiba|5300|NaN|21200|
|658|8972|HL4379|Televisão|5|Andressa|Chou|3/1/2018|Curitiba|2500|NaN|12500|
|659|8998|HL7348|SmartWatch|5|Thaís|Pereira|12/2/2018|Curitiba|1400|NaN|7000|
|660|9006|HL1148|Câmera|1|Lucas|Neto|2/4/2018|Curitiba|2100|NaN|2100|
|661|9012|HL8851|Notebook|1|Cézar|Santos|12/13/2018|Curitiba|3500|NaN|3500|
|662|9026|HL1148|Câmera|3|Marcela|Gasperi|2/3/2018|Curitiba|2100|NaN|6300|
|663|9028|HL1148|Câmera|3|Marcos|Nucci|11/7/2018|Curitiba|2100|NaN|6300|
|664|9047|HL7348|SmartWatch|4|Ives|Barbosa|9/17/2018|Curitiba|1400|NaN|5600|
|665|9051|HL8851|Notebook|1|Giulia|Pessanha|8/24/2018|Curitiba|3500|NaN|3500|
|666|9098|HL1918|iPhone|5|Diego|Barros|8/10/2018|Curitiba|5300|NaN|26500|
|667|9119|HL2714|Tablet|1|Giovanna|Santos|12/20/2018|Curitiba|1600|NaN|1600|
|668|9120|HL7348|SmartWatch|4|Clarissa|Santos|1/7/2018|Curitiba|1400|NaN|5600|
|669|9123|HL4379|Televisão|4|Jorge|Carvalho|4/17/2018|Curitiba|2500|NaN|10000|
|670|9160|HL8851|Notebook|5|Rafaela|Ferreira|7/6/2018|Curitiba|3500|NaN|17500|
|671|9174|HL1918|iPhone|3|Júlia|Almeida|2/20/2018|Curitiba|5300|NaN|15900|
|672|9183|HL7348|SmartWatch|3|Luiza|Cabral|2/11/2018|Curitiba|1400|NaN|4200|
|673|9203|HL9962|Android|4|Rafael|Guimarães|7/23/2018|Curitiba|3400|NaN|13600|
|674|9215|HL4379|Televisão|5|Victor|Lira|8/15/2018|Curitiba|2500|NaN|12500|
|675|9238|HL4379|Televisão|5|Eduardo|Ferreira|3/6/2018|Curitiba|2500|NaN|12500|
|676|9261|HL1918|iPhone|4|Sylvio|Bernhardt|9/16/2018|Curitiba|5300|NaN|21200|
|677|9328|HL9962|Android|1|Sandy|Figueiredo|12/3/2018|Curitiba|3400|NaN|3400|
|678|9332|HL1918|iPhone|4|Ives|Teixeira|3/7/2018|Curitiba|5300|NaN|21200|
|679|9374|HL2714|Tablet|2|Julia|Leite|3/4/2018|Curitiba|1600|NaN|3200|
|680|9375|HL1148|Câmera|1|Silvio|Provenzano|4/15/2018|Curitiba|2100|NaN|2100|
|681|9384|HL8851|Notebook|1|Isabelle|Firmino|11/17/2018|Curitiba|3500|NaN|3500|
|682|9401|HL7348|SmartWatch|3|Leandro|Melo|1/31/2018|Curitiba|1400|NaN|4200|
|683|9411|HL4379|Televisão|2|Maria|Cardoso|12/12/2018|Curitiba|2500|NaN|5000|
|684|9427|HL1148|Câmera|4|Fernanda|Silva|1/13/2018|Curitiba|2100|NaN|8400|
|685|9458|HL8851|Notebook|2|Lenon|Fernandes|9/1/2018|Curitiba|3500|NaN|7000|
|686|9510|HL7348|SmartWatch|1|Izabel|Lopes|8/2/2018|Curitiba|1400|NaN|1400|
|687|9545|HL1148|Câmera|4|Felipe|Paulo|3/2/2018|Curitiba|2100|NaN|8400|
|688|9547|HL1918|iPhone|3|Carlos|Portela|7/19/2018|Curitiba|5300|NaN|15900|
|689|9556|HL8851|Notebook|3|Guilherme|Castilho|7/11/2018|Curitiba|3500|NaN|10500|
|690|9584|HL9962|Android|4|Samara|Pinto|2/19/2018|Curitiba|3400|NaN|13600|
|691|9594|HL4379|Televisão|4|Monique|Vasconcelos|10/8/2018|Curitiba|2500|NaN|10000|
|692|9611|HL1918|iPhone|2|Igor|Lima|4/10/2018|Curitiba|5300|NaN|10600|
|693|9614|HL1148|Câmera|3|Nicolas|Monteiro|3/31/2018|Curitiba|2100|NaN|6300|
|694|9644|HL1918|iPhone|5|Ulisses|Filho|9/14/2018|Curitiba|5300|NaN|26500|
|695|9657|HL1918|iPhone|1|Debora|Silva|5/9/2018|Curitiba|5300|NaN|5300|
|696|9658|HL1148|Câmera|1|Bruna|Gomes|7/9/2018|Curitiba|2100|NaN|2100|
|697|9688|HL2714|Tablet|2|Bruno|Ursulino|1/30/2018|Curitiba|1600|NaN|3200|
|698|9690|HL8851|Notebook|1|Renan|Freire|1/19/2018|Curitiba|3500|NaN|3500|
|699|9703|HL4379|Televisão|4|Mariane|Ferreira|8/23/2018|Curitiba|2500|NaN|10000|
|700|9716|HL2714|Tablet|5|Paula|Calbucci|7/19/2018|Curitiba|1600|NaN|8000|
|701|9717|HL1148|Câmera|2|Hygor|Essaber|3/28/2018|Curitiba|2100|NaN|4200|
|702|9741|HL4379|Televisão|1|Ravena|Bhering|6/10/2018|Curitiba|2500|NaN|2500|
|703|9749|HL9962|Android|3|Juliana|Mesquita|3/8/2018|Curitiba|3400|NaN|10200|
|704|9759|HL1918|iPhone|2|Nathan|Morelli|9/2/2018|Curitiba|5300|NaN|10600|
|705|9775|HL1918|iPhone|2|Rogério|Pereira|8/8/2018|Curitiba|5300|NaN|10600|
|706|9787|HL8851|Notebook|1|Luis|Villanova|1/14/2018|Curitiba|3500|NaN|3500|
|707|9808|HL8851|Notebook|4|Luiz|Conceição|6/13/2018|Curitiba|3500|NaN|14000|
|708|9823|HL1918|iPhone|2|Natalia|Andrade|8/11/2018|Curitiba|5300|NaN|10600|
|709|9835|HL1918|iPhone|2|Guilherme|Merotto|12/24/2018|Curitiba|5300|NaN|10600|
|710|9836|HL2714|Tablet|2|Wendela|Veloso|6/21/2018|Curitiba|1600|NaN|3200|
|711|9844|HL7348|SmartWatch|3|Ana|Bôas|1/21/2018|Curitiba|1400|NaN|4200|
|712|9849|HL9962|Android|2|Caio|Moura|11/26/2018|Curitiba|3400|NaN|6800|
|713|9851|HL9962|Android|2|Fernanda|Silva|3/31/2018|Curitiba|3400|NaN|6800|
|714|9859|HL2714|Tablet|1|Júlio|Fraga|12/25/2018|Curitiba|1600|NaN|1600|
|715|9876|HL4379|Televisão|5|Bruno|Mota|4/30/2018|Curitiba|2500|NaN|12500|
|716|9918|HL1148|Câmera|2|Lucas|Reis|12/27/2018|Curitiba|2100|NaN|4200|
|717|9944|HL1918|iPhone|5|Raphael|Kurtz|7/16/2018|Curitiba|5300|NaN|26500|
|718|9998|HL7348|SmartWatch|1|Vinícius|Antunes|12/10/2018|Curitiba|1400|NaN|1400|
|0|1|HL4379|Televisão|3|Renan|Nascimento|9/14/2018|Recife|2500|NaN|7500|
|1|24|HL2714|Tablet|5|Carla|Zakhm|11/13/2018|Recife|1600|NaN|8000|
|2|26|HL1918|iPhone|4|Bianca|Tatsch|10/10/2018|Recife|5300|NaN|21200|
|3|35|HL1918|iPhone|3|Guido|Monteiro|4/18/2018|Recife|5300|NaN|15900|
|4|44|HL4379|Televisão|1|Eduardo|Quindeler|7/20/2018|Recife|2500|NaN|2500|
|5|46|HL8851|Notebook|2|Larissa|Cruz|9/15/2018|Recife|3500|NaN|7000|
|6|58|HL9962|Android|1|Alexandre|Dantas|1/28/2018|Recife|3400|NaN|3400|
|7|60|HL1148|Câmera|1|Marina|Mesquita|8/25/2018|Recife|2100|NaN|2100|
|8|78|HL4379|Televisão|2|Lucas|Junior|8/3/2018|Recife|2500|NaN|5000|
|9|90|HL4379|Televisão|4|Luíza|Goulart|7/25/2018|Recife|2500|NaN|10000|
|10|98|HL1148|Câmera|3|Carla|Zakhm|6/7/2018|Recife|2100|NaN|6300|
|11|112|HL8851|Notebook|4|Allan|Candido|4/5/2018|Recife|3500|NaN|14000|
|12|127|HL7348|SmartWatch|5|Bárbara|Lima|5/6/2018|Recife|1400|NaN|7000|
|13|144|HL1148|Câmera|3|Juan|Fernandes|3/28/2018|Recife|2100|NaN|6300|
|14|149|HL2714|Tablet|2|Gabrielle|Porto|4/23/2018|Recife|1600|NaN|3200|
|15|209|HL1918|iPhone|2|Eduardo|Silva|3/31/2018|Recife|5300|NaN|10600|
|16|229|HL1918|iPhone|3|Raphael|Ferman|4/22/2018|Recife|5300|NaN|15900|
|17|260|HL4379|Televisão|4|Rilson|Guedes|9/27/2018|Recife|2500|NaN|10000|
|18|278|HL1918|iPhone|3|Paola|Abreu|12/9/2018|Recife|5300|NaN|15900|
|19|285|HL1918|iPhone|3|João|Peçanha|9/15/2018|Recife|5300|NaN|15900|
|20|290|HL9962|Android|3|Victor|Ferreira|3/18/2018|Recife|3400|NaN|10200|
|21|291|HL7348|SmartWatch|5|Patrick|Silva|10/28/2018|Recife|1400|NaN|7000|
|22|294|HL1918|iPhone|5|Bernard|Pedrosa|6/10/2018|Recife|5300|NaN|26500|
|23|321|HL2714|Tablet|1|Catarina|Teixeira|3/9/2018|Recife|1600|NaN|1600|
|24|333|HL1918|iPhone|3|Izabel|Miura|11/7/2018|Recife|5300|NaN|15900|
|25|337|HL2714|Tablet|3|João|Menezes|9/26/2018|Recife|1600|NaN|4800|
|26|369|HL8851|Notebook|1|Anderson|Martins|6/6/2018|Recife|3500|NaN|3500|
|27|386|HL2714|Tablet|1|Rebeca|Taylor|5/9/2018|Recife|1600|NaN|1600|
|28|424|HL1918|iPhone|1|Raissa|Maia|8/19/2018|Recife|5300|NaN|5300|
|29|443|HL4379|Televisão|4|Eduardo|Veiga|6/3/2018|Recife|2500|NaN|10000|
|30|473|HL4379|Televisão|1|Priscila|Carvalho|2/5/2018|Recife|2500|NaN|2500|
|31|483|HL2714|Tablet|3|Lucas|Valim|5/2/2018|Recife|1600|NaN|4800|
|32|485|HL1918|iPhone|2|Juliana|Silva|6/26/2018|Recife|5300|NaN|10600|
|33|507|HL4379|Televisão|2|Ana|Soledade|3/18/2018|Recife|2500|NaN|5000|
|34|508|HL1918|iPhone|5|Letícia|Leal|4/7/2018|Recife|5300|NaN|26500|
|35|529|HL1918|iPhone|1|Kim|Ferreira|10/8/2018|Recife|5300|NaN|5300|
|36|596|HL1148|Câmera|3|Paula|Carneiro|5/22/2018|Recife|2100|NaN|6300|
|37|613|HL9962|Android|1|Carolina|Motta|10/18/2018|Recife|3400|NaN|3400|
|38|617|HL2714|Tablet|4|Rachel|Silva|12/8/2018|Recife|1600|NaN|6400|
|39|619|HL7348|SmartWatch|5|Gabriel|Thome|2/5/2018|Recife|1400|NaN|7000|
|40|623|HL8851|Notebook|5|Pedro|Santos|1/27/2018|Recife|3500|NaN|17500|
|41|647|HL1148|Câmera|1|Amanda|Braga|3/19/2018|Recife|2100|NaN|2100|
|42|667|HL9962|Android|1|Ana|Almeida|1/5/2018|Recife|3400|NaN|3400|
|43|669|HL1918|iPhone|2|Bianca|Tatsch|12/22/2018|Recife|5300|NaN|10600|
|44|671|HL4379|Televisão|4|Aline|Mello|10/4/2018|Recife|2500|NaN|10000|
|45|674|HL1918|iPhone|4|Pedro|Jorge|6/20/2018|Recife|5300|NaN|21200|
|46|676|HL9962|Android|3|Henrique|Lencastre|5/5/2018|Recife|3400|NaN|10200|
|47|687|HL4379|Televisão|1|Victor|Gomes|5/24/2018|Recife|2500|NaN|2500|
|48|694|HL9962|Android|5|Luiza|Ribeiro|7/28/2018|Recife|3400|NaN|17000|
|49|709|HL1918|iPhone|2|Débora|Lopes|10/3/2018|Recife|5300|NaN|10600|
|50|722|HL1918|iPhone|3|Bernardo|Botelho|8/24/2018|Recife|5300|NaN|15900|
|51|746|HL4379|Televisão|5|Vanessa|Bach|5/29/2018|Recife|2500|NaN|12500|
|52|749|HL8851|Notebook|5|Hércules|Júnior|7/12/2018|Recife|3500|NaN|17500|
|53|769|HL1918|iPhone|3|Rogério|Pereira|1/23/2018|Recife|5300|NaN|15900|
|54|804|HL1918|iPhone|2|Khaio|Mesquita|11/30/2018|Recife|5300|NaN|10600|
|55|811|HL1918|iPhone|3|Raíssa|Nimer|1/31/2018|Recife|5300|NaN|15900|
|56|816|HL4379|Televisão|1|Lucas|Assunção|11/1/2018|Recife|2500|NaN|2500|
|57|819|HL7348|SmartWatch|3|Thales|Portillo|6/24/2018|Recife|1400|NaN|4200|
|58|842|HL8851|Notebook|4|Mariana|Baptista|6/6/2018|Recife|3500|NaN|14000|
|59|857|HL9962|Android|4|Luiz|Almeida|4/3/2018|Recife|3400|NaN|13600|
|60|877|HL1918|iPhone|1|Maria|Cardoso|10/16/2018|Recife|5300|NaN|5300|
|61|909|HL9962|Android|1|Daniel|Nauenberg|4/20/2018|Recife|3400|NaN|3400|
|62|914|HL4379|Televisão|2|Luiz|Freire|9/15/2018|Recife|2500|NaN|5000|
|63|931|HL4379|Televisão|2|Pedro|Buraco|4/22/2018|Recife|2500|NaN|5000|
|64|932|HL1918|iPhone|2|Thomaz|Ferreira|3/12/2018|Recife|5300|NaN|10600|
|65|950|HL1918|iPhone|4|Lucas|Freire|5/27/2018|Recife|5300|NaN|21200|
|66|954|HL1918|iPhone|5|Caroline|Pinto|1/28/2018|Recife|5300|NaN|26500|
|67|962|HL1918|iPhone|4|Daniel|Cardoso|11/1/2018|Recife|5300|NaN|21200|
|68|967|HL1918|iPhone|5|Raíssa|Oliveira|6/9/2018|Recife|5300|NaN|26500|
|69|971|HL7348|SmartWatch|5|Livia|Cozendey|10/9/2018|Recife|1400|NaN|7000|
|70|974|HL1918|iPhone|3|Matheus|Sapir|1/8/2018|Recife|5300|NaN|15900|
|71|978|HL1918|iPhone|5|Samara|Pinto|8/14/2018|Recife|5300|NaN|26500|
|72|980|HL1148|Câmera|5|Ana|Almeida|8/13/2018|Recife|2100|NaN|10500|
|73|985|HL7348|SmartWatch|4|Chan|Santos|8/23/2018|Recife|1400|NaN|5600|
|74|1012|HL7348|SmartWatch|2|Yasmim|Verly|10/9/2018|Recife|1400|NaN|2800|
|75|1027|HL8851|Notebook|2|Helvio|Pedrosa|7/20/2018|Recife|3500|NaN|7000|
|76|1032|HL2714|Tablet|5|Dykson|Silva|11/25/2018|Recife|1600|NaN|8000|
|77|1039|HL1918|iPhone|1|Mateus|Maia|4/18/2018|Recife|5300|NaN|5300|
|78|1049|HL4379|Televisão|4|Carlos|Araujo|10/8/2018|Recife|2500|NaN|10000|
|79|1073|HL1918|iPhone|1|Andressa|Nóbrega|2/22/2018|Recife|5300|NaN|5300|
|80|1099|HL9962|Android|2|Antonio|Bernhardt|11/10/2018|Recife|3400|NaN|6800|
|81|1110|HL1918|iPhone|5|Marina|Perdomo|3/9/2018|Recife|5300|NaN|26500|
|82|1112|HL4379|Televisão|4|Fernanda|Bhering|11/19/2018|Recife|2500|NaN|10000|
|83|1130|HL4379|Televisão|5|Bruno|Silva|2/18/2018|Recife|2500|NaN|12500|
|84|1135|HL1918|iPhone|2|Carolina|Motta|7/28/2018|Recife|5300|NaN|10600|
|85|1137|HL4379|Televisão|4|Julia|Aliani|7/31/2018|Recife|2500|NaN|10000|
|86|1144|HL9962|Android|5|Beatriz|Perdomo|4/4/2018|Recife|3400|NaN|17000|
|87|1155|HL1148|Câmera|2|Marcela|Medeiros|10/30/2018|Recife|2100|NaN|4200|
|88|1156|HL9962|Android|2|Eduardo|Vargas|9/25/2018|Recife|3400|NaN|6800|
|89|1172|HL4379|Televisão|1|Eduardo|Vargas|8/24/2018|Recife|2500|NaN|2500|
|90|1188|HL7348|SmartWatch|3|Ana|Campos|4/12/2018|Recife|1400|NaN|4200|
|91|1190|HL9962|Android|1|Gabriel|Silva|7/15/2018|Recife|3400|NaN|3400|
|92|1201|HL2714|Tablet|4|Gabriel|Rocha|1/13/2018|Recife|1600|NaN|6400|
|93|1225|HL4379|Televisão|3|Jéssica|Stefanelli|5/22/2018|Recife|2500|NaN|7500|
|94|1237|HL1918|iPhone|4|Wellington|Duarte|12/20/2018|Recife|5300|NaN|21200|
|95|1239|HL1918|iPhone|5|Brenno|Santos|8/30/2018|Recife|5300|NaN|26500|
|96|1243|HL4379|Televisão|1|Stefan|Santos|9/15/2018|Recife|2500|NaN|2500|
|97|1312|HL2714|Tablet|5|Marina|Mesquita|11/21/2018|Recife|1600|NaN|8000|
|98|1316|HL4379|Televisão|3|Bruna|Franco|10/22/2018|Recife|2500|NaN|7500|
|99|1320|HL1148|Câmera|4|Luiza|Farias|12/31/2018|Recife|2100|NaN|8400|
|100|1322|HL7348|SmartWatch|4|Roberta|Nogueira|8/17/2018|Recife|1400|NaN|5600|
|101|1323|HL1918|iPhone|1|Diego|Barros|11/26/2018|Recife|5300|NaN|5300|
|102|1324|HL1918|iPhone|5|Joao|Pereira|10/1/2018|Recife|5300|NaN|26500|
|103|1414|HL1918|iPhone|5|Amanda|Delgado|5/25/2018|Recife|5300|NaN|26500|
|104|1425|HL1918|iPhone|1|Eric|Carvalho|10/25/2018|Recife|5300|NaN|5300|
|105|1453|HL1918|iPhone|1|Stefan|Nunes|2/24/2018|Recife|5300|NaN|5300|
|106|1458|HL1918|iPhone|3|Carlos|Mesquita|1/14/2018|Recife|5300|NaN|15900|
|107|1472|HL1148|Câmera|3|Raul|Junqueira|5/16/2018|Recife|2100|NaN|6300|
|108|1479|HL7348|SmartWatch|3|Vitor|Arruda|6/25/2018|Recife|1400|NaN|4200|
|109|1480|HL1918|iPhone|3|Amanda|Delgado|4/8/2018|Recife|5300|NaN|15900|
|110|1493|HL1918|iPhone|2|Sylvio|Bernhardt|5/8/2018|Recife|5300|NaN|10600|
|111|1495|HL2714|Tablet|5|Camille|Silva|5/14/2018|Recife|1600|NaN|8000|
|112|1504|HL1148|Câmera|4|Bruno|Velucci|3/29/2018|Recife|2100|NaN|8400|
|113|1505|HL1148|Câmera|2|Thaís|Ribeiro|11/6/2018|Recife|2100|NaN|4200|
|114|1525|HL7348|SmartWatch|5|Marina|Gama|2/18/2018|Recife|1400|NaN|7000|
|115|1557|HL4379|Televisão|2|Jéssica|Resinente|12/24/2018|Recife|2500|NaN|5000|
|116|1559|HL4379|Televisão|5|Luis|Oliveira|3/3/2018|Recife|2500|NaN|12500|
|117|1568|HL1918|iPhone|2|Vanessa|Bach|3/17/2018|Recife|5300|NaN|10600|
|118|1576|HL1918|iPhone|4|Lucas|Neto|4/18/2018|Recife|5300|NaN|21200|
|119|1586|HL9962|Android|4|David|Assumpção|6/13/2018|Recife|3400|NaN|13600|
|120|1588|HL1918|iPhone|3|Guilherme|Vianna|5/2/2018|Recife|5300|NaN|15900|
|121|1592|HL1148|Câmera|1|Diego|Marchesi|4/22/2018|Recife|2100|NaN|2100|
|122|1595|HL1918|iPhone|4|Isabel|Mesquita|2/20/2018|Recife|5300|NaN|21200|
|123|1596|HL1148|Câmera|5|Lázaro|Villanova|11/11/2018|Recife|2100|NaN|10500|
|124|1637|HL9962|Android|1|Caroline|Aquino|11/5/2018|Recife|3400|NaN|3400|
|125|1664|HL9962|Android|3|José|Fonseca|10/23/2018|Recife|3400|NaN|10200|
|126|1678|HL1918|iPhone|3|Daniela|Andrada|4/24/2018|Recife|5300|NaN|15900|
|127|1688|HL2714|Tablet|5|Silvio|Provenzano|7/19/2018|Recife|1600|NaN|8000|
|128|1689|HL1918|iPhone|1|Thales|Portillo|12/8/2018|Recife|5300|NaN|5300|
|129|1699|HL4379|Televisão|5|Natalia|Marinho|6/24/2018|Recife|2500|NaN|12500|
|130|1714|HL4379|Televisão|5|Marina|Marins|4/18/2018|Recife|2500|NaN|12500|
|131|1738|HL4379|Televisão|5|Andre|Sampaio|12/3/2018|Recife|2500|NaN|12500|
|132|1745|HL1918|iPhone|2|Juliana|Mesquita|7/3/2018|Recife|5300|NaN|10600|
|133|1746|HL8851|Notebook|1|Pedro|Sena|9/5/2018|Recife|3500|NaN|3500|
|134|1765|HL1918|iPhone|4|Diogo|Ressurreição|4/1/2018|Recife|5300|NaN|21200|
|135|1822|HL1148|Câmera|1|Débora|Lopes|4/19/2018|Recife|2100|NaN|2100|
|136|1827|HL9962|Android|1|Wilson|Brandão|2/13/2018|Recife|3400|NaN|3400|
|137|1900|HL4379|Televisão|2|Henrique|Oliveira|8/27/2018|Recife|2500|NaN|5000|
|138|1901|HL1918|iPhone|1|Marina|Mesquita|8/20/2018|Recife|5300|NaN|5300|
|139|1902|HL1918|iPhone|2|Pedro|Rodrigues|7/23/2018|Recife|5300|NaN|10600|
|140|1903|HL1918|iPhone|5|Giulia|Lopes|10/8/2018|Recife|5300|NaN|26500|
|141|1905|HL9962|Android|4|Paola|Abreu|7/20/2018|Recife|3400|NaN|13600|
|142|1908|HL2714|Tablet|4|Nathan|Cunha|8/12/2018|Recife|1600|NaN|6400|
|143|1946|HL1918|iPhone|2|Nathan|Morelli|12/16/2018|Recife|5300|NaN|10600|
|144|1983|HL4379|Televisão|4|Ana|Leite|10/29/2018|Recife|2500|NaN|10000|
|145|1984|HL8851|Notebook|5|Luis|Silva|9/21/2018|Recife|3500|NaN|17500|
|146|2013|HL4379|Televisão|5|Lucas|Junior|9/1/2018|Recife|2500|NaN|12500|
|147|2023|HL7348|SmartWatch|3|Victor|Soares|8/11/2018|Recife|1400|NaN|4200|
|148|2042|HL1918|iPhone|5|Clarissa|Santos|3/17/2018|Recife|5300|NaN|26500|
|149|2074|HL1918|iPhone|5|Guido|Monteiro|5/17/2018|Recife|5300|NaN|26500|
|150|2087|HL9962|Android|1|Raísa|Berto|1/9/2018|Recife|3400|NaN|3400|
|151|2091|HL4379|Televisão|3|Adrielle|Vieira|3/30/2018|Recife|2500|NaN|7500|
|152|2094|HL4379|Televisão|3|Thainá|Binello|11/14/2018|Recife|2500|NaN|7500|
|153|2103|HL1918|iPhone|1|Victor|Zakhm|8/17/2018|Recife|5300|NaN|5300|
|154|2108|HL9962|Android|1|Gabriel|Garcia|12/28/2018|Recife|3400|NaN|3400|
|155|2122|HL8851|Notebook|5|Milena|Alcoforado|4/7/2018|Recife|3500|NaN|17500|
|156|2126|HL2714|Tablet|4|Arthur|Pereira|7/26/2018|Recife|1600|NaN|6400|
|157|2151|HL8851|Notebook|4|Marcos|Nucci|1/3/2018|Recife|3500|NaN|14000|
|158|2173|HL4379|Televisão|3|Jonatas|Essaber|10/3/2018|Recife|2500|NaN|7500|
|159|2228|HL9962|Android|4|Jackson|Derossi|11/2/2018|Recife|3400|NaN|13600|
|160|2235|HL9962|Android|1|Raísa|Rodrigues|1/22/2018|Recife|3400|NaN|3400|
|161|2238|HL4379|Televisão|3|Adrielle|Vieira|5/13/2018|Recife|2500|NaN|7500|
|162|2285|HL4379|Televisão|5|Myllena|Corrêa|8/18/2018|Recife|2500|NaN|12500|
|163|2290|HL1918|iPhone|3|Gabrielle|Viríssimo|11/2/2018|Recife|5300|NaN|15900|
|164|2314|HL1918|iPhone|5|Jeferson|Sone|11/26/2018|Recife|5300|NaN|26500|
|165|2334|HL2714|Tablet|4|Pedro|Ronfini|3/24/2018|Recife|1600|NaN|6400|
|166|2341|HL1918|iPhone|5|Wilson|Miranda|5/31/2018|Recife|5300|NaN|26500|
|167|2343|HL4379|Televisão|4|Daniel|Felippe|7/8/2018|Recife|2500|NaN|10000|
|168|2358|HL8851|Notebook|2|Matheus|Miranda|5/16/2018|Recife|3500|NaN|7000|
|169|2359|HL4379|Televisão|5|Fernanda|Junior|1/5/2018|Recife|2500|NaN|12500|
|170|2369|HL9962|Android|4|Amanda|Felippe|1/19/2018|Recife|3400|NaN|13600|
|171|2406|HL7348|SmartWatch|3|Carolina|Figueiredo|3/3/2018|Recife|1400|NaN|4200|
|172|2419|HL2714|Tablet|1|Matheus|Gomes|12/16/2018|Recife|1600|NaN|1600|
|173|2441|HL8851|Notebook|2|Julia|Leig|7/20/2018|Recife|3500|NaN|7000|
|174|2453|HL9962|Android|2|Daniel|Sousa|12/3/2018|Recife|3400|NaN|6800|
|175|2465|HL1918|iPhone|3|Rafaela|Gomes|8/27/2018|Recife|5300|NaN|15900|
|176|2471|HL1918|iPhone|4|Lucas|Chagas|1/26/2018|Recife|5300|NaN|21200|
|177|2479|HL2714|Tablet|2|Felipe|Júnior|1/6/2018|Recife|1600|NaN|3200|
|178|2484|HL2714|Tablet|5|Ruan|Lopes|10/30/2018|Recife|1600|NaN|8000|
|179|2487|HL7348|SmartWatch|5|Luis|Oliveira|10/5/2018|Recife|1400|NaN|7000|
|180|2501|HL8851|Notebook|4|Lorena|Kohn|7/15/2018|Recife|3500|NaN|14000|
|181|2505|HL9962|Android|5|Tiago|Pereira|3/8/2018|Recife|3400|NaN|17000|
|182|2515|HL1918|iPhone|1|Mariana|Miranda|8/23/2018|Recife|5300|NaN|5300|
|183|2524|HL1918|iPhone|1|João|Menezes|9/21/2018|Recife|5300|NaN|5300|
|184|2561|HL1918|iPhone|3|Bruna|Londero|4/17/2018|Recife|5300|NaN|15900|
|185|2563|HL1148|Câmera|3|Gustavo|Thome|8/8/2018|Recife|2100|NaN|6300|
|186|2568|HL8851|Notebook|1|Guilherme|Lima|8/6/2018|Recife|3500|NaN|3500|
|187|2573|HL4379|Televisão|1|Carlos|Barbosa|2/14/2018|Recife|2500|NaN|2500|
|188|2591|HL1918|iPhone|5|Nathalia|Ventura|11/2/2018|Recife|5300|NaN|26500|
|189|2604|HL4379|Televisão|5|Felipe|Jorge|12/31/2018|Recife|2500|NaN|12500|
|190|2607|HL2714|Tablet|3|Diego|Marchesi|6/9/2018|Recife|1600|NaN|4800|
|191|2615|HL1918|iPhone|5|Mariane|Racy|11/7/2018|Recife|5300|NaN|26500|
|192|2616|HL1918|iPhone|3|Gustavo|Gomes|11/17/2018|Recife|5300|NaN|15900|
|193|2618|HL1918|iPhone|5|Matheus|Silva|9/24/2018|Recife|5300|NaN|26500|
|194|2640|HL7348|SmartWatch|3|Caio|Fernandes|5/24/2018|Recife|1400|NaN|4200|
|195|2651|HL1148|Câmera|1|Caroline|Cavalcanti|6/23/2018|Recife|2100|NaN|2100|
|196|2656|HL8851|Notebook|3|Bianca|Allevato|3/13/2018|Recife|3500|NaN|10500|
|197|2682|HL1148|Câmera|4|Victor|Gomes|4/2/2018|Recife|2100|NaN|8400|
|198|2683|HL8851|Notebook|2|Victor|Lira|10/9/2018|Recife|3500|NaN|7000|
|199|2698|HL1918|iPhone|3|Victor|Gomes|12/24/2018|Recife|5300|NaN|15900|
|200|2705|HL2714|Tablet|5|Lucas|Chagas|12/5/2018|Recife|1600|NaN|8000|
|201|2716|HL8851|Notebook|1|Carlos|Araujo|4/19/2018|Recife|3500|NaN|3500|
|202|2719|HL1148|Câmera|3|Bianca|Allevato|2/19/2018|Recife|2100|NaN|6300|
|203|2722|HL1148|Câmera|2|Luis|Garcia|6/9/2018|Recife|2100|NaN|4200|
|204|2732|HL1918|iPhone|2|Julia|Silva|2/5/2018|Recife|5300|NaN|10600|
|205|2755|HL4379|Televisão|4|Clara|Silveira|12/25/2018|Recife|2500|NaN|10000|
|206|2780|HL2714|Tablet|4|Fabio|Ramos|7/18/2018|Recife|1600|NaN|6400|
|207|2782|HL8851|Notebook|5|Luiz|Conceição|2/19/2018|Recife|3500|NaN|17500|
|208|2786|HL1918|iPhone|5|Daniel|Monteiro|6/14/2018|Recife|5300|NaN|26500|
|209|2792|HL9962|Android|4|Ana|Soledade|2/9/2018|Recife|3400|NaN|13600|
|210|2815|HL1918|iPhone|5|Sthefeson|Pereira|12/11/2018|Recife|5300|NaN|26500|
|211|2817|HL2714|Tablet|1|Rodrigo|Feijo|9/29/2018|Recife|1600|NaN|1600|
|212|2819|HL8851|Notebook|2|Breno|Costa|1/25/2018|Recife|3500|NaN|7000|
|213|2824|HL1918|iPhone|1|Pedro|Bitencourt|8/5/2018|Recife|5300|NaN|5300|
|214|2878|HL1918|iPhone|2|Bernardo|Borges|2/4/2018|Recife|5300|NaN|10600|
|215|2895|HL1918|iPhone|1|Deysiane|Bach|3/21/2018|Recife|5300|NaN|5300|
|216|2899|HL1918|iPhone|4|Norman|Jimbo|4/5/2018|Recife|5300|NaN|21200|
|217|2903|HL9962|Android|1|Gabrielle|Viríssimo|9/27/2018|Recife|3400|NaN|3400|
|218|2905|HL8851|Notebook|1|João|Peçanha|1/18/2018|Recife|3500|NaN|3500|
|219|2916|HL4379|Televisão|1|Mariana|Barrozo|8/10/2018|Recife|2500|NaN|2500|
|220|2924|HL7348|SmartWatch|2|Ana|Silva|4/21/2018|Recife|1400|NaN|2800|
|221|2949|HL2714|Tablet|4|Sarah|Souza|7/25/2018|Recife|1600|NaN|6400|
|222|2959|HL9962|Android|5|Ana|Soledade|11/25/2018|Recife|3400|NaN|17000|
|223|2973|HL4379|Televisão|1|Caio|Fernandes|8/17/2018|Recife|2500|NaN|2500|
|224|2978|HL7348|SmartWatch|3|Luis|Silva|3/30/2018|Recife|1400|NaN|4200|
|225|2983|HL7348|SmartWatch|4|Henrique|Oliveira|12/7/2018|Recife|1400|NaN|5600|
|226|2988|HL1918|iPhone|2|Beatriz|Almeida|2/15/2018|Recife|5300|NaN|10600|
|227|2990|HL4379|Televisão|2|Lucas|Freire|7/31/2018|Recife|2500|NaN|5000|
|228|2991|HL7348|SmartWatch|4|Paulo|Campos|10/30/2018|Recife|1400|NaN|5600|
|229|3012|HL8851|Notebook|1|Renan|Cunha|9/19/2018|Recife|3500|NaN|3500|
|230|3016|HL4379|Televisão|3|Paola|Abreu|10/1/2018|Recife|2500|NaN|7500|
|231|3031|HL1148|Câmera|1|Lucas|Cavalcanti|5/2/2018|Recife|2100|NaN|2100|
|232|3053|HL9962|Android|5|João|Monteiro|11/14/2018|Recife|3400|NaN|17000|
|233|3097|HL9962|Android|5|Carolina|Vasconcelos|2/20/2018|Recife|3400|NaN|17000|
|234|3123|HL1148|Câmera|5|Giulia|Lopes|9/29/2018|Recife|2100|NaN|10500|
|235|3150|HL1918|iPhone|4|Marina|Perdomo|8/2/2018|Recife|5300|NaN|21200|
|236|3173|HL9962|Android|5|Joyce|Souza|6/29/2018|Recife|3400|NaN|17000|
|237|3181|HL1918|iPhone|1|Brenno|Santos|2/2/2018|Recife|5300|NaN|5300|
|238|3186|HL7348|SmartWatch|3|Caio|Ferreira|3/3/2018|Recife|1400|NaN|4200|
|239|3192|HL7348|SmartWatch|3|Rojane|Lima|5/19/2018|Recife|1400|NaN|4200|
|240|3200|HL4379|Televisão|1|Fernanda|Junior|4/25/2018|Recife|2500|NaN|2500|
|241|3212|HL1918|iPhone|2|Pedro|Xavier|6/22/2018|Recife|5300|NaN|10600|
|242|3215|HL4379|Televisão|1|Marina|Aragão|8/8/2018|Recife|2500|NaN|2500|
|243|3217|HL2714|Tablet|2|Matheus|Ramos|11/2/2018|Recife|1600|NaN|3200|
|244|3249|HL2714|Tablet|3|Aline|Andrade|1/10/2018|Recife|1600|NaN|4800|
|245|3271|HL7348|SmartWatch|4|Pedro|Jorge|10/21/2018|Recife|1400|NaN|5600|
|246|3295|HL2714|Tablet|5|Ana|Michetti|3/12/2018|Recife|1600|NaN|8000|
|247|3306|HL1918|iPhone|2|Rebeca|Reis|7/12/2018|Recife|5300|NaN|10600|
|248|3358|HL9962|Android|3|Patrícia|Amaral|12/15/2018|Recife|3400|NaN|10200|
|249|3368|HL2714|Tablet|3|Viviane|Cunha|12/24/2018|Recife|1600|NaN|4800|
|250|3369|HL1918|iPhone|3|João|Aires|3/1/2018|Recife|5300|NaN|15900|
|251|3376|HL1918|iPhone|3|Carolina|Santos|8/19/2018|Recife|5300|NaN|15900|
|252|3385|HL9962|Android|3|Pedro|Santana|6/28/2018|Recife|3400|NaN|10200|
|253|3388|HL1918|iPhone|4|Catarina|Teixeira|3/31/2018|Recife|5300|NaN|21200|
|254|3391|HL4379|Televisão|3|Gabriel|Azevedo|1/1/2018|Recife|2500|NaN|7500|
|255|3438|HL1918|iPhone|3|Elaine|Santos|10/25/2018|Recife|5300|NaN|15900|
|256|3470|HL1148|Câmera|4|Rafaela|Rodrigues|1/11/2018|Recife|2100|NaN|8400|
|257|3473|HL8851|Notebook|4|Matheus|Figueiredo|3/18/2018|Recife|3500|NaN|14000|
|258|3480|HL1918|iPhone|2|Jônatas|Tanaka|8/26/2018|Recife|5300|NaN|10600|
|259|3506|HL1918|iPhone|4|Rafaela|Feio|7/18/2018|Recife|5300|NaN|21200|
|260|3518|HL4379|Televisão|4|Carlos|Souza|9/3/2018|Recife|2500|NaN|10000|
|261|3531|HL4379|Televisão|4|Cícero|Lima|6/28/2018|Recife|2500|NaN|10000|
|262|3536|HL9962|Android|5|Pedro|Ronfini|3/28/2018|Recife|3400|NaN|17000|
|263|3551|HL1918|iPhone|4|Silvio|Fahrnholz|11/23/2018|Recife|5300|NaN|21200|
|264|3583|HL4379|Televisão|4|Michelle|Miura|4/23/2018|Recife|2500|NaN|10000|
|265|3641|HL7348|SmartWatch|4|Wen|Santos|3/13/2018|Recife|1400|NaN|5600|
|266|3648|HL1918|iPhone|1|Matheus|Delgado|7/10/2018|Recife|5300|NaN|5300|
|267|3652|HL2714|Tablet|2|Ana|Soledade|5/10/2018|Recife|1600|NaN|3200|
|268|3673|HL7348|SmartWatch|1|Diego|Rodrigues|2/12/2018|Recife|1400|NaN|1400|
|269|3680|HL9962|Android|1|Isabella|Montanholi|6/28/2018|Recife|3400|NaN|3400|
|270|3694|HL4379|Televisão|5|Patrícia|Fernandes|7/28/2018|Recife|2500|NaN|12500|
|271|3703|HL2714|Tablet|3|Hygor|Essaber|12/21/2018|Recife|1600|NaN|4800|
|272|3806|HL1918|iPhone|4|Bernardo|Botelho|3/2/2018|Recife|5300|NaN|21200|
|273|3815|HL9962|Android|4|Carlos|Souza|1/26/2018|Recife|3400|NaN|13600|
|274|3819|HL4379|Televisão|1|Carlos|Barbosa|6/19/2018|Recife|2500|NaN|2500|
|275|3861|HL1918|iPhone|2|Sandy|Figueiredo|11/25/2018|Recife|5300|NaN|10600|
|276|3870|HL1918|iPhone|5|Paulo|Campos|10/24/2018|Recife|5300|NaN|26500|
|277|3871|HL8851|Notebook|5|Marcelo|Pereira|8/31/2018|Recife|3500|NaN|17500|
|278|3874|HL8851|Notebook|5|Bernardo|Soares|4/14/2018|Recife|3500|NaN|17500|
|279|3882|HL1918|iPhone|1|Carlos|Mesquita|11/19/2018|Recife|5300|NaN|5300|
|280|3893|HL1918|iPhone|3|Raphael|Rezende|3/5/2018|Recife|5300|NaN|15900|
|281|3909|HL4379|Televisão|2|Ana|Soledade|6/8/2018|Recife|2500|NaN|5000|
|282|3919|HL8851|Notebook|2|Bárbara|Lima|8/28/2018|Recife|3500|NaN|7000|
|283|3922|HL1918|iPhone|4|Rodrigo|Mendes|5/24/2018|Recife|5300|NaN|21200|
|284|3929|HL1148|Câmera|2|Giovanna|Santos|4/23/2018|Recife|2100|NaN|4200|
|285|3941|HL4379|Televisão|5|Bernardo|Ribeiro|7/3/2018|Recife|2500|NaN|12500|
|286|3943|HL1918|iPhone|4|Gabriel|Assis|10/27/2018|Recife|5300|NaN|21200|
|287|3947|HL1918|iPhone|1|Roberto|Mattos|12/28/2018|Recife|5300|NaN|5300|
|288|3952|HL1918|iPhone|5|Raul|Silveira|1/1/2018|Recife|5300|NaN|26500|
|289|3953|HL9962|Android|1|Paula|Cavalcanti|9/25/2018|Recife|3400|NaN|3400|
|290|3972|HL9962|Android|1|Diogo|Peixoto|4/30/2018|Recife|3400|NaN|3400|
|291|3974|HL1918|iPhone|2|Júlio|Freire|11/1/2018|Recife|5300|NaN|10600|
|292|4003|HL7348|SmartWatch|3|Luis|Silva|8/8/2018|Recife|1400|NaN|4200|
|293|4007|HL8851|Notebook|5|Roberta|Pimenta|9/8/2018|Recife|3500|NaN|17500|
|294|4023|HL9962|Android|2|Carlos|Assis|6/30/2018|Recife|3400|NaN|6800|
|295|4037|HL1918|iPhone|3|Juliana|Hollander|12/20/2018|Recife|5300|NaN|15900|
|296|4038|HL1918|iPhone|5|Isabela|Teixeira|9/3/2018|Recife|5300|NaN|26500|
|297|4041|HL7348|SmartWatch|5|Mônica|Rotolo|10/31/2018|Recife|1400|NaN|7000|
|298|4043|HL7348|SmartWatch|1|Juliana|Hollander|12/26/2018|Recife|1400|NaN|1400|
|299|4085|HL8851|Notebook|1|Felipe|Cavalcanti|9/17/2018|Recife|3500|NaN|3500|
|300|4089|HL1918|iPhone|5|Bruna|Soares|9/30/2018|Recife|5300|NaN|26500|
|301|4094|HL1148|Câmera|1|Glenda|Santos|2/7/2018|Recife|2100|NaN|2100|
|302|4103|HL1918|iPhone|3|Gustavo|Accardo|5/6/2018|Recife|5300|NaN|15900|
|303|4105|HL9962|Android|1|Felipe|Mendonça|8/25/2018|Recife|3400|NaN|3400|
|304|4137|HL1918|iPhone|2|Carolina|Santos|2/19/2018|Recife|5300|NaN|10600|
|305|4145|HL1148|Câmera|2|Eduardo|Nunes|5/12/2018|Recife|2100|NaN|4200|
|306|4152|HL1148|Câmera|1|Laura|Araujo|10/28/2018|Recife|2100|NaN|2100|
|307|4157|HL4379|Televisão|1|Ian|Almeida|10/11/2018|Recife|2500|NaN|2500|
|308|4158|HL8851|Notebook|1|Jorge|Carvalho|10/9/2018|Recife|3500|NaN|3500|
|309|4168|HL1918|iPhone|3|Hércules|Júnior|8/25/2018|Recife|5300|NaN|15900|
|310|4179|HL1148|Câmera|4|Adrielle|Gabriel|8/11/2018|Recife|2100|NaN|8400|
|311|4186|HL8851|Notebook|5|Matheus|Tostes|2/15/2018|Recife|3500|NaN|17500|
|312|4188|HL1918|iPhone|5|Thales|Santos|3/27/2018|Recife|5300|NaN|26500|
|313|4194|HL1148|Câmera|1|Eric|Júnior|5/7/2018|Recife|2100|NaN|2100|
|314|4218|HL4379|Televisão|1|Guilherme|Monteiro|5/10/2018|Recife|2500|NaN|2500|
|315|4270|HL4379|Televisão|5|Diego|Mello|9/16/2018|Recife|2500|NaN|12500|
|316|4276|HL4379|Televisão|4|Daniel|Terra|4/5/2018|Recife|2500|NaN|10000|
|317|4278|HL1918|iPhone|5|Guilherme|Vianna|8/3/2018|Recife|5300|NaN|26500|
|318|4281|HL9962|Android|1|Mariane|Racy|7/19/2018|Recife|3400|NaN|3400|
|319|4287|HL4379|Televisão|4|Giovana|Vilela|10/2/2018|Recife|2500|NaN|10000|
|320|4294|HL4379|Televisão|1|Gabrielle|Viríssimo|6/2/2018|Recife|2500|NaN|2500|
|321|4328|HL2714|Tablet|2|João|Ribeiro|12/27/2018|Recife|1600|NaN|3200|
|322|4363|HL9962|Android|5|Anna|Silva|4/21/2018|Recife|3400|NaN|17000|
|323|4409|HL7348|SmartWatch|1|Pedro|Dalforne|5/4/2018|Recife|1400|NaN|1400|
|324|4411|HL7348|SmartWatch|5|Pedro|Macckione|10/5/2018|Recife|1400|NaN|7000|
|325|4429|HL9962|Android|4|Larissa|Nauenberg|1/22/2018|Recife|3400|NaN|13600|
|326|4444|HL1148|Câmera|4|Bianca|Allevato|8/6/2018|Recife|2100|NaN|8400|
|327|4466|HL2714|Tablet|2|Felipe|Paulo|1/19/2018|Recife|1600|NaN|3200|
|328|4468|HL1918|iPhone|5|Victoria|Tavares|6/19/2018|Recife|5300|NaN|26500|
|329|4471|HL4379|Televisão|5|Marcelo|Magalhães|9/1/2018|Recife|2500|NaN|12500|
|330|4478|HL8851|Notebook|2|Alexandre|Rodriguez|6/3/2018|Recife|3500|NaN|7000|
|331|4481|HL1918|iPhone|5|Renan|Ventura|2/17/2018|Recife|5300|NaN|26500|
|332|4494|HL1918|iPhone|4|Renan|Nucci|10/27/2018|Recife|5300|NaN|21200|
|333|4507|HL2714|Tablet|3|Isabel|Mesquita|11/30/2018|Recife|1600|NaN|4800|
|334|4541|HL1918|iPhone|1|Eduardo|Lopes|8/5/2018|Recife|5300|NaN|5300|
|335|4557|HL4379|Televisão|1|Amanda|Braga|12/11/2018|Recife|2500|NaN|2500|
|336|4576|HL9962|Android|3|Breno|Britto|11/3/2018|Recife|3400|NaN|10200|
|337|4587|HL4379|Televisão|4|Raphael|Coelho|1/3/2018|Recife|2500|NaN|10000|
|338|4665|HL9962|Android|4|Daniel|Ortiz|10/8/2018|Recife|3400|NaN|13600|
|339|4670|HL1918|iPhone|2|Adrielle|Gabriel|7/12/2018|Recife|5300|NaN|10600|
|340|4674|HL4379|Televisão|2|Jéssica|Teixeira|10/1/2018|Recife|2500|NaN|5000|
|341|4684|HL1918|iPhone|3|Lucas|Assunção|12/17/2018|Recife|5300|NaN|15900|
|342|4689|HL2714|Tablet|4|Caroline|Pinto|4/30/2018|Recife|1600|NaN|6400|
|343|4695|HL1918|iPhone|5|Guilherme|Monteiro|6/12/2018|Recife|5300|NaN|26500|
|344|4705|HL8851|Notebook|3|Carolina|Figueiredo|2/28/2018|Recife|3500|NaN|10500|
|345|4716|HL1918|iPhone|2|Rebeca|Reis|8/31/2018|Recife|5300|NaN|10600|
|346|4722|HL4379|Televisão|4|Guilherme|Jordao|10/27/2018|Recife|2500|NaN|10000|
|347|4765|HL1918|iPhone|4|Pedro|Delgado|2/1/2018|Recife|5300|NaN|21200|
|348|4770|HL8851|Notebook|3|Pedro|Cardoso|8/17/2018|Recife|3500|NaN|10500|
|349|4794|HL7348|SmartWatch|2|Debora|Silva|10/4/2018|Recife|1400|NaN|2800|
|350|4800|HL2714|Tablet|3|Breno|Costa|10/5/2018|Recife|1600|NaN|4800|
|351|4809|HL2714|Tablet|4|Nathan|Morelli|4/13/2018|Recife|1600|NaN|6400|
|352|4816|HL1918|iPhone|4|Brenno|Santos|11/29/2018|Recife|5300|NaN|21200|
|353|4820|HL1148|Câmera|2|Lucas|Neto|8/27/2018|Recife|2100|NaN|4200|
|354|4829|HL1918|iPhone|4|Guido|Monteiro|12/17/2018|Recife|5300|NaN|21200|
|355|4840|HL9962|Android|3|Anna|Maia|8/1/2018|Recife|3400|NaN|10200|
|356|4850|HL4379|Televisão|5|Victor|Firmino|8/22/2018|Recife|2500|NaN|12500|
|357|4857|HL1148|Câmera|2|Pedro|Santana|3/29/2018|Recife|2100|NaN|4200|
|358|4858|HL1148|Câmera|3|Ruan|Lopes|3/16/2018|Recife|2100|NaN|6300|
|359|4860|HL1918|iPhone|2|Lucas|Almeida|11/30/2018|Recife|5300|NaN|10600|
|360|4878|HL2714|Tablet|3|Alessandra|Martins|5/30/2018|Recife|1600|NaN|4800|
|361|4892|HL9962|Android|3|Marina|Delgado|12/20/2018|Recife|3400|NaN|10200|
|362|4894|HL1918|iPhone|5|Rafaela|Feio|4/3/2018|Recife|5300|NaN|26500|
|363|4905|HL1918|iPhone|5|Mariane|Racy|9/15/2018|Recife|5300|NaN|26500|
|364|4906|HL1918|iPhone|2|Lara|Moreira|1/2/2018|Recife|5300|NaN|10600|
|365|4928|HL4379|Televisão|2|Andressa|Chou|7/27/2018|Recife|2500|NaN|5000|
|366|4936|HL1918|iPhone|3|Marcela|Johnson|9/10/2018|Recife|5300|NaN|15900|
|367|4938|HL1918|iPhone|5|Marina|Aragão|7/17/2018|Recife|5300|NaN|26500|
|368|4942|HL4379|Televisão|5|Lucas|Fontoura|8/18/2018|Recife|2500|NaN|12500|
|369|4943|HL1918|iPhone|1|Catarina|Teixeira|1/15/2018|Recife|5300|NaN|5300|
|370|4973|HL2714|Tablet|3|Pedro|Rodrigues|11/4/2018|Recife|1600|NaN|4800|
|371|4978|HL1918|iPhone|5|Roberta|Teixeira|5/6/2018|Recife|5300|NaN|26500|
|372|4995|HL1918|iPhone|3|Joyce|Medina|4/9/2018|Recife|5300|NaN|15900|
|373|5048|HL8851|Notebook|2|Felipe|Cavalcanti|8/2/2018|Recife|3500|NaN|7000|
|374|5049|HL2714|Tablet|5|Lucas|Valim|6/23/2018|Recife|1600|NaN|8000|
|375|5059|HL4379|Televisão|3|Caio|Ferreira|9/28/2018|Recife|2500|NaN|7500|
|376|5087|HL7348|SmartWatch|5|Victor|Corrêa|12/1/2018|Recife|1400|NaN|7000|
|377|5110|HL4379|Televisão|3|Anderson|Barreto|2/14/2018|Recife|2500|NaN|7500|
|378|5118|HL1918|iPhone|1|Jônatas|Tanaka|12/29/2018|Recife|5300|NaN|5300|
|379|5126|HL1918|iPhone|3|Wilson|Brandão|10/15/2018|Recife|5300|NaN|15900|
|380|5131|HL1148|Câmera|1|Paula|Carneiro|6/14/2018|Recife|2100|NaN|2100|
|381|5152|HL8851|Notebook|1|Maria|Junior|1/12/2018|Recife|3500|NaN|3500|
|382|5158|HL2714|Tablet|5|Beatriz|Rodrigues|12/2/2018|Recife|1600|NaN|8000|
|383|5215|HL7348|SmartWatch|3|Paula|Isbelle|7/23/2018|Recife|1400|NaN|4200|
|384|5263|HL2714|Tablet|3|Henrique|Oliveira|12/30/2018|Recife|1600|NaN|4800|
|385|5272|HL1918|iPhone|4|Priscila|Carvalho|5/21/2018|Recife|5300|NaN|21200|
|386|5290|HL4379|Televisão|2|Stela|Mendonça|5/28/2018|Recife|2500|NaN|5000|
|387|5318|HL1918|iPhone|4|Jorge|Carvalho|12/29/2018|Recife|5300|NaN|21200|
|388|5320|HL1918|iPhone|2|Henrique|Silva|7/4/2018|Recife|5300|NaN|10600|
|389|5340|HL9962|Android|5|Matheus|Gomes|2/9/2018|Recife|3400|NaN|17000|
|390|5359|HL2714|Tablet|2|Wellington|Duarte|4/26/2018|Recife|1600|NaN|3200|
|391|5388|HL4379|Televisão|4|William|Mendonça|12/30/2018|Recife|2500|NaN|10000|
|392|5402|HL4379|Televisão|3|Pedro|Bitencourt|9/17/2018|Recife|2500|NaN|7500|
|393|5405|HL4379|Televisão|2|Victor|Magalhães|10/9/2018|Recife|2500|NaN|5000|
|394|5415|HL4379|Televisão|5|Joyce|Souza|11/30/2018|Recife|2500|NaN|12500|
|395|5428|HL4379|Televisão|1|Luiza|Cavalcanti|4/26/2018|Recife|2500|NaN|2500|
|396|5436|HL7348|SmartWatch|1|Joyce|Medina|5/5/2018|Recife|1400|NaN|1400|
|397|5453|HL4379|Televisão|3|Lais|Candido|7/30/2018|Recife|2500|NaN|7500|
|398|5465|HL1148|Câmera|5|Mateus|Franco|4/14/2018|Recife|2100|NaN|10500|
|399|5508|HL1148|Câmera|5|Sthefeson|Barroso|7/15/2018|Recife|2100|NaN|10500|
|400|5532|HL4379|Televisão|4|Manuela|Ferreira|3/7/2018|Recife|2500|NaN|10000|
|401|5585|HL1918|iPhone|2|Allan|Guedes|9/20/2018|Recife|5300|NaN|10600|
|402|5612|HL8851|Notebook|5|Bárbara|Cavalcante|1/31/2018|Recife|3500|NaN|17500|
|403|5647|HL2714|Tablet|1|Bruno|Barcessat|10/5/2018|Recife|1600|NaN|1600|
|404|5670|HL4379|Televisão|4|Wilson|Vianna|1/12/2018|Recife|2500|NaN|10000|
|405|5672|HL1918|iPhone|4|Danilo|Alves|12/22/2018|Recife|5300|NaN|21200|
|406|5692|HL1918|iPhone|5|Isabel|Leite|5/2/2018|Recife|5300|NaN|26500|
|407|5713|HL1918|iPhone|1|Luana|Santana|2/14/2018|Recife|5300|NaN|5300|
|408|5719|HL9962|Android|1|Tiago|Pereira|7/26/2018|Recife|3400|NaN|3400|
|409|5720|HL8851|Notebook|1|Stefan|Nunes|3/11/2018|Recife|3500|NaN|3500|
|410|5735|HL4379|Televisão|1|Ana|Silva|8/23/2018|Recife|2500|NaN|2500|
|411|5740|HL4379|Televisão|1|Silvio|Fahrnholz|6/14/2018|Recife|2500|NaN|2500|
|412|5743|HL4379|Televisão|3|Ylana|Teraoka|6/17/2018|Recife|2500|NaN|7500|
|413|5753|HL2714|Tablet|1|Wilson|Meirelles|3/4/2018|Recife|1600|NaN|1600|
|414|5790|HL1918|iPhone|4|João|Alves|12/29/2018|Recife|5300|NaN|21200|
|415|5807|HL1148|Câmera|2|Roberto|Nogueira|6/6/2018|Recife|2100|NaN|4200|
|416|5813|HL8851|Notebook|5|Raul|Silveira|12/28/2018|Recife|3500|NaN|17500|
|417|5815|HL2714|Tablet|2|Vinícius|Antunes|12/10/2018|Recife|1600|NaN|3200|
|418|5818|HL1918|iPhone|3|João|Ribeiro|11/29/2018|Recife|5300|NaN|15900|
|419|5826|HL1918|iPhone|1|Pedro|Dalforne|11/19/2018|Recife|5300|NaN|5300|
|420|5830|HL4379|Televisão|2|Raissa|Negrelli|8/9/2018|Recife|2500|NaN|5000|
|421|5835|HL7348|SmartWatch|1|Myllena|Corrêa|8/2/2018|Recife|1400|NaN|1400|
|422|5839|HL1148|Câmera|4|Jéssica|Netto|10/22/2018|Recife|2100|NaN|8400|
|423|5849|HL9962|Android|1|Renan|Firmino|9/5/2018|Recife|3400|NaN|3400|
|424|5851|HL4379|Televisão|4|Itai|Puntel|5/17/2018|Recife|2500|NaN|10000|
|425|5853|HL2714|Tablet|4|Carolina|Siqueira|7/22/2018|Recife|1600|NaN|6400|
|426|5864|HL1918|iPhone|2|Gabriel|Rocha|1/9/2018|Recife|5300|NaN|10600|
|427|5865|HL1918|iPhone|5|Raphael|Kurtz|7/16/2018|Recife|5300|NaN|26500|
|428|5902|HL4379|Televisão|5|Antônio|Soares|10/7/2018|Recife|2500|NaN|12500|
|429|5905|HL4379|Televisão|3|Jessica|Ferreira|4/24/2018|Recife|2500|NaN|7500|
|430|5914|HL4379|Televisão|4|Maurício|Dias|12/30/2018|Recife|2500|NaN|10000|
|431|5915|HL8851|Notebook|3|Rodrigo|Silva|8/5/2018|Recife|3500|NaN|10500|
|432|5934|HL1148|Câmera|5|Rebeca|Taylor|12/18/2018|Recife|2100|NaN|10500|
|433|5948|HL1918|iPhone|2|Raphael|Kurtz|1/20/2018|Recife|5300|NaN|10600|
|434|5990|HL2714|Tablet|5|Antonio|Manhães|6/5/2018|Recife|1600|NaN|8000|
|435|5999|HL1918|iPhone|1|Paula|Isbelle|9/25/2018|Recife|5300|NaN|5300|
|436|6004|HL1148|Câmera|5|Amanda|Amaral|5/24/2018|Recife|2100|NaN|10500|
|437|6016|HL9962|Android|5|Raissa|Pinheiro|6/5/2018|Recife|3400|NaN|17000|
|438|6023|HL1148|Câmera|5|Rodrigo|Feijo|11/22/2018|Recife|2100|NaN|10500|
|439|6040|HL1918|iPhone|4|Raissa|Maia|6/23/2018|Recife|5300|NaN|21200|
|440|6067|HL1148|Câmera|1|Rogério|Pereira|10/19/2018|Recife|2100|NaN|2100|
|441|6082|HL9962|Android|2|Arthur|Pereira|10/8/2018|Recife|3400|NaN|6800|
|442|6084|HL4379|Televisão|3|Igor|Lima|2/2/2018|Recife|2500|NaN|7500|
|443|6105|HL1918|iPhone|2|Pedro|Santana|7/29/2018|Recife|5300|NaN|10600|
|444|6123|HL4379|Televisão|3|Giovana|Vilela|4/16/2018|Recife|2500|NaN|7500|
|445|6147|HL1918|iPhone|1|Isabela|Teixeira|8/6/2018|Recife|5300|NaN|5300|
|446|6171|HL9962|Android|5|Rebeca|Manhães|12/23/2018|Recife|3400|NaN|17000|
|447|6176|HL1918|iPhone|3|Aline|Mello|8/8/2018|Recife|5300|NaN|15900|
|448|6180|HL8851|Notebook|1|Laís|Oliveira|8/4/2018|Recife|3500|NaN|3500|
|449|6183|HL4379|Televisão|3|Ulisses|Filho|10/18/2018|Recife|2500|NaN|7500|
|450|6185|HL1148|Câmera|5|Breno|Caputo|8/8/2018|Recife|2100|NaN|10500|
|451|6186|HL9962|Android|3|David|Campelo|6/16/2018|Recife|3400|NaN|10200|
|452|6204|HL7348|SmartWatch|3|Raul|Junqueira|5/13/2018|Recife|1400|NaN|4200|
|453|6213|HL7348|SmartWatch|4|Fernanda|Silva|7/17/2018|Recife|1400|NaN|5600|
|454|6214|HL1148|Câmera|1|Marcela|Gasperi|6/17/2018|Recife|2100|NaN|2100|
|455|6227|HL2714|Tablet|5|Lucas|Machado|4/18/2018|Recife|1600|NaN|8000|
|456|6246|HL1918|iPhone|4|João|Oliveira|7/31/2018|Recife|5300|NaN|21200|
|457|6271|HL4379|Televisão|3|Daniel|Terra|1/7/2018|Recife|2500|NaN|7500|
|458|6279|HL9962|Android|2|Pedro|Macckione|2/15/2018|Recife|3400|NaN|6800|
|459|6285|HL4379|Televisão|5|Fernanda|Rubim|3/18/2018|Recife|2500|NaN|12500|
|460|6338|HL4379|Televisão|1|David|Campelo|5/3/2018|Recife|2500|NaN|2500|
|461|6371|HL8851|Notebook|4|Lucas|Lemos|9/24/2018|Recife|3500|NaN|14000|
|462|6387|HL8851|Notebook|1|Rodrigo|Mendes|6/5/2018|Recife|3500|NaN|3500|
|463|6391|HL1148|Câmera|1|João|Menezes|6/25/2018|Recife|2100|NaN|2100|
|464|6421|HL1918|iPhone|4|Eduardo|Quindeler|1/19/2018|Recife|5300|NaN|21200|
|465|6442|HL9962|Android|1|Isabela|Resende|12/31/2018|Recife|3400|NaN|3400|
|466|6446|HL4379|Televisão|4|Pedro|Santos|7/30/2018|Recife|2500|NaN|10000|
|467|6531|HL7348|SmartWatch|5|Antônio|Soares|1/26/2018|Recife|1400|NaN|7000|
|468|6624|HL1918|iPhone|2|Luis|Silva|12/1/2018|Recife|5300|NaN|10600|
|469|6634|HL1918|iPhone|1|Ana|Júnior|10/12/2018|Recife|5300|NaN|5300|
|470|6637|HL1918|iPhone|2|Victor|Lira|7/23/2018|Recife|5300|NaN|10600|
|471|6661|HL4379|Televisão|3|Luiza|Cavalcanti|3/23/2018|Recife|2500|NaN|7500|
|472|6663|HL2714|Tablet|4|Thayna|Martins|5/29/2018|Recife|1600|NaN|6400|
|473|6664|HL9962|Android|4|Jéssica|Stefanelli|10/5/2018|Recife|3400|NaN|13600|
|474|6676|HL2714|Tablet|3|Felipe|Mello|4/27/2018|Recife|1600|NaN|4800|
|475|6679|HL1918|iPhone|2|Raphael|Ferman|8/11/2018|Recife|5300|NaN|10600|
|476|6686|HL1918|iPhone|4|Lucas|Freire|8/12/2018|Recife|5300|NaN|21200|
|477|6687|HL4379|Televisão|4|Raphael|Guedes|7/12/2018|Recife|2500|NaN|10000|
|478|6720|HL1918|iPhone|2|Isabel|Mesquita|2/25/2018|Recife|5300|NaN|10600|
|479|6722|HL4379|Televisão|1|Desirée|Heimlich|1/22/2018|Recife|2500|NaN|2500|
|480|6724|HL9962|Android|1|Pedro|Conceição|4/7/2018|Recife|3400|NaN|3400|
|481|6725|HL1918|iPhone|5|Marina|Cormack|5/18/2018|Recife|5300|NaN|26500|
|482|6733|HL1918|iPhone|4|Felipe|Mello|10/15/2018|Recife|5300|NaN|21200|
|483|6736|HL9962|Android|3|Gustavo|Azevedo|9/29/2018|Recife|3400|NaN|10200|
|484|6743|HL1918|iPhone|4|Thales|Andrade|8/28/2018|Recife|5300|NaN|21200|
|485|6744|HL2714|Tablet|5|Pedro|Macckione|2/26/2018|Recife|1600|NaN|8000|
|486|6748|HL1918|iPhone|1|Roberto|Nogueira|8/14/2018|Recife|5300|NaN|5300|
|487|6795|HL4379|Televisão|3|Thales|Fanara|2/18/2018|Recife|2500|NaN|7500|
|488|6796|HL8851|Notebook|4|Mateus|Duque|6/23/2018|Recife|3500|NaN|14000|
|489|6832|HL9962|Android|5|Natalia|Guedes|8/25/2018|Recife|3400|NaN|17000|
|490|6834|HL1918|iPhone|1|Felipe|Júnior|1/24/2018|Recife|5300|NaN|5300|
|491|6842|HL2714|Tablet|1|Rebeca|Taylor|9/11/2018|Recife|1600|NaN|1600|
|492|6853|HL1918|iPhone|4|Sthefeson|Pereira|12/11/2018|Recife|5300|NaN|21200|
|493|6885|HL4379|Televisão|1|Itai|Puntel|10/5/2018|Recife|2500|NaN|2500|
|494|6893|HL8851|Notebook|3|Ulisses|Filho|7/12/2018|Recife|3500|NaN|10500|
|495|6912|HL2714|Tablet|1|João|Peçanha|5/23/2018|Recife|1600|NaN|1600|
|496|6931|HL9962|Android|4|Rogério|Gentile|10/13/2018|Recife|3400|NaN|13600|
|497|6951|HL8851|Notebook|4|Rafael|Rocha|8/5/2018|Recife|3500|NaN|14000|
|498|6957|HL1148|Câmera|3|Beatriz|Biase|7/12/2018|Recife|2100|NaN|6300|
|499|6967|HL7348|SmartWatch|3|Maria|Junior|2/27/2018|Recife|1400|NaN|4200|
|500|6977|HL1918|iPhone|1|Carla|Zakhm|12/27/2018|Recife|5300|NaN|5300|
|501|6981|HL1918|iPhone|2|Fernanda|Silva|12/10/2018|Recife|5300|NaN|10600|
|502|6986|HL1918|iPhone|5|Juliana|Silva|12/28/2018|Recife|5300|NaN|26500|
|503|6993|HL1918|iPhone|1|Luana|Santos|7/3/2018|Recife|5300|NaN|5300|
|504|7004|HL7348|SmartWatch|4|Julia|Leig|3/10/2018|Recife|1400|NaN|5600|
|505|7010|HL4379|Televisão|2|Antonio|Bernhardt|6/4/2018|Recife|2500|NaN|5000|
|506|7018|HL1148|Câmera|5|Barbara|Procaci|12/2/2018|Recife|2100|NaN|10500|
|507|7027|HL2714|Tablet|1|Raissa|Negrelli|3/27/2018|Recife|1600|NaN|1600|
|508|7050|HL4379|Televisão|5|Gustavo|Junior|7/24/2018|Recife|2500|NaN|12500|
|509|7061|HL1148|Câmera|1|Ana|Bôas|8/6/2018|Recife|2100|NaN|2100|
|510|7068|HL2714|Tablet|4|Bruno|Barcessat|8/28/2018|Recife|1600|NaN|6400|
|511|7070|HL1918|iPhone|2|Juan|Fernandes|9/2/2018|Recife|5300|NaN|10600|
|512|7087|HL4379|Televisão|2|Breno|Britto|10/15/2018|Recife|2500|NaN|5000|
|513|7124|HL1918|iPhone|3|Maria|Costa|8/11/2018|Recife|5300|NaN|15900|
|514|7147|HL1918|iPhone|2|Beatriz|Almeida|8/26/2018|Recife|5300|NaN|10600|
|515|7172|HL1918|iPhone|4|Diogo|Ressurreição|1/25/2018|Recife|5300|NaN|21200|
|516|7179|HL1918|iPhone|3|Cláudio|Aragão|8/26/2018|Recife|5300|NaN|15900|
|517|7204|HL1918|iPhone|4|Lucas|Lacerda|5/16/2018|Recife|5300|NaN|21200|
|518|7209|HL8851|Notebook|3|Beatriz|Biase|1/9/2018|Recife|3500|NaN|10500|
|519|7213|HL4379|Televisão|4|Thales|Fanara|12/19/2018|Recife|2500|NaN|10000|
|520|7224|HL7348|SmartWatch|1|Yasmim|Verly|3/9/2018|Recife|1400|NaN|1400|
|521|7233|HL4379|Televisão|3|Livia|Cozendey|1/24/2018|Recife|2500|NaN|7500|
|522|7250|HL1918|iPhone|5|Lázaro|Villanova|11/4/2018|Recife|5300|NaN|26500|
|523|7253|HL2714|Tablet|5|Sthefeson|Pereira|10/29/2018|Recife|1600|NaN|8000|
|524|7259|HL1918|iPhone|3|Fernanda|Figueiredo|8/21/2018|Recife|5300|NaN|15900|
|525|7260|HL4379|Televisão|5|Jéssica|Stefanelli|5/10/2018|Recife|2500|NaN|12500|
|526|7264|HL1918|iPhone|5|Bruna|Brandao|6/16/2018|Recife|5300|NaN|26500|
|527|7282|HL1918|iPhone|4|Nina|Magalhães|8/10/2018|Recife|5300|NaN|21200|
|528|7285|HL1918|iPhone|2|Fernanda|Rubim|11/14/2018|Recife|5300|NaN|10600|
|529|7293|HL4379|Televisão|5|Ulisses|Filho|4/27/2018|Recife|2500|NaN|12500|
|530|7312|HL7348|SmartWatch|3|Gabriel|Silva|12/20/2018|Recife|1400|NaN|4200|
|531|7320|HL1148|Câmera|4|Daniel|Valente|9/24/2018|Recife|2100|NaN|8400|
|532|7449|HL2714|Tablet|4|Fabio|Boccaletti|3/6/2018|Recife|1600|NaN|6400|
|533|7461|HL1148|Câmera|5|Beatriz|Rodrigues|2/27/2018|Recife|2100|NaN|10500|
|534|7498|HL2714|Tablet|2|João|Fonseca|6/8/2018|Recife|1600|NaN|3200|
|535|7503|HL4379|Televisão|1|Mariane|Racy|12/21/2018|Recife|2500|NaN|2500|
|536|7513|HL9962|Android|4|Raíssa|Oliveira|12/23/2018|Recife|3400|NaN|13600|
|537|7518|HL4379|Televisão|3|Luiza|Cavalcanti|11/23/2018|Recife|2500|NaN|7500|
|538|7541|HL2714|Tablet|1|Mariane|Ferreira|3/29/2018|Recife|1600|NaN|1600|
|539|7547|HL1918|iPhone|1|Pedro|Ferrari|10/11/2018|Recife|5300|NaN|5300|
|540|7548|HL1918|iPhone|5|Antônio|Soares|4/12/2018|Recife|5300|NaN|26500|
|541|7550|HL4379|Televisão|4|Daniel|Alcoforado|8/9/2018|Recife|2500|NaN|10000|
|542|7559|HL4379|Televisão|2|Breno|Quinto|3/19/2018|Recife|2500|NaN|5000|
|543|7562|HL7348|SmartWatch|1|Igor|Azevedo|4/12/2018|Recife|1400|NaN|1400|
|544|7575|HL8851|Notebook|4|Nathalia|Ventura|7/18/2018|Recife|3500|NaN|14000|
|545|7576|HL1918|iPhone|1|Willian|Albino|7/4/2018|Recife|5300|NaN|5300|
|546|7584|HL2714|Tablet|1|Pedro|Cardoso|4/10/2018|Recife|1600|NaN|1600|
|547|7591|HL1918|iPhone|5|Danilo|Rubim|1/3/2018|Recife|5300|NaN|26500|
|548|7643|HL2714|Tablet|4|João|Fonseca|7/24/2018|Recife|1600|NaN|6400|
|549|7649|HL4379|Televisão|5|Guilherme|Castilho|3/19/2018|Recife|2500|NaN|12500|
|550|7691|HL1918|iPhone|1|Thales|Santos|4/16/2018|Recife|5300|NaN|5300|
|551|7693|HL2714|Tablet|3|Cláudio|Aragão|4/15/2018|Recife|1600|NaN|4800|
|552|7717|HL4379|Televisão|4|Thays|Castro|10/22/2018|Recife|2500|NaN|10000|
|553|7725|HL9962|Android|2|José|Carvalho|2/20/2018|Recife|3400|NaN|6800|
|554|7761|HL4379|Televisão|5|Guilherme|Rachide|6/24/2018|Recife|2500|NaN|12500|
|555|7780|HL4379|Televisão|1|Caio|Vianna|8/25/2018|Recife|2500|NaN|2500|
|556|7801|HL7348|SmartWatch|2|Yasser|Calbucci|3/2/2018|Recife|1400|NaN|2800|
|557|7815|HL4379|Televisão|3|Raphael|Machado|11/6/2018|Recife|2500|NaN|7500|
|558|7833|HL1918|iPhone|4|Amanda|Delgado|1/8/2018|Recife|5300|NaN|21200|
|559|7865|HL7348|SmartWatch|5|Bruna|Londero|5/12/2018|Recife|1400|NaN|7000|
|560|7902|HL4379|Televisão|1|Maria|Cardoso|7/3/2018|Recife|2500|NaN|2500|
|561|7922|HL2714|Tablet|2|Breno|Britto|2/8/2018|Recife|1600|NaN|3200|
|562|7936|HL4379|Televisão|3|Fillipe|Almeida|7/24/2018|Recife|2500|NaN|7500|
|563|7944|HL1918|iPhone|4|Luiza|Farias|3/22/2018|Recife|5300|NaN|21200|
|564|7946|HL1148|Câmera|4|Bruno|Oliveira|2/12/2018|Recife|2100|NaN|8400|
|565|8002|HL4379|Televisão|1|Marcelo|Guadagnino|6/19/2018|Recife|2500|NaN|2500|
|566|8005|HL1918|iPhone|3|Bernardo|Borges|6/20/2018|Recife|5300|NaN|15900|
|567|8019|HL8851|Notebook|3|Giovanna|Santos|4/16/2018|Recife|3500|NaN|10500|
|568|8020|HL8851|Notebook|3|Matheus|Tostes|3/21/2018|Recife|3500|NaN|10500|
|569|8022|HL7348|SmartWatch|4|Fernanda|Silva|7/20/2018|Recife|1400|NaN|5600|
|570|8031|HL1148|Câmera|4|Mayara|Soares|12/10/2018|Recife|2100|NaN|8400|
|571|8041|HL8851|Notebook|1|Philipe|Morete|1/16/2018|Recife|3500|NaN|3500|
|572|8060|HL8851|Notebook|1|Ana|Leite|12/11/2018|Recife|3500|NaN|3500|
|573|8066|HL1918|iPhone|3|Gustavo|Thome|1/28/2018|Recife|5300|NaN|15900|
|574|8084|HL2714|Tablet|3|Isabella|Santos|9/24/2018|Recife|1600|NaN|4800|
|575|8088|HL9962|Android|3|Bárbara|Cavalcante|10/11/2018|Recife|3400|NaN|10200|
|576|8103|HL4379|Televisão|1|Bruno|Mota|5/19/2018|Recife|2500|NaN|2500|
|577|8114|HL1918|iPhone|2|Douglas|Rodrigues|4/13/2018|Recife|5300|NaN|10600|
|578|8120|HL4379|Televisão|5|Caio|Silva|9/23/2018|Recife|2500|NaN|12500|
|579|8131|HL1918|iPhone|1|Jônatas|Tanaka|11/24/2018|Recife|5300|NaN|5300|
|580|8155|HL7348|SmartWatch|3|Anna|Maia|2/24/2018|Recife|1400|NaN|4200|
|581|8157|HL7348|SmartWatch|5|Pedro|Oliveira|8/6/2018|Recife|1400|NaN|7000|
|582|8162|HL1918|iPhone|3|Luíza|Goulart|6/12/2018|Recife|5300|NaN|15900|
|583|8175|HL2714|Tablet|3|Philipe|Morete|5/29/2018|Recife|1600|NaN|4800|
|584|8185|HL1918|iPhone|4|David|Vasconcelos|12/30/2018|Recife|5300|NaN|21200|
|585|8201|HL8851|Notebook|4|Isabela|Resende|6/26/2018|Recife|3500|NaN|14000|
|586|8207|HL1148|Câmera|5|Marcela|Gasperi|6/9/2018|Recife|2100|NaN|10500|
|587|8224|HL1918|iPhone|4|Sandy|Figueiredo|6/8/2018|Recife|5300|NaN|21200|
|588|8227|HL2714|Tablet|4|João|Guadagnino|1/23/2018|Recife|1600|NaN|6400|
|589|8229|HL1148|Câmera|5|Caio|Caldas|2/27/2018|Recife|2100|NaN|10500|
|590|8252|HL1918|iPhone|3|Michelle|Pereira|3/4/2018|Recife|5300|NaN|15900|
|591|8273|HL4379|Televisão|3|Renan|Nascimento|1/6/2018|Recife|2500|NaN|7500|
|592|8279|HL1918|iPhone|3|Gustavo|Aragão|8/31/2018|Recife|5300|NaN|15900|
|593|8310|HL8851|Notebook|3|Daniel|Ortiz|9/14/2018|Recife|3500|NaN|10500|
|594|8357|HL1918|iPhone|2|Lázaro|Nascimento|8/16/2018|Recife|5300|NaN|10600|
|595|8362|HL1918|iPhone|5|Joao|Pereira|7/10/2018|Recife|5300|NaN|26500|
|596|8385|HL7348|SmartWatch|2|Gustavo|Aragão|8/31/2018|Recife|1400|NaN|2800|
|597|8414|HL2714|Tablet|3|Gabriela|Cavalcanti|1/3/2018|Recife|1600|NaN|4800|
|598|8421|HL2714|Tablet|1|Eric|Júnior|7/22/2018|Recife|1600|NaN|1600|
|599|8422|HL1918|iPhone|3|Catarina|Teixeira|5/11/2018|Recife|5300|NaN|15900|
|600|8433|HL1148|Câmera|4|Luíza|Garcia|9/22/2018|Recife|2100|NaN|8400|
|601|8439|HL1918|iPhone|5|Dandara|Reis|3/10/2018|Recife|5300|NaN|26500|
|602|8464|HL1148|Câmera|5|Alvaro|Kranz|7/31/2018|Recife|2100|NaN|10500|
|603|8496|HL1918|iPhone|3|Kimberly|Sad|5/19/2018|Recife|5300|NaN|15900|
|604|8526|HL1918|iPhone|2|Thaís|Moura|4/4/2018|Recife|5300|NaN|10600|
|605|8527|HL4379|Televisão|3|Bernardo|Ribeiro|7/16/2018|Recife|2500|NaN|7500|
|606|8536|HL1148|Câmera|3|Bernardo|Ribeiro|4/29/2018|Recife|2100|NaN|6300|
|607|8539|HL7348|SmartWatch|1|Letícia|Araujo|5/19/2018|Recife|1400|NaN|1400|
|608|8547|HL8851|Notebook|3|Raíza|Lopes|5/8/2018|Recife|3500|NaN|10500|
|609|8552|HL7348|SmartWatch|1|Mônica|Rotolo|9/15/2018|Recife|1400|NaN|1400|
|610|8577|HL1918|iPhone|2|Mariana|Barrozo|6/10/2018|Recife|5300|NaN|10600|
|611|8601|HL1918|iPhone|1|Victor|Lira|5/5/2018|Recife|5300|NaN|5300|
|612|8602|HL2714|Tablet|4|João|Bach|6/4/2018|Recife|1600|NaN|6400|
|613|8605|HL8851|Notebook|5|Rafael|Ramos|9/18/2018|Recife|3500|NaN|17500|
|614|8607|HL7348|SmartWatch|2|Rafael|Portela|6/23/2018|Recife|1400|NaN|2800|
|615|8635|HL9962|Android|1|Carlos|Cardoso|10/31/2018|Recife|3400|NaN|3400|
|616|8654|HL8851|Notebook|2|Luiza|Procaci|3/17/2018|Recife|3500|NaN|7000|
|617|8661|HL7348|SmartWatch|4|Roger|Rosa|5/31/2018|Recife|1400|NaN|5600|
|618|8667|HL4379|Televisão|4|Marina|Mesquita|7/24/2018|Recife|2500|NaN|10000|
|619|8673|HL1918|iPhone|3|Giulia|Pessanha|11/20/2018|Recife|5300|NaN|15900|
|620|8692|HL7348|SmartWatch|5|Pedro|Bitencourt|7/28/2018|Recife|1400|NaN|7000|
|621|8723|HL8851|Notebook|1|Luana|Santana|7/28/2018|Recife|3500|NaN|3500|
|622|8724|HL4379|Televisão|2|Kim|Ferreira|7/19/2018|Recife|2500|NaN|5000|
|623|8725|HL2714|Tablet|3|Livia|Corrêa|5/10/2018|Recife|1600|NaN|4800|
|624|8745|HL1918|iPhone|2|Antonio|Bernhardt|7/6/2018|Recife|5300|NaN|10600|
|625|8747|HL9962|Android|2|Aline|Andrade|11/18/2018|Recife|3400|NaN|6800|
|626|8750|HL1918|iPhone|5|Patrick|Silva|8/9/2018|Recife|5300|NaN|26500|
|627|8754|HL2714|Tablet|3|Bruna|Ramos|10/11/2018|Recife|1600|NaN|4800|
|628|8778|HL1918|iPhone|5|Maria|Costa|10/31/2018|Recife|5300|NaN|26500|
|629|8788|HL4379|Televisão|1|Beatriz|Santos|9/13/2018|Recife|2500|NaN|2500|
|630|8789|HL1918|iPhone|4|Ruan|Lopes|6/8/2018|Recife|5300|NaN|21200|
|631|8797|HL2714|Tablet|3|Marina|Marins|11/18/2018|Recife|1600|NaN|4800|
|632|8806|HL4379|Televisão|1|Luiza|Farias|3/21/2018|Recife|2500|NaN|2500|
|633|8814|HL7348|SmartWatch|2|Juliana|Silva|6/21/2018|Recife|1400|NaN|2800|
|634|8852|HL4379|Televisão|1|Lázaro|Villanova|9/25/2018|Recife|2500|NaN|2500|
|635|8874|HL4379|Televisão|4|Aline|Morais|7/29/2018|Recife|2500|NaN|10000|
|636|8877|HL8851|Notebook|3|Lenon|Fernandes|7/20/2018|Recife|3500|NaN|10500|
|637|8888|HL4379|Televisão|4|Marianna|Pestana|4/23/2018|Recife|2500|NaN|10000|
|638|8894|HL7348|SmartWatch|2|Chan|Santos|5/15/2018|Recife|1400|NaN|2800|
|639|8918|HL1148|Câmera|4|Leandro|Rodrigues|6/2/2018|Recife|2100|NaN|8400|
|640|8941|HL4379|Televisão|3|Jônatas|Soares|10/9/2018|Recife|2500|NaN|7500|
|641|8962|HL7348|SmartWatch|5|Joyce|Souza|3/17/2018|Recife|1400|NaN|7000|
|642|8971|HL2714|Tablet|4|Lucas|Machado|6/2/2018|Recife|1600|NaN|6400|
|643|8973|HL9962|Android|3|Beatriz|Li|1/7/2018|Recife|3400|NaN|10200|
|644|8985|HL4379|Televisão|4|Ana|Júnior|12/3/2018|Recife|2500|NaN|10000|
|645|9020|HL1918|iPhone|1|Pedro|Lyra|11/25/2018|Recife|5300|NaN|5300|
|646|9052|HL1918|iPhone|3|João|Abraçado|6/10/2018|Recife|5300|NaN|15900|
|647|9069|HL7348|SmartWatch|4|Marcelo|Guadagnino|7/4/2018|Recife|1400|NaN|5600|
|648|9083|HL1918|iPhone|2|Giovanna|Santos|1/4/2018|Recife|5300|NaN|10600|
|649|9085|HL8851|Notebook|2|Gabrielle|Viríssimo|3/24/2018|Recife|3500|NaN|7000|
|650|9099|HL9962|Android|5|Jorge|Carvalho|9/8/2018|Recife|3400|NaN|17000|
|651|9101|HL4379|Televisão|4|Danilo|Rubim|3/23/2018|Recife|2500|NaN|10000|
|652|9134|HL4379|Televisão|3|Beatriz|Li|5/10/2018|Recife|2500|NaN|7500|
|653|9137|HL1918|iPhone|4|Rafael|Ramos|2/4/2018|Recife|5300|NaN|21200|
|654|9152|HL2714|Tablet|5|Stefan|Nunes|10/22/2018|Recife|1600|NaN|8000|
|655|9159|HL1918|iPhone|1|Raul|Junqueira|1/27/2018|Recife|5300|NaN|5300|
|656|9182|HL1918|iPhone|3|David|Vasconcelos|9/9/2018|Recife|5300|NaN|15900|
|657|9189|HL8851|Notebook|5|Deysiane|Bach|1/29/2018|Recife|3500|NaN|17500|
|658|9200|HL1918|iPhone|3|Rafaela|Rodrigues|1/2/2018|Recife|5300|NaN|15900|
|659|9207|HL1148|Câmera|2|Patrícia|Fernandes|1/20/2018|Recife|2100|NaN|4200|
|660|9220|HL8851|Notebook|2|Thaís|Pereira|4/19/2018|Recife|3500|NaN|7000|
|661|9221|HL4379|Televisão|5|Matheus|Moraes|8/7/2018|Recife|2500|NaN|12500|
|662|9246|HL4379|Televisão|2|Hércules|Moreira|9/16/2018|Recife|2500|NaN|5000|
|663|9251|HL1148|Câmera|1|João|Matheus|6/1/2018|Recife|2100|NaN|2100|
|664|9254|HL7348|SmartWatch|1|Gabriel|Almeida|2/23/2018|Recife|1400|NaN|1400|
|665|9259|HL9962|Android|4|Fernanda|Junior|11/7/2018|Recife|3400|NaN|13600|
|666|9267|HL2714|Tablet|4|Gabriel|Pereira|12/5/2018|Recife|1600|NaN|6400|
|667|9269|HL4379|Televisão|5|Dykson|Silva|2/15/2018|Recife|2500|NaN|12500|
|668|9286|HL7348|SmartWatch|4|Marina|Correa|6/11/2018|Recife|1400|NaN|5600|
|669|9293|HL7348|SmartWatch|4|Bianca|Allevato|3/23/2018|Recife|1400|NaN|5600|
|670|9295|HL2714|Tablet|5|Kimberly|Sad|6/8/2018|Recife|1600|NaN|8000|
|671|9308|HL4379|Televisão|4|Marina|Mesquita|2/2/2018|Recife|2500|NaN|10000|
|672|9322|HL9962|Android|3|Gabrielle|Silva|7/5/2018|Recife|3400|NaN|10200|
|673|9327|HL2714|Tablet|5|Priscila|Carvalho|3/8/2018|Recife|1600|NaN|8000|
|674|9354|HL1918|iPhone|1|Carolina|Santos|2/18/2018|Recife|5300|NaN|5300|
|675|9361|HL1918|iPhone|2|Pedro|Rodrigues|5/29/2018|Recife|5300|NaN|10600|
|676|9364|HL1148|Câmera|1|Mariana|Baptista|8/21/2018|Recife|2100|NaN|2100|
|677|9394|HL1918|iPhone|3|Rebeca|Manhães|7/9/2018|Recife|5300|NaN|15900|
|678|9438|HL1918|iPhone|4|Andre|Nóbrega|1/23/2018|Recife|5300|NaN|21200|
|679|9440|HL1918|iPhone|5|Ana|Felippe|9/27/2018|Recife|5300|NaN|26500|
|680|9454|HL4379|Televisão|2|Cícero|Lima|11/10/2018|Recife|2500|NaN|5000|
|681|9455|HL1148|Câmera|5|Camilla|Guimarães|1/18/2018|Recife|2100|NaN|10500|
|682|9462|HL8851|Notebook|2|Gustavo|Accardo|2/28/2018|Recife|3500|NaN|7000|
|683|9469|HL7348|SmartWatch|5|Andressa|Nóbrega|3/28/2018|Recife|1400|NaN|7000|
|684|9475|HL1918|iPhone|5|Anderson|Barreto|8/11/2018|Recife|5300|NaN|26500|
|685|9493|HL1148|Câmera|5|Jonatas|Passos|7/27/2018|Recife|2100|NaN|10500|
|686|9495|HL1918|iPhone|2|Carlos|Barbosa|8/22/2018|Recife|5300|NaN|10600|
|687|9502|HL2714|Tablet|2|Bruno|Oliveira|6/27/2018|Recife|1600|NaN|3200|
|688|9512|HL4379|Televisão|3|Victor|Corrêa|5/13/2018|Recife|2500|NaN|7500|
|689|9513|HL1148|Câmera|3|Julia|Leig|4/12/2018|Recife|2100|NaN|6300|
|690|9516|HL7348|SmartWatch|1|Beatriz|Rocha|3/21/2018|Recife|1400|NaN|1400|
|691|9525|HL4379|Televisão|3|Marianna|Pestana|3/21/2018|Recife|2500|NaN|7500|
|692|9534|HL4379|Televisão|2|João|Silva|2/21/2018|Recife|2500|NaN|5000|
|693|9543|HL1918|iPhone|3|Camille|Silva|4/15/2018|Recife|5300|NaN|15900|
|694|9580|HL1148|Câmera|1|Luíza|Garcia|10/15/2018|Recife|2100|NaN|2100|
|695|9588|HL7348|SmartWatch|4|Juan|Barbosa|2/12/2018|Recife|1400|NaN|5600|
|696|9589|HL7348|SmartWatch|1|Pedro|Buraco|11/19/2018|Recife|1400|NaN|1400|
|697|9590|HL1148|Câmera|4|Henrique|Villanova|10/28/2018|Recife|2100|NaN|8400|
|698|9620|HL4379|Televisão|2|Luísa|Fonseca|12/20/2018|Recife|2500|NaN|5000|
|699|9637|HL1918|iPhone|4|Rafael|Rocha|3/29/2018|Recife|5300|NaN|21200|
|700|9652|HL8851|Notebook|5|Joyce|Souza|11/24/2018|Recife|3500|NaN|17500|
|701|9665|HL1148|Câmera|3|Alberto|Silveira|1/18/2018|Recife|2100|NaN|6300|
|702|9673|HL4379|Televisão|2|João|Tabet|5/22/2018|Recife|2500|NaN|5000|
|703|9676|HL1918|iPhone|1|Camilla|Cardeman|4/20/2018|Recife|5300|NaN|5300|
|704|9686|HL1918|iPhone|4|João|Silva|1/27/2018|Recife|5300|NaN|21200|
|705|9773|HL1918|iPhone|3|Giselia|Thiele|9/18/2018|Recife|5300|NaN|15900|
|706|9781|HL4379|Televisão|2|João|Siqueira|6/16/2018|Recife|2500|NaN|5000|
|707|9784|HL1918|iPhone|4|Camilla|Guimarães|1/29/2018|Recife|5300|NaN|21200|
|708|9802|HL1918|iPhone|4|João|Menezes|8/17/2018|Recife|5300|NaN|21200|
|709|9805|HL4379|Televisão|3|Eric|Carvalho|4/24/2018|Recife|2500|NaN|7500|
|710|9821|HL2714|Tablet|2|Priscila|Suzano|5/11/2018|Recife|1600|NaN|3200|
|711|9832|HL2714|Tablet|2|Stephanie|Oliveira|7/19/2018|Recife|1600|NaN|3200|
|712|9853|HL4379|Televisão|1|Célio|Xavier|3/1/2018|Recife|2500|NaN|2500|
|713|9860|HL8851|Notebook|5|Matheus|Delgado|8/9/2018|Recife|3500|NaN|17500|
|714|9865|HL4379|Televisão|2|Clara|Silveira|12/2/2018|Recife|2500|NaN|5000|
|715|9874|HL2714|Tablet|4|Bianca|Piero|2/25/2018|Recife|1600|NaN|6400|
|716|9875|HL7348|SmartWatch|3|Rubens|Netto|11/6/2018|Recife|1400|NaN|4200|
|717|9888|HL8851|Notebook|2|Giovanna|Santos|1/3/2018|Recife|3500|NaN|7000|
|718|9920|HL1148|Câmera|4|Arthur|Souza|12/8/2018|Recife|2100|NaN|8400|
|719|9930|HL1918|iPhone|3|Fillipe|Almeida|10/9/2018|Recife|5300|NaN|15900|
|720|9938|HL4379|Televisão|3|Fernanda|Silva|12/18/2018|Recife|2500|NaN|7500|
|721|9941|HL2714|Tablet|5|Alvaro|Kranz|11/21/2018|Recife|1600|NaN|8000|
|722|9969|HL1918|iPhone|4|Itai|Puntel|11/6/2018|Recife|5300|NaN|21200|
|723|9986|HL9962|Android|4|Julia|Leite|4/8/2018|Recife|3400|NaN|13600|
|724|9992|HL1918|iPhone|1|Marina|Cormack|12/31/2018|Recife|5300|NaN|5300|
|0|5|HL1918|iPhone|4|Sarah|Souza|2/14/2018|São Paulo|5300|NaN|21200|
|1|6|HL7348|SmartWatch|3|Alexandre|Rodriguez|5/20/2018|São Paulo|1400|NaN|4200|
|2|9|HL1148|Câmera|3|Camille|Silva|3/26/2018|São Paulo|2100|NaN|6300|
|3|10|HL1918|iPhone|3|Alon|Palmeira|11/6/2018|São Paulo|5300|NaN|15900|
|4|18|HL8851|Notebook|4|Leandro|Rodrigues|8/6/2018|São Paulo|3500|NaN|14000|
|5|20|HL7348|SmartWatch|2|Henrique|Silva|8/5/2018|São Paulo|1400|NaN|2800|
|6|23|HL8851|Notebook|5|Fillipe|Almeida|12/6/2018|São Paulo|3500|NaN|17500|
|7|30|HL1148|Câmera|4|Gabriel|Puntel|9/27/2018|São Paulo|2100|NaN|8400|
|8|31|HL1918|iPhone|5|Clarissa|Santos|12/23/2018|São Paulo|5300|NaN|26500|
|9|32|HL1918|iPhone|2|Danilo|Rubim|11/20/2018|São Paulo|5300|NaN|10600|
|10|33|HL7348|SmartWatch|1|Nathan|Morelli|1/2/2018|São Paulo|1400|NaN|1400|
|11|36|HL7348|SmartWatch|4|Beatriz|Li|12/13/2018|São Paulo|1400|NaN|5600|
|12|37|HL2714|Tablet|1|Sarah|Souza|1/3/2018|São Paulo|1600|NaN|1600|
|13|38|HL8851|Notebook|5|João|Aires|12/24/2018|São Paulo|3500|NaN|17500|
|14|47|HL4379|Televisão|2|Guilherme|Merotto|11/17/2018|São Paulo|2500|NaN|5000|
|15|48|HL1918|iPhone|4|Myllena|Carneiro|1/7/2018|São Paulo|5300|NaN|21200|
|16|56|HL1148|Câmera|3|Kim|Ferreira|3/19/2018|São Paulo|2100|NaN|6300|
|17|57|HL1918|iPhone|5|Ana|Silva|5/25/2018|São Paulo|5300|NaN|26500|
|18|62|HL1148|Câmera|3|Adrielle|Vieira|11/25/2018|São Paulo|2100|NaN|6300|
|19|69|HL4379|Televisão|2|Carolina|Figueiredo|2/17/2018|São Paulo|2500|NaN|5000|
|20|75|HL9962|Android|3|Marcelo|Guadagnino|12/27/2018|São Paulo|3400|NaN|10200|
|21|80|HL2714|Tablet|2|Deysiane|Medronho|10/12/2018|São Paulo|1600|NaN|3200|
|22|81|HL4379|Televisão|4|Jackson|Derossi|6/3/2018|São Paulo|2500|NaN|10000|
|23|86|HL1148|Câmera|2|Victor|Lira|7/8/2018|São Paulo|2100|NaN|4200|
|24|87|HL1918|iPhone|1|João|Abraçado|4/30/2018|São Paulo|5300|NaN|5300|
|25|92|HL1148|Câmera|4|Matheus|Gomes|1/18/2018|São Paulo|2100|NaN|8400|
|26|96|HL1918|iPhone|4|Lucas|Fontoura|5/4/2018|São Paulo|5300|NaN|21200|
|27|106|HL1148|Câmera|2|Mariana|Barrozo|8/5/2018|São Paulo|2100|NaN|4200|
|28|111|HL4379|Televisão|4|Maurício|Dias|9/10/2018|São Paulo|2500|NaN|10000|
|29|118|HL8851|Notebook|1|Gustavo|Gomes|7/6/2018|São Paulo|3500|NaN|3500|
|30|125|HL9962|Android|5|Marina|Mesquita|2/16/2018|São Paulo|3400|NaN|17000|
|31|126|HL1148|Câmera|3|Ana|Michetti|5/11/2018|São Paulo|2100|NaN|6300|
|32|134|HL9962|Android|1|Rafael|Portela|3/23/2018|São Paulo|3400|NaN|3400|
|33|137|HL2714|Tablet|3|Bianca|Ferezin|1/25/2018|São Paulo|1600|NaN|4800|
|34|143|HL4379|Televisão|5|Fernanda|Junior|7/8/2018|São Paulo|2500|NaN|12500|
|35|145|HL9962|Android|3|Rodrigo|Alves|8/21/2018|São Paulo|3400|NaN|10200|
|36|148|HL8851|Notebook|4|Carla|Zakhm|1/25/2018|São Paulo|3500|NaN|14000|
|37|154|HL8851|Notebook|1|João|Monteiro|2/2/2018|São Paulo|3500|NaN|3500|
|38|156|HL2714|Tablet|1|Sthefeson|Barroso|3/9/2018|São Paulo|1600|NaN|1600|
|39|161|HL1148|Câmera|2|Patrícia|Amaral|6/1/2018|São Paulo|2100|NaN|4200|
|40|162|HL1918|iPhone|3|Diego|Rodrigues|2/21/2018|São Paulo|5300|NaN|15900|
|41|170|HL2714|Tablet|4|Felipe|Mendonça|12/20/2018|São Paulo|1600|NaN|6400|
|42|173|HL9962|Android|2|Samara|Pinto|12/23/2018|São Paulo|3400|NaN|6800|
|43|176|HL1918|iPhone|1|Paloma|Sperandei|4/9/2018|São Paulo|5300|NaN|5300|
|44|179|HL4379|Televisão|4|Dykson|Silva|12/5/2018|São Paulo|2500|NaN|10000|
|45|182|HL2714|Tablet|4|Priscila|Carvalho|2/21/2018|São Paulo|1600|NaN|6400|
|46|184|HL4379|Televisão|4|Daniela|Rosa|4/25/2018|São Paulo|2500|NaN|10000|
|47|186|HL1918|iPhone|4|Roberto|Tiradentes|10/17/2018|São Paulo|5300|NaN|21200|
|48|191|HL1918|iPhone|1|Lucas|Fontoura|12/1/2018|São Paulo|5300|NaN|5300|
|49|195|HL1918|iPhone|4|Ana|Monte|7/24/2018|São Paulo|5300|NaN|21200|
|50|198|HL1148|Câmera|4|Juliana|Silva|8/8/2018|São Paulo|2100|NaN|8400|
|51|203|HL4379|Televisão|1|Pedro|Delgado|3/23/2018|São Paulo|2500|NaN|2500|
|52|204|HL4379|Televisão|1|Vanessa|Bach|7/24/2018|São Paulo|2500|NaN|2500|
|53|206|HL1918|iPhone|4|Luis|Souza|5/9/2018|São Paulo|5300|NaN|21200|
|54|213|HL4379|Televisão|3|Khaio|Mesquita|1/15/2018|São Paulo|2500|NaN|7500|
|55|221|HL2714|Tablet|2|Diogo|Ressurreição|4/1/2018|São Paulo|1600|NaN|3200|
|56|223|HL2714|Tablet|5|Lucas|Lima|10/9/2018|São Paulo|1600|NaN|8000|
|57|241|HL1918|iPhone|3|José|Vieira|8/9/2018|São Paulo|5300|NaN|15900|
|58|264|HL2714|Tablet|2|Marina|Marins|7/23/2018|São Paulo|1600|NaN|3200|
|59|268|HL1918|iPhone|1|Tiago|Pereira|11/23/2018|São Paulo|5300|NaN|5300|
|60|273|HL1918|iPhone|4|Larissa|Vasconcellos|5/3/2018|São Paulo|5300|NaN|21200|
|61|275|HL9962|Android|2|Amanda|Delgado|5/3/2018|São Paulo|3400|NaN|6800|
|62|276|HL8851|Notebook|5|Arthur|Rocha|9/18/2018|São Paulo|3500|NaN|17500|
|63|280|HL1918|iPhone|2|Luana|Santos|11/14/2018|São Paulo|5300|NaN|10600|
|64|286|HL1918|iPhone|2|Tayla|Lima|3/12/2018|São Paulo|5300|NaN|10600|
|65|288|HL4379|Televisão|1|Lucas|Junior|10/17/2018|São Paulo|2500|NaN|2500|
|66|298|HL1918|iPhone|1|Giselia|Thiele|12/4/2018|São Paulo|5300|NaN|5300|
|67|299|HL1918|iPhone|3|Natalia|Guedes|2/13/2018|São Paulo|5300|NaN|15900|
|68|301|HL1918|iPhone|1|Dykson|Silva|3/9/2018|São Paulo|5300|NaN|5300|
|69|303|HL8851|Notebook|1|Lucas|Freire|3/27/2018|São Paulo|3500|NaN|3500|
|70|304|HL9962|Android|1|João|Matheus|5/19/2018|São Paulo|3400|NaN|3400|
|71|305|HL2714|Tablet|1|Andressa|Rotsztejn|8/25/2018|São Paulo|1600|NaN|1600|
|72|307|HL7348|SmartWatch|2|Juliana|Silva|5/17/2018|São Paulo|1400|NaN|2800|
|73|309|HL4379|Televisão|1|Cézar|Santos|7/27/2018|São Paulo|2500|NaN|2500|
|74|314|HL1918|iPhone|5|Bruno|Barcessat|10/28/2018|São Paulo|5300|NaN|26500|
|75|315|HL4379|Televisão|5|Luiza|Cabral|12/3/2018|São Paulo|2500|NaN|12500|
|76|317|HL2714|Tablet|3|José|Fonseca|10/6/2018|São Paulo|1600|NaN|4800|
|77|318|HL4379|Televisão|2|Morgana|Correa|9/4/2018|São Paulo|2500|NaN|5000|
|78|330|HL1918|iPhone|4|Lucas|Baptista|4/11/2018|São Paulo|5300|NaN|21200|
|79|331|HL1918|iPhone|1|Bruna|Franco|12/2/2018|São Paulo|5300|NaN|5300|
|80|332|HL8851|Notebook|4|Daniel|Felippe|9/15/2018|São Paulo|3500|NaN|14000|
|81|339|HL1918|iPhone|5|Bianca|Paz|1/2/2018|São Paulo|5300|NaN|26500|
|82|342|HL1918|iPhone|5|Tadeu|Sousa|5/28/2018|São Paulo|5300|NaN|26500|
|83|343|HL7348|SmartWatch|1|Vanessa|Bach|5/12/2018|São Paulo|1400|NaN|1400|
|84|344|HL7348|SmartWatch|1|Adrielle|Gabriel|2/10/2018|São Paulo|1400|NaN|1400|
|85|345|HL4379|Televisão|3|Marina|Miranda|10/16/2018|São Paulo|2500|NaN|7500|
|86|349|HL2714|Tablet|3|Laís|Oliveira|12/17/2018|São Paulo|1600|NaN|4800|
|87|359|HL1148|Câmera|2|Henrique|Oliveira|9/7/2018|São Paulo|2100|NaN|4200|
|88|368|HL2714|Tablet|2|Arthur|Rocha|2/17/2018|São Paulo|1600|NaN|3200|
|89|370|HL4379|Televisão|5|Adriane|Chagas|1/20/2018|São Paulo|2500|NaN|12500|
|90|380|HL8851|Notebook|2|Raíza|Lopes|6/21/2018|São Paulo|3500|NaN|7000|
|91|381|HL1918|iPhone|1|Renan|Cunha|1/13/2018|São Paulo|5300|NaN|5300|
|92|393|HL2714|Tablet|5|Lucas|Costa|4/8/2018|São Paulo|1600|NaN|8000|
|93|396|HL1918|iPhone|5|Thainá|Binello|9/22/2018|São Paulo|5300|NaN|26500|
|94|401|HL7348|SmartWatch|2|Maria|Cardoso|6/17/2018|São Paulo|1400|NaN|2800|
|95|406|HL1148|Câmera|2|Hiaiune|Valim|1/30/2018|São Paulo|2100|NaN|4200|
|96|408|HL4379|Televisão|2|Gabriel|Rubim|5/3/2018|São Paulo|2500|NaN|5000|
|97|411|HL4379|Televisão|4|Rebeca|Taylor|5/26/2018|São Paulo|2500|NaN|10000|
|98|417|HL1918|iPhone|2|Joyce|Medina|1/13/2018|São Paulo|5300|NaN|10600|
|99|422|HL1918|iPhone|3|Daniel|Valente|12/28/2018|São Paulo|5300|NaN|15900|
|100|425|HL4379|Televisão|2|Bruno|Mota|1/15/2018|São Paulo|2500|NaN|5000|
|101|427|HL1918|iPhone|4|Carolina|Bernardes|7/7/2018|São Paulo|5300|NaN|21200|
|102|431|HL9962|Android|3|Raphael|Coelho|3/13/2018|São Paulo|3400|NaN|10200|
|103|432|HL1918|iPhone|5|Guido|Monteiro|12/28/2018|São Paulo|5300|NaN|26500|
|104|433|HL1148|Câmera|1|Milena|Alcoforado|3/17/2018|São Paulo|2100|NaN|2100|
|105|455|HL4379|Televisão|4|Letícia|Leal|11/14/2018|São Paulo|2500|NaN|10000|
|106|458|HL8851|Notebook|5|Julia|Leig|4/19/2018|São Paulo|3500|NaN|17500|
|107|462|HL1918|iPhone|4|Gabriela|Aliani|7/24/2018|São Paulo|5300|NaN|21200|
|108|467|HL1918|iPhone|4|Douglas|Rodrigues|5/18/2018|São Paulo|5300|NaN|21200|
|109|471|HL2714|Tablet|2|Bruna|Ramos|8/22/2018|São Paulo|1600|NaN|3200|
|110|472|HL1148|Câmera|3|Marcos|Nucci|5/7/2018|São Paulo|2100|NaN|6300|
|111|475|HL1918|iPhone|5|Henrique|Lencastre|11/23/2018|São Paulo|5300|NaN|26500|
|112|477|HL9962|Android|2|Raphael|Kurtz|10/3/2018|São Paulo|3400|NaN|6800|
|113|484|HL1918|iPhone|3|Paula|Carneiro|3/18/2018|São Paulo|5300|NaN|15900|
|114|488|HL1918|iPhone|5|Bianca|Paz|12/26/2018|São Paulo|5300|NaN|26500|
|115|489|HL1148|Câmera|5|Brenno|Santos|12/1/2018|São Paulo|2100|NaN|10500|
|116|497|HL7348|SmartWatch|2|Gustavo|Accardo|6/4/2018|São Paulo|1400|NaN|2800|
|117|500|HL4379|Televisão|5|Thayane|Resende|12/12/2018|São Paulo|2500|NaN|12500|
|118|501|HL7348|SmartWatch|5|Mariana|Barrozo|6/5/2018|São Paulo|1400|NaN|7000|
|119|515|HL4379|Televisão|3|Luiza|Ribeiro|3/25/2018|São Paulo|2500|NaN|7500|
|120|519|HL9962|Android|2|Ana|Soledade|2/3/2018|São Paulo|3400|NaN|6800|
|121|532|HL8851|Notebook|4|Juliana|Correa|7/25/2018|São Paulo|3500|NaN|14000|
|122|534|HL7348|SmartWatch|5|Caio|Silva|4/11/2018|São Paulo|1400|NaN|7000|
|123|543|HL1918|iPhone|5|Gabriel|Assis|6/11/2018|São Paulo|5300|NaN|26500|
|124|546|HL1918|iPhone|1|Thaís|Ribeiro|8/22/2018|São Paulo|5300|NaN|5300|
|125|551|HL9962|Android|4|Manuela|Ferreira|1/7/2018|São Paulo|3400|NaN|13600|
|126|552|HL8851|Notebook|1|Thiago|Veloso|9/15/2018|São Paulo|3500|NaN|3500|
|127|557|HL9962|Android|3|Thayna|Martins|2/4/2018|São Paulo|3400|NaN|10200|
|128|564|HL8851|Notebook|1|Raphael|Guedes|5/26/2018|São Paulo|3500|NaN|3500|
|129|565|HL1918|iPhone|3|Helvio|Pedrosa|7/14/2018|São Paulo|5300|NaN|15900|
|130|573|HL8851|Notebook|5|Julia|Penteado|2/19/2018|São Paulo|3500|NaN|17500|
|131|580|HL4379|Televisão|2|Natali|Rangel|8/31/2018|São Paulo|2500|NaN|5000|
|132|581|HL2714|Tablet|1|Roberto|Nogueira|10/14/2018|São Paulo|1600|NaN|1600|
|133|586|HL9962|Android|5|Victor|Magalhães|5/31/2018|São Paulo|3400|NaN|17000|
|134|589|HL1918|iPhone|3|Ananda|Dias|2/10/2018|São Paulo|5300|NaN|15900|
|135|595|HL9962|Android|2|Khaio|Mesquita|5/26/2018|São Paulo|3400|NaN|6800|
|136|600|HL8851|Notebook|3|Yasmim|Bittencourt|1/4/2018|São Paulo|3500|NaN|10500|
|137|602|HL1918|iPhone|4|Izabel|Lopes|8/13/2018|São Paulo|5300|NaN|21200|
|138|606|HL2714|Tablet|4|Caio|Cardoso|9/29/2018|São Paulo|1600|NaN|6400|
|139|620|HL4379|Televisão|4|Carolina|Rocha|6/26/2018|São Paulo|2500|NaN|10000|
|140|622|HL1918|iPhone|2|Fernanda|Rubim|12/6/2018|São Paulo|5300|NaN|10600|
|141|625|HL8851|Notebook|5|Kim|Ferreira|1/18/2018|São Paulo|3500|NaN|17500|
|142|639|HL1918|iPhone|1|Mateus|Polastri|10/26/2018|São Paulo|5300|NaN|5300|
|143|640|HL2714|Tablet|3|Débora|Lopes|2/10/2018|São Paulo|1600|NaN|4800|
|144|641|HL1918|iPhone|4|Leandro|Melo|12/2/2018|São Paulo|5300|NaN|21200|
|145|643|HL1148|Câmera|1|Livia|Codeceira|9/28/2018|São Paulo|2100|NaN|2100|
|146|644|HL1148|Câmera|2|Gustavo|Guimarães|12/9/2018|São Paulo|2100|NaN|4200|
|147|656|HL1918|iPhone|3|Mariana|Barrozo|12/22/2018|São Paulo|5300|NaN|15900|
|148|658|HL1918|iPhone|2|Natalia|Andrade|12/24/2018|São Paulo|5300|NaN|10600|
|149|665|HL8851|Notebook|5|Luíza|Garcia|7/23/2018|São Paulo|3500|NaN|17500|
|150|682|HL1918|iPhone|1|Larissa|Florim|3/2/2018|São Paulo|5300|NaN|5300|
|151|689|HL7348|SmartWatch|5|Julia|Leite|9/21/2018|São Paulo|1400|NaN|7000|
|152|693|HL1918|iPhone|2|Debora|Silva|6/29/2018|São Paulo|5300|NaN|10600|
|153|698|HL4379|Televisão|4|Daniela|Andrada|9/20/2018|São Paulo|2500|NaN|10000|
|154|702|HL4379|Televisão|4|Priscila|Carvalho|10/29/2018|São Paulo|2500|NaN|10000|
|155|703|HL2714|Tablet|1|Daniel|Valente|5/25/2018|São Paulo|1600|NaN|1600|
|156|712|HL1918|iPhone|4|Deysiane|Bach|2/2/2018|São Paulo|5300|NaN|21200|
|157|721|HL2714|Tablet|1|Roberto|Tiradentes|8/7/2018|São Paulo|1600|NaN|1600|
|158|724|HL1918|iPhone|3|Julie|Ferreira|5/8/2018|São Paulo|5300|NaN|15900|
|159|726|HL1918|iPhone|1|Clara|Bruno|4/27/2018|São Paulo|5300|NaN|5300|
|160|727|HL1918|iPhone|5|Guilherme|Lima|10/8/2018|São Paulo|5300|NaN|26500|
|161|732|HL8851|Notebook|3|Isabella|Santos|7/23/2018|São Paulo|3500|NaN|10500|
|162|736|HL4379|Televisão|1|Viviane|Cunha|12/27/2018|São Paulo|2500|NaN|2500|
|163|737|HL7348|SmartWatch|1|Bárbara|Cavalcante|7/27/2018|São Paulo|1400|NaN|1400|
|164|740|HL4379|Televisão|5|Camilla|Cardeman|6/6/2018|São Paulo|2500|NaN|12500|
|165|753|HL8851|Notebook|4|Joao|Silva|4/25/2018|São Paulo|3500|NaN|14000|
|166|779|HL4379|Televisão|3|Henrique|Silva|1/18/2018|São Paulo|2500|NaN|7500|
|167|784|HL1918|iPhone|5|Luiz|Mendonça|8/27/2018|São Paulo|5300|NaN|26500|
|168|785|HL2714|Tablet|3|Breno|Britto|11/27/2018|São Paulo|1600|NaN|4800|
|169|790|HL4379|Televisão|4|Arthur|Souza|8/27/2018|São Paulo|2500|NaN|10000|
|170|794|HL1148|Câmera|4|Vitor|Campos|1/14/2018|São Paulo|2100|NaN|8400|
|171|796|HL8851|Notebook|1|Thaís|Ribeiro|4/14/2018|São Paulo|3500|NaN|3500|
|172|803|HL1148|Câmera|3|Matheus|Tostes|9/26/2018|São Paulo|2100|NaN|6300|
|173|818|HL4379|Televisão|5|Gabriel|Pereira|5/11/2018|São Paulo|2500|NaN|12500|
|174|822|HL9962|Android|2|João|Rodrigues|6/25/2018|São Paulo|3400|NaN|6800|
|175|827|HL7348|SmartWatch|5|Tadeu|Sousa|2/11/2018|São Paulo|1400|NaN|7000|
|176|828|HL1918|iPhone|3|Breno|Godoy|3/4/2018|São Paulo|5300|NaN|15900|
|177|831|HL1918|iPhone|3|Thomáz|Vannier|4/1/2018|São Paulo|5300|NaN|15900|
|178|837|HL4379|Televisão|1|Thomáz|Bôas|11/4/2018|São Paulo|2500|NaN|2500|
|179|844|HL9962|Android|3|Rachel|Silva|1/29/2018|São Paulo|3400|NaN|10200|
|180|848|HL1918|iPhone|1|Camilla|Cardeman|12/30/2018|São Paulo|5300|NaN|5300|
|181|853|HL1918|iPhone|3|Gabriel|Soares|11/13/2018|São Paulo|5300|NaN|15900|
|182|858|HL1148|Câmera|5|Ana|Monte|11/20/2018|São Paulo|2100|NaN|10500|
|183|868|HL1148|Câmera|5|Bruno|Oliveira|4/29/2018|São Paulo|2100|NaN|10500|
|184|869|HL7348|SmartWatch|1|Amanda|Gontijo|6/7/2018|São Paulo|1400|NaN|1400|
|185|875|HL1918|iPhone|5|André|Alves|5/3/2018|São Paulo|5300|NaN|26500|
|186|878|HL7348|SmartWatch|4|Mariana|Barrozo|10/14/2018|São Paulo|1400|NaN|5600|
|187|880|HL1148|Câmera|1|Douglas|Rodrigues|5/25/2018|São Paulo|2100|NaN|2100|
|188|882|HL7348|SmartWatch|5|Lívia|Tanaka|2/12/2018|São Paulo|1400|NaN|7000|
|189|885|HL4379|Televisão|4|Marcela|Gasperi|3/28/2018|São Paulo|2500|NaN|10000|
|190|886|HL4379|Televisão|3|Daniel|Nauenberg|4/15/2018|São Paulo|2500|NaN|7500|
|191|894|HL1918|iPhone|3|Guilherme|Jordao|3/18/2018|São Paulo|5300|NaN|15900|
|192|899|HL2714|Tablet|1|João|Costa|12/10/2018|São Paulo|1600|NaN|1600|
|193|900|HL1918|iPhone|3|Eduardo|Soares|7/10/2018|São Paulo|5300|NaN|15900|
|194|902|HL9962|Android|5|Thomáz|Bôas|4/22/2018|São Paulo|3400|NaN|17000|
|195|903|HL7348|SmartWatch|3|Luana|Santana|3/5/2018|São Paulo|1400|NaN|4200|
|196|908|HL1148|Câmera|1|Lucas|Lacerda|12/11/2018|São Paulo|2100|NaN|2100|
|197|912|HL8851|Notebook|2|Antonio|Manhães|9/15/2018|São Paulo|3500|NaN|7000|
|198|922|HL1148|Câmera|3|Rebeca|Manhães|12/28/2018|São Paulo|2100|NaN|6300|
|199|923|HL1148|Câmera|2|Matheus|Tostes|5/22/2018|São Paulo|2100|NaN|4200|
|200|925|HL9962|Android|1|Raphael|Ferman|1/10/2018|São Paulo|3400|NaN|3400|
|201|930|HL1148|Câmera|2|Jéssica|Stefanelli|1/20/2018|São Paulo|2100|NaN|4200|
|202|933|HL1918|iPhone|3|Camilla|Vieira|4/6/2018|São Paulo|5300|NaN|15900|
|203|934|HL1918|iPhone|3|Breno|Costa|8/26/2018|São Paulo|5300|NaN|15900|
|204|944|HL4379|Televisão|3|Adriana|Passos|5/12/2018|São Paulo|2500|NaN|7500|
|205|948|HL4379|Televisão|1|Luiz|Almeida|1/15/2018|São Paulo|2500|NaN|2500|
|206|952|HL4379|Televisão|3|Mateus|Polastri|2/7/2018|São Paulo|2500|NaN|7500|
|207|956|HL8851|Notebook|2|Alex|Fernandes|9/14/2018|São Paulo|3500|NaN|7000|
|208|958|HL1918|iPhone|4|Gustavo|Guimarães|6/1/2018|São Paulo|5300|NaN|21200|
|209|959|HL4379|Televisão|1|Marcelo|Guadagnino|7/14/2018|São Paulo|2500|NaN|2500|
|210|961|HL9962|Android|5|Lucas|Reis|10/1/2018|São Paulo|3400|NaN|17000|
|211|988|HL8851|Notebook|3|Rilson|Dias|3/10/2018|São Paulo|3500|NaN|10500|
|212|992|HL7348|SmartWatch|3|Matheus|Silva|8/1/2018|São Paulo|1400|NaN|4200|
|213|1000|HL9962|Android|5|Adriana|Passos|5/20/2018|São Paulo|3400|NaN|17000|
|214|1005|HL1148|Câmera|3|Bianca|Piero|9/12/2018|São Paulo|2100|NaN|6300|
|215|1010|HL4379|Televisão|1|João|Aires|9/25/2018|São Paulo|2500|NaN|2500|
|216|1013|HL9962|Android|4|Kimberly|Sad|3/28/2018|São Paulo|3400|NaN|13600|
|217|1015|HL1148|Câmera|3|Roberta|Nogueira|2/7/2018|São Paulo|2100|NaN|6300|
|218|1019|HL1918|iPhone|2|Juliana|Silva|10/15/2018|São Paulo|5300|NaN|10600|
|219|1022|HL1918|iPhone|3|Rodrigo|Souza|9/22/2018|São Paulo|5300|NaN|15900|
|220|1024|HL8851|Notebook|3|Beatriz|Silva|3/25/2018|São Paulo|3500|NaN|10500|
|221|1026|HL1918|iPhone|5|Lucas|Monte|11/11/2018|São Paulo|5300|NaN|26500|
|222|1028|HL7348|SmartWatch|5|Matheus|Afonso|1/1/2018|São Paulo|1400|NaN|7000|
|223|1033|HL1918|iPhone|4|Carolina|Rachide|7/27/2018|São Paulo|5300|NaN|21200|
|224|1036|HL2714|Tablet|3|Bruna|Ramos|5/26/2018|São Paulo|1600|NaN|4800|
|225|1043|HL9962|Android|1|Patrícia|Ferreira|5/21/2018|São Paulo|3400|NaN|3400|
|226|1048|HL1918|iPhone|5|Aline|Andrade|8/3/2018|São Paulo|5300|NaN|26500|
|227|1052|HL1918|iPhone|3|Thiago|Nóbrega|2/3/2018|São Paulo|5300|NaN|15900|
|228|1062|HL1148|Câmera|1|Diego|Mello|6/7/2018|São Paulo|2100|NaN|2100|
|229|1069|HL8851|Notebook|5|Bianca|Tatsch|12/9/2018|São Paulo|3500|NaN|17500|
|230|1070|HL4379|Televisão|3|Andressa|Rotsztejn|4/1/2018|São Paulo|2500|NaN|7500|
|231|1071|HL1918|iPhone|1|Renan|Nucci|5/30/2018|São Paulo|5300|NaN|5300|
|232|1078|HL1148|Câmera|1|Isabela|Chagas|10/29/2018|São Paulo|2100|NaN|2100|
|233|1082|HL4379|Televisão|5|Jessica|Ferreira|6/13/2018|São Paulo|2500|NaN|12500|
|234|1085|HL1148|Câmera|1|Mariana|Miranda|4/8/2018|São Paulo|2100|NaN|2100|
|235|1089|HL4379|Televisão|5|Juliana|Guimarães|10/25/2018|São Paulo|2500|NaN|12500|
|236|1092|HL1918|iPhone|4|Gabriel|Soares|2/2/2018|São Paulo|5300|NaN|21200|
|237|1098|HL1148|Câmera|3|Maria|Junior|12/25/2018|São Paulo|2100|NaN|6300|
|238|1106|HL1918|iPhone|3|Ana|Campos|12/18/2018|São Paulo|5300|NaN|15900|
|239|1108|HL1918|iPhone|3|Bruna|Rosa|7/31/2018|São Paulo|5300|NaN|15900|
|240|1111|HL7348|SmartWatch|1|Morgana|Correa|9/12/2018|São Paulo|1400|NaN|1400|
|241|1118|HL9962|Android|1|Vivianne|Rodrigues|6/3/2018|São Paulo|3400|NaN|3400|
|242|1120|HL8851|Notebook|1|Bernardo|Borges|3/22/2018|São Paulo|3500|NaN|3500|
|243|1124|HL1148|Câmera|3|Renan|Nascimento|12/5/2018|São Paulo|2100|NaN|6300|
|244|1127|HL8851|Notebook|2|Ana|Leite|12/11/2018|São Paulo|3500|NaN|7000|
|245|1132|HL8851|Notebook|2|Yasmim|Verly|5/2/2018|São Paulo|3500|NaN|7000|
|246|1133|HL2714|Tablet|2|Amanda|Roberto|1/27/2018|São Paulo|1600|NaN|3200|
|247|1136|HL1918|iPhone|2|Aline|Mello|1/16/2018|São Paulo|5300|NaN|10600|
|248|1140|HL1148|Câmera|3|Joao|Pereira|11/25/2018|São Paulo|2100|NaN|6300|
|249|1151|HL2714|Tablet|4|Lucas|Fontoura|3/5/2018|São Paulo|1600|NaN|6400|
|250|1157|HL8851|Notebook|2|Patrick|Silva|9/23/2018|São Paulo|3500|NaN|7000|
|251|1169|HL4379|Televisão|1|Maria|Mello|4/18/2018|São Paulo|2500|NaN|2500|
|252|1170|HL1918|iPhone|3|Amanda|Amaral|9/27/2018|São Paulo|5300|NaN|15900|
|253|1174|HL2714|Tablet|2|Andre|Sampaio|8/22/2018|São Paulo|1600|NaN|3200|
|254|1175|HL9962|Android|5|Larissa|Cruz|2/7/2018|São Paulo|3400|NaN|17000|
|255|1189|HL1918|iPhone|1|Caroline|Cavalcanti|1/4/2018|São Paulo|5300|NaN|5300|
|256|1191|HL4379|Televisão|2|João|Silva|2/8/2018|São Paulo|2500|NaN|5000|
|257|1196|HL1918|iPhone|2|Carlos|Assis|5/14/2018|São Paulo|5300|NaN|10600|
|258|1198|HL7348|SmartWatch|2|Giovanna|Santos|7/6/2018|São Paulo|1400|NaN|2800|
|259|1200|HL4379|Televisão|4|Carlos|Mesquita|12/16/2018|São Paulo|2500|NaN|10000|
|260|1211|HL1918|iPhone|3|Manuela|Merege|2/1/2018|São Paulo|5300|NaN|15900|
|261|1212|HL1918|iPhone|2|Stela|Mendonça|9/20/2018|São Paulo|5300|NaN|10600|
|262|1213|HL9962|Android|5|Nina|Magalhães|12/6/2018|São Paulo|3400|NaN|17000|
|263|1214|HL2714|Tablet|3|Yasmim|Verly|4/4/2018|São Paulo|1600|NaN|4800|
|264|1217|HL1918|iPhone|4|Lucas|Assunção|5/30/2018|São Paulo|5300|NaN|21200|
|265|1218|HL8851|Notebook|2|Rafael|Wajnsztok|2/15/2018|São Paulo|3500|NaN|7000|
|266|1223|HL4379|Televisão|3|Lucas|Junior|1/5/2018|São Paulo|2500|NaN|7500|
|267|1224|HL7348|SmartWatch|3|Erick|Soares|4/19/2018|São Paulo|1400|NaN|4200|
|268|1230|HL4379|Televisão|4|Ulisses|Quinto|10/12/2018|São Paulo|2500|NaN|10000|
|269|1231|HL2714|Tablet|2|Victoria|Mazza|4/26/2018|São Paulo|1600|NaN|3200|
|270|1240|HL8851|Notebook|2|Lucas|Coelho|9/24/2018|São Paulo|3500|NaN|7000|
|271|1246|HL1148|Câmera|5|Guilherme|Marchesi|6/16/2018|São Paulo|2100|NaN|10500|
|272|1248|HL1148|Câmera|2|Guilherme|Castilho|11/8/2018|São Paulo|2100|NaN|4200|
|273|1256|HL1918|iPhone|5|Raphael|Ferman|12/13/2018|São Paulo|5300|NaN|26500|
|274|1258|HL8851|Notebook|2|Victoria|Tavares|4/20/2018|São Paulo|3500|NaN|7000|
|275|1269|HL9962|Android|4|Caroll|Johnson|9/24/2018|São Paulo|3400|NaN|13600|
|276|1278|HL1148|Câmera|4|Gabrielle|Figueiredo|10/8/2018|São Paulo|2100|NaN|8400|
|277|1281|HL1148|Câmera|4|Isabela|Rodrigues|12/26/2018|São Paulo|2100|NaN|8400|
|278|1282|HL1918|iPhone|3|Bruno|Freitas|6/30/2018|São Paulo|5300|NaN|15900|
|279|1288|HL1918|iPhone|3|José|Seixas|6/16/2018|São Paulo|5300|NaN|15900|
|280|1289|HL8851|Notebook|5|Julia|Silva|3/6/2018|São Paulo|3500|NaN|17500|
|281|1293|HL1918|iPhone|2|Matheus|Silva|1/26/2018|São Paulo|5300|NaN|10600|
|282|1294|HL9962|Android|2|Guilherme|Vianna|9/18/2018|São Paulo|3400|NaN|6800|
|283|1296|HL1148|Câmera|5|Michelle|Miura|9/10/2018|São Paulo|2100|NaN|10500|
|284|1301|HL1148|Câmera|2|Raphael|Coelho|12/23/2018|São Paulo|2100|NaN|4200|
|285|1302|HL1918|iPhone|1|Bernardo|Nauenberg|12/25/2018|São Paulo|5300|NaN|5300|
|286|1303|HL4379|Televisão|5|Igor|Lima|1/22/2018|São Paulo|2500|NaN|12500|
|287|1304|HL4379|Televisão|4|João|Ribeiro|9/25/2018|São Paulo|2500|NaN|10000|
|288|1305|HL9962|Android|3|Matheus|Delgado|12/17/2018|São Paulo|3400|NaN|10200|
|289|1311|HL8851|Notebook|2|Carolina|Silva|3/2/2018|São Paulo|3500|NaN|7000|
|290|1317|HL4379|Televisão|2|Michelle|Figueiredo|3/11/2018|São Paulo|2500|NaN|5000|
|291|1319|HL4379|Televisão|4|Guilherme|Vianna|12/12/2018|São Paulo|2500|NaN|10000|
|292|1325|HL1918|iPhone|5|Amanda|Machado|4/18/2018|São Paulo|5300|NaN|26500|
|293|1329|HL1148|Câmera|4|Sandy|Moreira|1/6/2018|São Paulo|2100|NaN|8400|
|294|1341|HL4379|Televisão|1|Ana|Campos|8/23/2018|São Paulo|2500|NaN|2500|
|295|1347|HL1918|iPhone|4|Yasmim|Bittencourt|3/7/2018|São Paulo|5300|NaN|21200|
|296|1349|HL4379|Televisão|5|Júlia|Almeida|1/5/2018|São Paulo|2500|NaN|12500|
|297|1353|HL1148|Câmera|2|Fernanda|Ferreira|7/24/2018|São Paulo|2100|NaN|4200|
|298|1356|HL9962|Android|2|Luísa|Fonseca|11/29/2018|São Paulo|3400|NaN|6800|
|299|1361|HL8851|Notebook|3|Carolina|Brum|2/8/2018|São Paulo|3500|NaN|10500|
|300|1365|HL1918|iPhone|3|Victor|Corrêa|6/17/2018|São Paulo|5300|NaN|15900|
|301|1370|HL1918|iPhone|3|Paula|Isbelle|12/17/2018|São Paulo|5300|NaN|15900|
|302|1374|HL2714|Tablet|1|Ives|Teixeira|1/22/2018|São Paulo|1600|NaN|1600|
|303|1385|HL4379|Televisão|2|Roger|Rosa|9/3/2018|São Paulo|2500|NaN|5000|
|304|1392|HL1918|iPhone|3|Lucas|Rocha|11/1/2018|São Paulo|5300|NaN|15900|
|305|1395|HL8851|Notebook|1|Thiago|Nóbrega|3/25/2018|São Paulo|3500|NaN|3500|
|306|1398|HL4379|Televisão|5|Pedro|Buraco|5/12/2018|São Paulo|2500|NaN|12500|
|307|1404|HL9962|Android|1|Luis|Villanova|10/16/2018|São Paulo|3400|NaN|3400|
|308|1409|HL7348|SmartWatch|2|Tainah|Nogueira|12/8/2018|São Paulo|1400|NaN|2800|
|309|1412|HL4379|Televisão|5|Laura|Araujo|12/22/2018|São Paulo|2500|NaN|12500|
|310|1413|HL9962|Android|3|Bianca|Tatsch|11/1/2018|São Paulo|3400|NaN|10200|
|311|1426|HL1918|iPhone|5|Paula|Calbucci|1/14/2018|São Paulo|5300|NaN|26500|
|312|1428|HL1918|iPhone|1|Leticia|Mesquita|9/11/2018|São Paulo|5300|NaN|5300|
|313|1429|HL8851|Notebook|3|Ulisses|Filho|3/24/2018|São Paulo|3500|NaN|10500|
|314|1431|HL7348|SmartWatch|5|Brenno|Santos|5/1/2018|São Paulo|1400|NaN|7000|
|315|1433|HL1148|Câmera|2|Priscila|Carvalho|7/14/2018|São Paulo|2100|NaN|4200|
|316|1441|HL1918|iPhone|5|Andressa|Rotsztejn|3/30/2018|São Paulo|5300|NaN|26500|
|317|1443|HL7348|SmartWatch|3|Vanessa|Neves|10/14/2018|São Paulo|1400|NaN|4200|
|318|1447|HL1918|iPhone|4|Rodrigo|Bruno|9/13/2018|São Paulo|5300|NaN|21200|
|319|1449|HL4379|Televisão|1|Beatriz|Rocha|11/18/2018|São Paulo|2500|NaN|2500|
|320|1459|HL9962|Android|1|Arthur|Souza|3/4/2018|São Paulo|3400|NaN|3400|
|321|1461|HL9962|Android|5|Victor|Franco|10/16/2018|São Paulo|3400|NaN|17000|
|322|1471|HL4379|Televisão|1|Luíza|Melo|8/5/2018|São Paulo|2500|NaN|2500|
|323|1478|HL9962|Android|4|Andressa|Nóbrega|4/15/2018|São Paulo|3400|NaN|13600|
|324|1485|HL4379|Televisão|2|Fabio|Ramos|8/1/2018|São Paulo|2500|NaN|5000|
|325|1496|HL4379|Televisão|3|Adriana|Carneiro|8/25/2018|São Paulo|2500|NaN|7500|
|326|1500|HL7348|SmartWatch|4|Sthefeson|Pereira|12/19/2018|São Paulo|1400|NaN|5600|
|327|1501|HL2714|Tablet|1|Rafael|Portela|11/25/2018|São Paulo|1600|NaN|1600|
|328|1509|HL4379|Televisão|3|Rubens|Netto|12/8/2018|São Paulo|2500|NaN|7500|
|329|1513|HL4379|Televisão|4|Luiza|Farias|10/16/2018|São Paulo|2500|NaN|10000|
|330|1516|HL1918|iPhone|5|Bruna|Silva|8/27/2018|São Paulo|5300|NaN|26500|
|331|1519|HL4379|Televisão|3|Natali|Rangel|4/18/2018|São Paulo|2500|NaN|7500|
|332|1533|HL2714|Tablet|3|Rubens|Netto|7/26/2018|São Paulo|1600|NaN|4800|
|333|1535|HL8851|Notebook|2|Fernanda|Bhering|4/26/2018|São Paulo|3500|NaN|7000|
|334|1537|HL4379|Televisão|4|Rafaela|Ferreira|2/9/2018|São Paulo|2500|NaN|10000|
|335|1538|HL4379|Televisão|2|Thais|Rodrigues|12/31/2018|São Paulo|2500|NaN|5000|
|336|1546|HL4379|Televisão|4|Gabrielle|Silva|3/7/2018|São Paulo|2500|NaN|10000|
|337|1551|HL4379|Televisão|3|João|Tabet|3/27/2018|São Paulo|2500|NaN|7500|
|338|1561|HL1148|Câmera|5|Raphael|Filho|11/23/2018|São Paulo|2100|NaN|10500|
|339|1570|HL1918|iPhone|5|Bruno|Barcessat|2/8/2018|São Paulo|5300|NaN|26500|
|340|1575|HL4379|Televisão|5|Norman|Jimbo|4/20/2018|São Paulo|2500|NaN|12500|
|341|1578|HL9962|Android|1|Pedro|Martins|3/12/2018|São Paulo|3400|NaN|3400|
|342|1581|HL9962|Android|3|Gustavo|Junior|11/21/2018|São Paulo|3400|NaN|10200|
|343|1589|HL8851|Notebook|2|Alon|Pestana|12/20/2018|São Paulo|3500|NaN|7000|
|344|1600|HL4379|Televisão|1|Thomáz|Bôas|1/28/2018|São Paulo|2500|NaN|2500|
|345|1605|HL4379|Televisão|5|João|Capitulo|1/4/2018|São Paulo|2500|NaN|12500|
|346|1608|HL7348|SmartWatch|1|Livia|Codeceira|3/16/2018|São Paulo|1400|NaN|1400|
|347|1609|HL1918|iPhone|3|Carolina|Santos|11/8/2018|São Paulo|5300|NaN|15900|
|348|1611|HL4379|Televisão|5|Wilson|Vianna|5/24/2018|São Paulo|2500|NaN|12500|
|349|1624|HL4379|Televisão|4|Mariane|Ferreira|9/24/2018|São Paulo|2500|NaN|10000|
|350|1629|HL1918|iPhone|4|Eric|Carvalho|12/10/2018|São Paulo|5300|NaN|21200|
|351|1631|HL9962|Android|1|Rebeca|Taylor|1/30/2018|São Paulo|3400|NaN|3400|
|352|1633|HL7348|SmartWatch|5|Maria|Junior|10/16/2018|São Paulo|1400|NaN|7000|
|353|1636|HL1918|iPhone|3|Luísa|Fonseca|7/30/2018|São Paulo|5300|NaN|15900|
|354|1642|HL2714|Tablet|2|Matheus|Santos|1/11/2018|São Paulo|1600|NaN|3200|
|355|1657|HL7348|SmartWatch|1|José|Seixas|3/21/2018|São Paulo|1400|NaN|1400|
|356|1659|HL2714|Tablet|2|Breno|Quinto|5/13/2018|São Paulo|1600|NaN|3200|
|357|1660|HL1918|iPhone|3|Caroline|Cavalcanti|7/11/2018|São Paulo|5300|NaN|15900|
|358|1663|HL8851|Notebook|3|Tadeu|Sousa|2/13/2018|São Paulo|3500|NaN|10500|
|359|1672|HL4379|Televisão|1|Thales|Portillo|2/9/2018|São Paulo|2500|NaN|2500|
|360|1685|HL2714|Tablet|2|Bruna|Gomes|1/11/2018|São Paulo|1600|NaN|3200|
|361|1686|HL1918|iPhone|5|Pedro|Rodrigues|5/26/2018|São Paulo|5300|NaN|26500|
|362|1687|HL1918|iPhone|2|Ruan|Lopes|3/27/2018|São Paulo|5300|NaN|10600|
|363|1703|HL8851|Notebook|4|Caio|Vianna|10/26/2018|São Paulo|3500|NaN|14000|
|364|1704|HL1918|iPhone|4|Patrícia|Amaral|2/19/2018|São Paulo|5300|NaN|21200|
|365|1712|HL4379|Televisão|2|Philipe|Morete|3/8/2018|São Paulo|2500|NaN|5000|
|366|1721|HL7348|SmartWatch|4|Eric|Carvalho|7/8/2018|São Paulo|1400|NaN|5600|
|367|1735|HL1148|Câmera|5|Eduardo|Vargas|5/16/2018|São Paulo|2100|NaN|10500|
|368|1743|HL4379|Televisão|1|Lucas|Freire|10/27/2018|São Paulo|2500|NaN|2500|
|369|1747|HL2714|Tablet|4|Juliana|Pacheco|4/20/2018|São Paulo|1600|NaN|6400|
|370|1748|HL7348|SmartWatch|1|Philipe|Morete|4/14/2018|São Paulo|1400|NaN|1400|
|371|1754|HL4379|Televisão|4|Pedro|Macckione|1/30/2018|São Paulo|2500|NaN|10000|
|372|1756|HL4379|Televisão|2|Caio|Ferreira|3/7/2018|São Paulo|2500|NaN|5000|
|373|1763|HL8851|Notebook|1|Ana|Gomes|10/23/2018|São Paulo|3500|NaN|3500|
|374|1764|HL4379|Televisão|5|Júlio|Freire|7/6/2018|São Paulo|2500|NaN|12500|
|375|1770|HL1918|iPhone|5|Lucas|Aragão|6/12/2018|São Paulo|5300|NaN|26500|
|376|1782|HL1918|iPhone|5|Diego|Mello|12/3/2018|São Paulo|5300|NaN|26500|
|377|1783|HL4379|Televisão|3|Kimberly|Sad|4/26/2018|São Paulo|2500|NaN|7500|
|378|1788|HL2714|Tablet|5|Letícia|Rodrigues|3/31/2018|São Paulo|1600|NaN|8000|
|379|1792|HL1918|iPhone|4|Thales|Gouvêa|9/7/2018|São Paulo|5300|NaN|21200|
|380|1794|HL7348|SmartWatch|4|Matheus|Gomes|12/21/2018|São Paulo|1400|NaN|5600|
|381|1797|HL1918|iPhone|3|Sthefeson|Kohn|1/11/2018|São Paulo|5300|NaN|15900|
|382|1798|HL1918|iPhone|5|Jorge|Carvalho|6/16/2018|São Paulo|5300|NaN|26500|
|383|1800|HL4379|Televisão|3|Lucas|Destri|1/3/2018|São Paulo|2500|NaN|7500|
|384|1802|HL1918|iPhone|1|Mariana|Freire|2/8/2018|São Paulo|5300|NaN|5300|
|385|1809|HL1918|iPhone|1|Lucas|Assunção|11/21/2018|São Paulo|5300|NaN|5300|
|386|1810|HL1918|iPhone|4|Julia|Silva|8/19/2018|São Paulo|5300|NaN|21200|
|387|1813|HL1918|iPhone|4|Lais|Candido|9/14/2018|São Paulo|5300|NaN|21200|
|388|1814|HL7348|SmartWatch|3|Ulisses|Quinto|8/1/2018|São Paulo|1400|NaN|4200|
|389|1830|HL4379|Televisão|4|Carlos|Azevedo|10/25/2018|São Paulo|2500|NaN|10000|
|390|1831|HL1918|iPhone|2|Diego|Mello|4/19/2018|São Paulo|5300|NaN|10600|
|391|1834|HL1918|iPhone|2|Henrique|Lencastre|3/2/2018|São Paulo|5300|NaN|10600|
|392|1835|HL2714|Tablet|3|Thiago|Nóbrega|3/8/2018|São Paulo|1600|NaN|4800|
|393|1836|HL4379|Televisão|3|Juliana|Goes|7/2/2018|São Paulo|2500|NaN|7500|
|394|1850|HL2714|Tablet|1|Thales|Fanara|1/14/2018|São Paulo|1600|NaN|1600|
|395|1852|HL4379|Televisão|2|Ruan|Gonçalves|12/17/2018|São Paulo|2500|NaN|5000|
|396|1853|HL1148|Câmera|5|Marina|Delgado|3/26/2018|São Paulo|2100|NaN|10500|
|397|1855|HL4379|Televisão|4|Thiago|Miura|2/9/2018|São Paulo|2500|NaN|10000|
|398|1857|HL1918|iPhone|4|Gustavo|Junior|6/22/2018|São Paulo|5300|NaN|21200|
|399|1861|HL8851|Notebook|3|Paula|Calbucci|4/28/2018|São Paulo|3500|NaN|10500|
|400|1864|HL2714|Tablet|3|Philipe|Morete|5/9/2018|São Paulo|1600|NaN|4800|
|401|1867|HL1148|Câmera|2|Julia|Leig|9/21/2018|São Paulo|2100|NaN|4200|
|402|1876|HL7348|SmartWatch|1|Matheus|Tostes|5/17/2018|São Paulo|1400|NaN|1400|
|403|1877|HL1918|iPhone|1|Jonas|Gomes|9/13/2018|São Paulo|5300|NaN|5300|
|404|1881|HL9962|Android|3|Rebeca|Reis|9/13/2018|São Paulo|3400|NaN|10200|
|405|1893|HL1148|Câmera|1|Ana|Soledade|8/1/2018|São Paulo|2100|NaN|2100|
|406|1895|HL9962|Android|1|Joyce|Medina|1/1/2018|São Paulo|3400|NaN|3400|
|407|1911|HL4379|Televisão|2|Khaio|Mesquita|12/11/2018|São Paulo|2500|NaN|5000|
|408|1913|HL1918|iPhone|4|Giselia|Thiele|11/8/2018|São Paulo|5300|NaN|21200|
|409|1914|HL9962|Android|3|João|Monteiro|12/10/2018|São Paulo|3400|NaN|10200|
|410|1918|HL4379|Televisão|2|Fernanda|Rubim|6/2/2018|São Paulo|2500|NaN|5000|
|411|1929|HL4379|Televisão|4|Luiza|Cavalcanti|1/16/2018|São Paulo|2500|NaN|10000|
|412|1931|HL4379|Televisão|5|Paula|Isbelle|4/19/2018|São Paulo|2500|NaN|12500|
|413|1932|HL4379|Televisão|2|Lucas|Fontoura|6/30/2018|São Paulo|2500|NaN|5000|
|414|1933|HL1148|Câmera|3|Gabriella|Sagrillo|9/20/2018|São Paulo|2100|NaN|6300|
|415|1934|HL1918|iPhone|3|Isabela|Chagas|11/27/2018|São Paulo|5300|NaN|15900|
|416|1943|HL9962|Android|1|Larissa|Jesus|7/14/2018|São Paulo|3400|NaN|3400|
|417|1945|HL4379|Televisão|3|Bruno|Ferreira|1/13/2018|São Paulo|2500|NaN|7500|
|418|1951|HL9962|Android|4|João|Costa|5/13/2018|São Paulo|3400|NaN|13600|
|419|1953|HL1918|iPhone|1|Matheus|Gomes|3/28/2018|São Paulo|5300|NaN|5300|
|420|1965|HL4379|Televisão|3|Gabriel|Assis|10/21/2018|São Paulo|2500|NaN|7500|
|421|1968|HL9962|Android|2|Paula|Calbucci|5/6/2018|São Paulo|3400|NaN|6800|
|422|1970|HL9962|Android|5|Bruna|Brandao|10/2/2018|São Paulo|3400|NaN|17000|
|423|1975|HL2714|Tablet|4|Maria|Junior|12/16/2018|São Paulo|1600|NaN|6400|
|424|1976|HL9962|Android|4|Carlos|Azevedo|10/10/2018|São Paulo|3400|NaN|13600|
|425|1978|HL4379|Televisão|3|Alon|Guedes|2/19/2018|São Paulo|2500|NaN|7500|
|426|1980|HL7348|SmartWatch|4|Pedro|Pereira|5/12/2018|São Paulo|1400|NaN|5600|
|427|1982|HL2714|Tablet|1|Pedro|Conceição|8/11/2018|São Paulo|1600|NaN|1600|
|428|1986|HL1918|iPhone|4|José|Carvalho|2/27/2018|São Paulo|5300|NaN|21200|
|429|1991|HL2714|Tablet|3|Chan|Santos|6/25/2018|São Paulo|1600|NaN|4800|
|430|1993|HL1918|iPhone|4|João|Abraçado|4/15/2018|São Paulo|5300|NaN|21200|
|431|1999|HL1918|iPhone|5|Marcela|Medeiros|1/16/2018|São Paulo|5300|NaN|26500|
|432|2000|HL4379|Televisão|3|Eduardo|Vargas|7/24/2018|São Paulo|2500|NaN|7500|
|433|2005|HL1918|iPhone|5|Luísa|Fonseca|4/14/2018|São Paulo|5300|NaN|26500|
|434|2014|HL1918|iPhone|4|Juliana|Hollander|7/23/2018|São Paulo|5300|NaN|21200|
|435|2015|HL2714|Tablet|1|David|Vasconcelos|4/17/2018|São Paulo|1600|NaN|1600|
|436|2016|HL1148|Câmera|4|Lucas|Costa|10/1/2018|São Paulo|2100|NaN|8400|
|437|2019|HL1918|iPhone|2|Amanda|Roberto|8/26/2018|São Paulo|5300|NaN|10600|
|438|2022|HL7348|SmartWatch|3|Alessandra|Martins|1/28/2018|São Paulo|1400|NaN|4200|
|439|2030|HL1918|iPhone|2|Lívia|Marques|11/13/2018|São Paulo|5300|NaN|10600|
|440|2032|HL8851|Notebook|1|Jônatas|Tanaka|9/23/2018|São Paulo|3500|NaN|3500|
|441|2033|HL1918|iPhone|3|Marcela|Gasperi|7/31/2018|São Paulo|5300|NaN|15900|
|442|2037|HL9962|Android|2|Ana|Soledade|9/5/2018|São Paulo|3400|NaN|6800|
|443|2041|HL1918|iPhone|4|Giovana|Vilela|6/7/2018|São Paulo|5300|NaN|21200|
|444|2044|HL9962|Android|4|Victor|Oliveira|7/19/2018|São Paulo|3400|NaN|13600|
|445|2047|HL9962|Android|3|Yasmim|Verly|10/7/2018|São Paulo|3400|NaN|10200|
|446|2053|HL2714|Tablet|4|Daniel|Felippe|12/11/2018|São Paulo|1600|NaN|6400|
|447|2068|HL1148|Câmera|1|Luiz|Almeida|9/4/2018|São Paulo|2100|NaN|2100|
|448|2069|HL9962|Android|4|Cláudio|Aragão|5/22/2018|São Paulo|3400|NaN|13600|
|449|2073|HL2714|Tablet|5|Bruno|Temporal|11/6/2018|São Paulo|1600|NaN|8000|
|450|2075|HL1918|iPhone|3|Viviane|Cunha|8/31/2018|São Paulo|5300|NaN|15900|
|451|2077|HL9962|Android|1|Sthefeson|Barroso|1/1/2018|São Paulo|3400|NaN|3400|
|452|2078|HL2714|Tablet|1|Raul|Silveira|2/1/2018|São Paulo|1600|NaN|1600|
|453|2080|HL1148|Câmera|5|Célio|Xavier|4/17/2018|São Paulo|2100|NaN|10500|
|454|2081|HL4379|Televisão|4|Natália|Appel|12/2/2018|São Paulo|2500|NaN|10000|
|455|2089|HL1148|Câmera|3|João|Guadagnino|8/8/2018|São Paulo|2100|NaN|6300|
|456|2097|HL9962|Android|4|Felipe|Cavalcanti|6/27/2018|São Paulo|3400|NaN|13600|
|457|2100|HL1918|iPhone|4|Eric|Carvalho|2/13/2018|São Paulo|5300|NaN|21200|
|458|2105|HL8851|Notebook|3|Giovanna|Santos|10/5/2018|São Paulo|3500|NaN|10500|
|459|2109|HL8851|Notebook|2|Pedro|Sena|4/11/2018|São Paulo|3500|NaN|7000|
|460|2112|HL9962|Android|5|Bárbara|Lima|2/17/2018|São Paulo|3400|NaN|17000|
|461|2113|HL7348|SmartWatch|3|Dykson|Silva|8/24/2018|São Paulo|1400|NaN|4200|
|462|2115|HL1918|iPhone|1|Rafael|Ramos|12/25/2018|São Paulo|5300|NaN|5300|
|463|2119|HL1918|iPhone|3|Juliana|Guimarães|9/30/2018|São Paulo|5300|NaN|15900|
|464|2127|HL1918|iPhone|3|Gabriel|Almeida|5/18/2018|São Paulo|5300|NaN|15900|
|465|2131|HL7348|SmartWatch|2|Lázaro|Nascimento|2/11/2018|São Paulo|1400|NaN|2800|
|466|2135|HL9962|Android|2|Eduardo|Peluzo|3/29/2018|São Paulo|3400|NaN|6800|
|467|2140|HL4379|Televisão|5|Carolina|Silva|10/20/2018|São Paulo|2500|NaN|12500|
|468|2141|HL1148|Câmera|3|Juliana|Silva|10/4/2018|São Paulo|2100|NaN|6300|
|469|2142|HL4379|Televisão|5|Maria|Mello|3/3/2018|São Paulo|2500|NaN|12500|
|470|2147|HL1148|Câmera|1|Marcela|Medeiros|4/9/2018|São Paulo|2100|NaN|2100|
|471|2153|HL4379|Televisão|2|Adriane|Gomes|1/13/2018|São Paulo|2500|NaN|5000|
|472|2154|HL1918|iPhone|2|Livia|Corrêa|7/19/2018|São Paulo|5300|NaN|10600|
|473|2155|HL1918|iPhone|2|Nathan|Cunha|3/14/2018|São Paulo|5300|NaN|10600|
|474|2157|HL8851|Notebook|5|Raíssa|Nimer|3/31/2018|São Paulo|3500|NaN|17500|
|475|2158|HL1918|iPhone|3|José|Seixas|3/29/2018|São Paulo|5300|NaN|15900|
|476|2170|HL7348|SmartWatch|3|Vitor|Arruda|1/31/2018|São Paulo|1400|NaN|4200|
|477|2171|HL8851|Notebook|1|Eduardo|Lopes|9/8/2018|São Paulo|3500|NaN|3500|
|478|2183|HL1918|iPhone|2|Andreza|Ramos|6/23/2018|São Paulo|5300|NaN|10600|
|479|2186|HL2714|Tablet|4|João|Castilho|12/29/2018|São Paulo|1600|NaN|6400|
|480|2187|HL2714|Tablet|3|Caio|Ferreira|11/4/2018|São Paulo|1600|NaN|4800|
|481|2189|HL1918|iPhone|4|Sthefeson|Barroso|10/18/2018|São Paulo|5300|NaN|21200|
|482|2197|HL7348|SmartWatch|1|Alvaro|Kranz|11/14/2018|São Paulo|1400|NaN|1400|
|483|2198|HL9962|Android|3|Paola|Abreu|7/26/2018|São Paulo|3400|NaN|10200|
|484|2201|HL2714|Tablet|2|Thales|Portillo|4/12/2018|São Paulo|1600|NaN|3200|
|485|2213|HL1918|iPhone|4|Beatriz|Rodrigues|5/18/2018|São Paulo|5300|NaN|21200|
|486|2214|HL4379|Televisão|1|Carolina|Carneiro|5/29/2018|São Paulo|2500|NaN|2500|
|487|2218|HL4379|Televisão|5|Alex|Fernandes|11/4/2018|São Paulo|2500|NaN|12500|
|488|2225|HL1148|Câmera|3|Caio|Affonso|4/18/2018|São Paulo|2100|NaN|6300|
|489|2226|HL2714|Tablet|3|João|Júnior|10/1/2018|São Paulo|1600|NaN|4800|
|490|2231|HL2714|Tablet|3|Luiz|Almeida|5/2/2018|São Paulo|1600|NaN|4800|
|491|2233|HL8851|Notebook|2|Ylana|Teraoka|6/4/2018|São Paulo|3500|NaN|7000|
|492|2239|HL4379|Televisão|5|Victor|Firmino|2/27/2018|São Paulo|2500|NaN|12500|
|493|2244|HL4379|Televisão|1|Renan|Nucci|3/29/2018|São Paulo|2500|NaN|2500|
|494|2255|HL1148|Câmera|4|Victoria|Mazza|2/13/2018|São Paulo|2100|NaN|8400|
|495|2260|HL9962|Android|2|Henrique|Silva|9/15/2018|São Paulo|3400|NaN|6800|
|496|2265|HL1918|iPhone|4|Luis|Oliveira|4/11/2018|São Paulo|5300|NaN|21200|
|497|2267|HL2714|Tablet|2|Manuela|Merege|6/29/2018|São Paulo|1600|NaN|3200|
|498|2280|HL9962|Android|2|Jéssica|Netto|5/17/2018|São Paulo|3400|NaN|6800|
|499|2282|HL2714|Tablet|3|Ana|Felippe|10/6/2018|São Paulo|1600|NaN|4800|
|500|2283|HL9962|Android|2|Eduardo|Quindeler|7/21/2018|São Paulo|3400|NaN|6800|
|501|2287|HL1148|Câmera|5|Sarah|Souza|9/11/2018|São Paulo|2100|NaN|10500|
|502|2292|HL7348|SmartWatch|5|Luiz|Campista|1/21/2018|São Paulo|1400|NaN|7000|
|503|2306|HL1148|Câmera|3|Antônio|Oliveira|4/14/2018|São Paulo|2100|NaN|6300|
|504|2308|HL2714|Tablet|2|Livia|Corrêa|12/4/2018|São Paulo|1600|NaN|3200|
|505|2316|HL8851|Notebook|4|Mariana|Sousa|12/1/2018|São Paulo|3500|NaN|14000|
|506|2319|HL1918|iPhone|2|José|Vieira|2/26/2018|São Paulo|5300|NaN|10600|
|507|2321|HL7348|SmartWatch|3|Ananda|Dias|11/14/2018|São Paulo|1400|NaN|4200|
|508|2322|HL1918|iPhone|1|Renan|Nascimento|3/22/2018|São Paulo|5300|NaN|5300|
|509|2324|HL9962|Android|4|Ylana|Teraoka|7/8/2018|São Paulo|3400|NaN|13600|
|510|2326|HL8851|Notebook|4|Paula|Calbucci|10/14/2018|São Paulo|3500|NaN|14000|
|511|2330|HL8851|Notebook|2|Gabriela|Mello|3/8/2018|São Paulo|3500|NaN|7000|
|512|2331|HL1918|iPhone|5|Alex|Fernandes|2/17/2018|São Paulo|5300|NaN|26500|
|513|2335|HL4379|Televisão|3|Carolina|Silva|9/11/2018|São Paulo|2500|NaN|7500|
|514|2338|HL8851|Notebook|3|Felipe|Mendonça|9/8/2018|São Paulo|3500|NaN|10500|
|515|2352|HL9962|Android|4|Ana|Campos|11/15/2018|São Paulo|3400|NaN|13600|
|516|2365|HL4379|Televisão|4|David|Vasconcelos|9/16/2018|São Paulo|2500|NaN|10000|
|517|2384|HL7348|SmartWatch|5|Raphael|Mattos|12/30/2018|São Paulo|1400|NaN|7000|
|518|2385|HL9962|Android|5|Juan|Fernandes|4/28/2018|São Paulo|3400|NaN|17000|
|519|2392|HL8851|Notebook|1|Lucas|Assunção|8/8/2018|São Paulo|3500|NaN|3500|
|520|2395|HL1918|iPhone|4|Kimberly|Sad|5/14/2018|São Paulo|5300|NaN|21200|
|521|2399|HL7348|SmartWatch|3|Gabrielle|Silva|12/3/2018|São Paulo|1400|NaN|4200|
|522|2400|HL2714|Tablet|2|Juliana|Silva|12/22/2018|São Paulo|1600|NaN|3200|
|523|2408|HL8851|Notebook|3|Ives|Teixeira|12/28/2018|São Paulo|3500|NaN|10500|
|524|2409|HL8851|Notebook|5|Raissa|Maia|2/3/2018|São Paulo|3500|NaN|17500|
|525|2411|HL9962|Android|5|William|Mendonça|3/22/2018|São Paulo|3400|NaN|17000|
|526|2412|HL2714|Tablet|1|Isabella|Rodrigues|8/6/2018|São Paulo|1600|NaN|1600|
|527|2417|HL7348|SmartWatch|4|Jéssica|Resinente|8/17/2018|São Paulo|1400|NaN|5600|
|528|2438|HL7348|SmartWatch|1|Victor|Corrêa|3/14/2018|São Paulo|1400|NaN|1400|
|529|2448|HL4379|Televisão|1|Jeferson|Sone|12/22/2018|São Paulo|2500|NaN|2500|
|530|2450|HL2714|Tablet|2|Bruna|Londero|5/29/2018|São Paulo|1600|NaN|3200|
|531|2451|HL2714|Tablet|1|João|Pedrazza|2/12/2018|São Paulo|1600|NaN|1600|
|532|2454|HL1148|Câmera|3|Diego|Mello|1/28/2018|São Paulo|2100|NaN|6300|
|533|2455|HL9962|Android|1|Gabrielle|Figueiredo|7/29/2018|São Paulo|3400|NaN|3400|
|534|2463|HL1918|iPhone|1|Vinícius|Antunes|2/10/2018|São Paulo|5300|NaN|5300|
|535|2464|HL8851|Notebook|4|Gabrielle|Figueiredo|6/27/2018|São Paulo|3500|NaN|14000|
|536|2470|HL4379|Televisão|5|Felipe|Mello|9/19/2018|São Paulo|2500|NaN|12500|
|537|2480|HL1918|iPhone|1|Raphael|Rezende|8/17/2018|São Paulo|5300|NaN|5300|
|538|2483|HL4379|Televisão|5|Ulisses|Filho|8/30/2018|São Paulo|2500|NaN|12500|
|539|2494|HL4379|Televisão|3|José|Vieira|5/9/2018|São Paulo|2500|NaN|7500|
|540|2496|HL2714|Tablet|1|Luíza|Garcia|1/3/2018|São Paulo|1600|NaN|1600|
|541|2502|HL8851|Notebook|3|Célio|Xavier|2/15/2018|São Paulo|3500|NaN|10500|
|542|2504|HL2714|Tablet|1|Guilherme|Merotto|6/21/2018|São Paulo|1600|NaN|1600|
|543|2507|HL8851|Notebook|3|Thomáz|Vannier|7/3/2018|São Paulo|3500|NaN|10500|
|544|2511|HL4379|Televisão|5|Lucas|Costa|12/16/2018|São Paulo|2500|NaN|12500|
|545|2518|HL4379|Televisão|1|Pedro|Lyra|2/12/2018|São Paulo|2500|NaN|2500|
|546|2519|HL4379|Televisão|4|Eduardo|Vargas|4/2/2018|São Paulo|2500|NaN|10000|
|547|2525|HL4379|Televisão|3|Beatriz|Rocha|12/27/2018|São Paulo|2500|NaN|7500|
|548|2530|HL1148|Câmera|2|Isabelle|Gonçalves|2/12/2018|São Paulo|2100|NaN|4200|
|549|2533|HL1918|iPhone|4|Larissa|Jesus|7/5/2018|São Paulo|5300|NaN|21200|
|550|2539|HL8851|Notebook|2|Larissa|Jesus|3/25/2018|São Paulo|3500|NaN|7000|
|551|2547|HL4379|Televisão|4|Jéssica|Netto|11/5/2018|São Paulo|2500|NaN|10000|
|552|2548|HL1918|iPhone|5|Gustavo|Thome|3/30/2018|São Paulo|5300|NaN|26500|
|553|2550|HL7348|SmartWatch|5|Guilherme|Merotto|3/7/2018|São Paulo|1400|NaN|7000|
|554|2554|HL1918|iPhone|3|João|Siqueira|9/28/2018|São Paulo|5300|NaN|15900|
|555|2569|HL2714|Tablet|3|Bernard|Pedrosa|3/27/2018|São Paulo|1600|NaN|4800|
|556|2571|HL1148|Câmera|4|Roberta|Pimenta|9/14/2018|São Paulo|2100|NaN|8400|
|557|2574|HL4379|Televisão|2|Raphael|Coelho|6/20/2018|São Paulo|2500|NaN|5000|
|558|2579|HL2714|Tablet|1|Carolina|Silva|10/23/2018|São Paulo|1600|NaN|1600|
|559|2580|HL9962|Android|4|Arthur|Souza|8/21/2018|São Paulo|3400|NaN|13600|
|560|2586|HL4379|Televisão|2|Bruna|Chein|8/29/2018|São Paulo|2500|NaN|5000|
|561|2600|HL1918|iPhone|2|Danilo|Alves|8/29/2018|São Paulo|5300|NaN|10600|
|562|2602|HL4379|Televisão|2|Bruna|Ramos|6/1/2018|São Paulo|2500|NaN|5000|
|563|2603|HL1918|iPhone|1|Carolina|Bernardes|8/23/2018|São Paulo|5300|NaN|5300|
|564|2605|HL9962|Android|5|Bruno|Ursulino|12/1/2018|São Paulo|3400|NaN|17000|
|565|2619|HL7348|SmartWatch|5|Glenda|Santos|4/30/2018|São Paulo|1400|NaN|7000|
|566|2622|HL7348|SmartWatch|2|Pedro|Ferrari|4/4/2018|São Paulo|1400|NaN|2800|
|567|2628|HL8851|Notebook|3|Cassio|Faria|8/8/2018|São Paulo|3500|NaN|10500|
|568|2631|HL1918|iPhone|5|Andressa|Nóbrega|3/16/2018|São Paulo|5300|NaN|26500|
|569|2633|HL4379|Televisão|2|Marina|Delgado|9/30/2018|São Paulo|2500|NaN|5000|
|570|2638|HL9962|Android|1|Lucas|Almeida|6/5/2018|São Paulo|3400|NaN|3400|
|571|2646|HL1918|iPhone|2|Igor|Azevedo|6/14/2018|São Paulo|5300|NaN|10600|
|572|2647|HL1148|Câmera|3|Ana|Campos|12/2/2018|São Paulo|2100|NaN|6300|
|573|2655|HL1918|iPhone|1|Raphael|Guedes|4/12/2018|São Paulo|5300|NaN|5300|
|574|2663|HL2714|Tablet|2|Pedro|Ayres|10/5/2018|São Paulo|1600|NaN|3200|
|575|2671|HL1918|iPhone|4|Gustavo|Aragão|9/26/2018|São Paulo|5300|NaN|21200|
|576|2673|HL4379|Televisão|1|Erick|Soares|3/10/2018|São Paulo|2500|NaN|2500|
|577|2674|HL8851|Notebook|3|Wendela|Mariz|8/15/2018|São Paulo|3500|NaN|10500|
|578|2675|HL9962|Android|3|Leticia|Mesquita|2/22/2018|São Paulo|3400|NaN|10200|
|579|2678|HL1918|iPhone|4|Ruan|Lopes|1/16/2018|São Paulo|5300|NaN|21200|
|580|2686|HL1918|iPhone|5|Deysiane|Medronho|4/26/2018|São Paulo|5300|NaN|26500|
|581|2688|HL4379|Televisão|1|Bernard|Pedrosa|3/4/2018|São Paulo|2500|NaN|2500|
|582|2700|HL4379|Televisão|2|Fernanda|Rubim|11/23/2018|São Paulo|2500|NaN|5000|
|583|2701|HL4379|Televisão|4|Desirée|Heimlich|12/4/2018|São Paulo|2500|NaN|10000|
|584|2706|HL1918|iPhone|4|Marina|Miranda|6/18/2018|São Paulo|5300|NaN|21200|
|585|2717|HL9962|Android|4|Livia|Cozendey|10/23/2018|São Paulo|3400|NaN|13600|
|586|2725|HL8851|Notebook|5|Rafael|Portela|5/4/2018|São Paulo|3500|NaN|17500|
|587|2728|HL2714|Tablet|3|José|Marques|8/29/2018|São Paulo|1600|NaN|4800|
|588|2730|HL1918|iPhone|3|Gabriel|Thoni|6/13/2018|São Paulo|5300|NaN|15900|
|589|2731|HL1918|iPhone|3|Raísa|Rodrigues|2/2/2018|São Paulo|5300|NaN|15900|
|590|2736|HL4379|Televisão|1|Ruan|Lopes|3/16/2018|São Paulo|2500|NaN|2500|
|591|2737|HL9962|Android|4|Norman|Jimbo|8/4/2018|São Paulo|3400|NaN|13600|
|592|2740|HL7348|SmartWatch|4|Thomaz|Ferreira|7/25/2018|São Paulo|1400|NaN|5600|
|593|2742|HL1148|Câmera|2|Gustavo|Azevedo|11/21/2018|São Paulo|2100|NaN|4200|
|594|2743|HL4379|Televisão|4|João|Castilho|3/24/2018|São Paulo|2500|NaN|10000|
|595|2746|HL9962|Android|4|Ives|Teixeira|5/8/2018|São Paulo|3400|NaN|13600|
|596|2747|HL8851|Notebook|5|Carolina|Abrahão|4/30/2018|São Paulo|3500|NaN|17500|
|597|2752|HL1918|iPhone|2|Anna|Silva|12/13/2018|São Paulo|5300|NaN|10600|
|598|2756|HL4379|Televisão|1|Pedro|Xavier|7/13/2018|São Paulo|2500|NaN|2500|
|599|2769|HL1148|Câmera|2|Matheus|Gomes|8/21/2018|São Paulo|2100|NaN|4200|
|600|2770|HL9962|Android|3|Camilla|Cardeman|10/7/2018|São Paulo|3400|NaN|10200|
|601|2772|HL1918|iPhone|5|Matheus|Silva|3/17/2018|São Paulo|5300|NaN|26500|
|602|2781|HL7348|SmartWatch|3|Rachel|Silva|10/18/2018|São Paulo|1400|NaN|4200|
|603|2783|HL1918|iPhone|4|Juliana|Guimarães|3/14/2018|São Paulo|5300|NaN|21200|
|604|2795|HL7348|SmartWatch|3|Camila|Bastazini|8/17/2018|São Paulo|1400|NaN|4200|
|605|2805|HL7348|SmartWatch|3|Lucas|Lima|7/29/2018|São Paulo|1400|NaN|4200|
|606|2808|HL7348|SmartWatch|2|Adriana|Passos|5/19/2018|São Paulo|1400|NaN|2800|
|607|2814|HL1918|iPhone|1|Pedro|Oliveira|6/5/2018|São Paulo|5300|NaN|5300|
|608|2827|HL7348|SmartWatch|1|Eduardo|Silva|3/8/2018|São Paulo|1400|NaN|1400|
|609|2831|HL7348|SmartWatch|1|Luis|Souza|1/25/2018|São Paulo|1400|NaN|1400|
|610|2832|HL1918|iPhone|4|Jonatas|Passos|4/11/2018|São Paulo|5300|NaN|21200|
|611|2834|HL9962|Android|1|Diego|Marchesi|10/24/2018|São Paulo|3400|NaN|3400|
|612|2838|HL2714|Tablet|5|Joao|Pereira|2/4/2018|São Paulo|1600|NaN|8000|
|613|2839|HL8851|Notebook|1|Mariana|Freire|5/10/2018|São Paulo|3500|NaN|3500|
|614|2840|HL8851|Notebook|4|Beatriz|Silva|8/20/2018|São Paulo|3500|NaN|14000|
|615|2841|HL1918|iPhone|4|Breno|Farias|1/2/2018|São Paulo|5300|NaN|21200|
|616|2842|HL1918|iPhone|1|Carlos|Galvão|6/11/2018|São Paulo|5300|NaN|5300|
|617|2845|HL7348|SmartWatch|2|Giselia|Thiele|9/1/2018|São Paulo|1400|NaN|2800|
|618|2847|HL4379|Televisão|3|Daniel|Sousa|9/13/2018|São Paulo|2500|NaN|7500|
|619|2868|HL1918|iPhone|4|Fernanda|Silva|12/11/2018|São Paulo|5300|NaN|21200|
|620|2880|HL1918|iPhone|5|Matheus|Gomes|11/22/2018|São Paulo|5300|NaN|26500|
|621|2881|HL9962|Android|2|Karine|Barros|1/7/2018|São Paulo|3400|NaN|6800|
|622|2885|HL8851|Notebook|4|Pedro|Oliveira|11/1/2018|São Paulo|3500|NaN|14000|
|623|2886|HL9962|Android|5|Rafaela|Gomes|1/10/2018|São Paulo|3400|NaN|17000|
|624|2888|HL7348|SmartWatch|5|Lívia|Tanaka|7/12/2018|São Paulo|1400|NaN|7000|
|625|2898|HL4379|Televisão|4|Lucas|Assunção|7/24/2018|São Paulo|2500|NaN|10000|
|626|2907|HL1918|iPhone|1|Kim|Ferreira|9/7/2018|São Paulo|5300|NaN|5300|
|627|2908|HL4379|Televisão|1|Priscila|Carvalho|1/30/2018|São Paulo|2500|NaN|2500|
|628|2910|HL1918|iPhone|4|Renan|Melo|3/24/2018|São Paulo|5300|NaN|21200|
|629|2911|HL4379|Televisão|3|Daniel|Sousa|12/7/2018|São Paulo|2500|NaN|7500|
|630|2914|HL1918|iPhone|4|João|Júnior|5/7/2018|São Paulo|5300|NaN|21200|
|631|2919|HL1918|iPhone|3|Eduardo|Vargas|8/13/2018|São Paulo|5300|NaN|15900|
|632|2921|HL4379|Televisão|3|Luiz|Marinho|11/15/2018|São Paulo|2500|NaN|7500|
|633|2923|HL1918|iPhone|1|Katharina|Barros|9/17/2018|São Paulo|5300|NaN|5300|
|634|2925|HL1918|iPhone|1|Fernanda|Rubim|7/15/2018|São Paulo|5300|NaN|5300|
|635|2926|HL1918|iPhone|2|Lucas|Freire|8/9/2018|São Paulo|5300|NaN|10600|
|636|2930|HL1918|iPhone|3|Carolina|Costa|5/3/2018|São Paulo|5300|NaN|15900|
|637|2938|HL9962|Android|3|Allan|Guedes|11/28/2018|São Paulo|3400|NaN|10200|
|638|2939|HL4379|Televisão|3|Gabriel|Silva|4/23/2018|São Paulo|2500|NaN|7500|
|639|2944|HL8851|Notebook|5|Lívia|Marques|1/9/2018|São Paulo|3500|NaN|17500|
|640|2945|HL9962|Android|5|Célio|Xavier|7/1/2018|São Paulo|3400|NaN|17000|
|641|2975|HL1918|iPhone|5|Andre|Nóbrega|2/21/2018|São Paulo|5300|NaN|26500|
|642|2977|HL7348|SmartWatch|4|Sylvio|Bernhardt|7/15/2018|São Paulo|1400|NaN|5600|
|643|2993|HL2714|Tablet|1|Leonardo|Faria|7/5/2018|São Paulo|1600|NaN|1600|
|644|2997|HL9962|Android|5|Gabriella|Sagrillo|9/17/2018|São Paulo|3400|NaN|17000|
|645|3000|HL4379|Televisão|2|Natalia|Marinho|3/2/2018|São Paulo|2500|NaN|5000|
|646|3006|HL9962|Android|2|Ives|Barbosa|12/31/2018|São Paulo|3400|NaN|6800|
|647|3015|HL4379|Televisão|4|Jéssica|Stefanelli|2/15/2018|São Paulo|2500|NaN|10000|
|648|3017|HL1918|iPhone|3|Eduardo|Pacheco|9/21/2018|São Paulo|5300|NaN|15900|
|649|3020|HL4379|Televisão|5|Caroline|Pinto|11/21/2018|São Paulo|2500|NaN|12500|
|650|3022|HL1148|Câmera|2|Carolina|Siqueira|6/16/2018|São Paulo|2100|NaN|4200|
|651|3023|HL4379|Televisão|5|Caio|Moura|4/29/2018|São Paulo|2500|NaN|12500|
|652|3028|HL1918|iPhone|5|Adrielle|Vieira|9/11/2018|São Paulo|5300|NaN|26500|
|653|3029|HL1918|iPhone|3|Iuri|Barbosa|11/27/2018|São Paulo|5300|NaN|15900|
|654|3037|HL9962|Android|3|Matheus|Figueiredo|11/7/2018|São Paulo|3400|NaN|10200|
|655|3038|HL4379|Televisão|2|Bruna|Londero|11/17/2018|São Paulo|2500|NaN|5000|
|656|3043|HL4379|Televisão|4|Bruna|Silveira|4/9/2018|São Paulo|2500|NaN|10000|
|657|3051|HL9962|Android|5|Izabel|Lopes|6/9/2018|São Paulo|3400|NaN|17000|
|658|3058|HL4379|Televisão|5|Pedro|Macckione|2/17/2018|São Paulo|2500|NaN|12500|
|659|3071|HL4379|Televisão|1|Rafaela|Ferreira|3/17/2018|São Paulo|2500|NaN|2500|
|660|3073|HL2714|Tablet|2|Adrielle|Forte|8/2/2018|São Paulo|1600|NaN|3200|
|661|3077|HL4379|Televisão|2|Mariana|Barrozo|5/29/2018|São Paulo|2500|NaN|5000|
|662|3089|HL1148|Câmera|2|Fabio|Sepúlveda|1/7/2018|São Paulo|2100|NaN|4200|
|663|3090|HL1918|iPhone|3|Audir|Franco|2/8/2018|São Paulo|5300|NaN|15900|
|664|3103|HL1148|Câmera|1|Wendela|Veloso|9/9/2018|São Paulo|2100|NaN|2100|
|665|3104|HL9962|Android|4|Guilherme|Seixas|9/18/2018|São Paulo|3400|NaN|13600|
|666|3108|HL7348|SmartWatch|3|Gustavo|Aragão|2/13/2018|São Paulo|1400|NaN|4200|
|667|3109|HL9962|Android|1|Matheus|Silva|8/2/2018|São Paulo|3400|NaN|3400|
|668|3110|HL1918|iPhone|5|Jônatas|Soares|11/13/2018|São Paulo|5300|NaN|26500|
|669|3115|HL2714|Tablet|2|Mariana|Freire|5/10/2018|São Paulo|1600|NaN|3200|
|670|3120|HL9962|Android|3|Ulisses|Filho|7/4/2018|São Paulo|3400|NaN|10200|
|671|3126|HL1918|iPhone|3|Gabriela|Cavalcanti|6/20/2018|São Paulo|5300|NaN|15900|
|672|3128|HL8851|Notebook|5|Bernard|Pedrosa|10/16/2018|São Paulo|3500|NaN|17500|
|673|3130|HL7348|SmartWatch|3|Camila|Sobral|7/28/2018|São Paulo|1400|NaN|4200|
|674|3133|HL8851|Notebook|1|Katharina|Barros|1/23/2018|São Paulo|3500|NaN|3500|
|675|3134|HL4379|Televisão|5|Thays|Castro|7/21/2018|São Paulo|2500|NaN|12500|
|676|3135|HL4379|Televisão|4|Breno|Costa|5/9/2018|São Paulo|2500|NaN|10000|
|677|3137|HL4379|Televisão|1|Rilson|Dias|5/29/2018|São Paulo|2500|NaN|2500|
|678|3138|HL9962|Android|1|Anna|Figueiredo|9/5/2018|São Paulo|3400|NaN|3400|
|679|3145|HL1918|iPhone|4|Fernanda|Ferreira|2/15/2018|São Paulo|5300|NaN|21200|
|680|3147|HL9962|Android|4|Andressa|Rotsztejn|10/21/2018|São Paulo|3400|NaN|13600|
|681|3154|HL1918|iPhone|2|Victor|Oliveira|8/13/2018|São Paulo|5300|NaN|10600|
|682|3160|HL1148|Câmera|5|Cláudio|Aragão|5/7/2018|São Paulo|2100|NaN|10500|
|683|3164|HL8851|Notebook|1|Itai|Puntel|10/30/2018|São Paulo|3500|NaN|3500|
|684|3165|HL7348|SmartWatch|4|Daniel|Monteiro|4/30/2018|São Paulo|1400|NaN|5600|
|685|3169|HL1148|Câmera|2|Hanna|Fonseca|9/9/2018|São Paulo|2100|NaN|4200|
|686|3174|HL7348|SmartWatch|1|Patrícia|Ferreira|8/3/2018|São Paulo|1400|NaN|1400|
|687|3178|HL1918|iPhone|1|Guilherme|Santos|1/9/2018|São Paulo|5300|NaN|5300|
|688|3187|HL8851|Notebook|2|Giulia|Lopes|8/1/2018|São Paulo|3500|NaN|7000|
|689|3194|HL9962|Android|1|Antonio|Bernhardt|8/21/2018|São Paulo|3400|NaN|3400|
|690|3198|HL2714|Tablet|5|Mariana|Barrozo|7/29/2018|São Paulo|1600|NaN|8000|
|691|3205|HL4379|Televisão|5|Andressa|Chou|1/18/2018|São Paulo|2500|NaN|12500|
|692|3210|HL8851|Notebook|3|Beatriz|Nogueira|2/18/2018|São Paulo|3500|NaN|10500|
|693|3211|HL2714|Tablet|3|Thaís|Moura|2/26/2018|São Paulo|1600|NaN|4800|
|694|3213|HL4379|Televisão|2|Alexandre|Rodriguez|4/21/2018|São Paulo|2500|NaN|5000|
|695|3214|HL4379|Televisão|2|Marcelo|Rosa|7/9/2018|São Paulo|2500|NaN|5000|
|696|3221|HL1918|iPhone|3|Pedro|Dalforne|4/15/2018|São Paulo|5300|NaN|15900|
|697|3224|HL8851|Notebook|2|Michelle|Miura|8/5/2018|São Paulo|3500|NaN|7000|
|698|3227|HL2714|Tablet|4|Mateus|Duque|5/31/2018|São Paulo|1600|NaN|6400|
|699|3229|HL1918|iPhone|1|Joao|Pereira|2/13/2018|São Paulo|5300|NaN|5300|
|700|3230|HL1148|Câmera|4|Rodrigo|Silva|4/15/2018|São Paulo|2100|NaN|8400|
|701|3235|HL9962|Android|1|Gabriel|Ribeiro|5/5/2018|São Paulo|3400|NaN|3400|
|702|3238|HL1918|iPhone|5|Lívia|Tanaka|3/23/2018|São Paulo|5300|NaN|26500|
|703|3244|HL1918|iPhone|2|Henrique|Villanova|3/2/2018|São Paulo|5300|NaN|10600|
|704|3246|HL7348|SmartWatch|1|Breno|Farias|3/14/2018|São Paulo|1400|NaN|1400|
|705|3252|HL4379|Televisão|5|Deysiane|Bach|2/24/2018|São Paulo|2500|NaN|12500|
|706|3255|HL4379|Televisão|5|Matheus|Delgado|2/28/2018|São Paulo|2500|NaN|12500|
|707|3258|HL9962|Android|1|Anna|Silva|5/31/2018|São Paulo|3400|NaN|3400|
|708|3260|HL1918|iPhone|5|Rachel|Restum|2/28/2018|São Paulo|5300|NaN|26500|
|709|3262|HL1148|Câmera|2|Sandy|Figueiredo|7/26/2018|São Paulo|2100|NaN|4200|
|710|3263|HL4379|Televisão|2|Eduardo|Silva|8/21/2018|São Paulo|2500|NaN|5000|
|711|3264|HL1148|Câmera|5|Vitor|Boccaletti|1/3/2018|São Paulo|2100|NaN|10500|
|712|3272|HL9962|Android|4|Lucas|Freire|9/30/2018|São Paulo|3400|NaN|13600|
|713|3274|HL1918|iPhone|3|Bruno|Oliveira|9/26/2018|São Paulo|5300|NaN|15900|
|714|3277|HL9962|Android|2|Adrielle|Forte|12/28/2018|São Paulo|3400|NaN|6800|
|715|3288|HL8851|Notebook|3|Gabriel|Soares|8/6/2018|São Paulo|3500|NaN|10500|
|716|3292|HL2714|Tablet|1|Danilo|Mendonça|1/25/2018|São Paulo|1600|NaN|1600|
|717|3296|HL8851|Notebook|5|Rubens|Netto|2/10/2018|São Paulo|3500|NaN|17500|
|718|3300|HL1918|iPhone|1|Fernanda|Ferreira|10/26/2018|São Paulo|5300|NaN|5300|
|719|3303|HL8851|Notebook|2|Sandy|Ribeiro|12/24/2018|São Paulo|3500|NaN|7000|
|720|3304|HL2714|Tablet|5|Eduardo|Soares|10/28/2018|São Paulo|1600|NaN|8000|
|721|3309|HL1918|iPhone|3|Wilson|Brandão|2/16/2018|São Paulo|5300|NaN|15900|
|722|3314|HL9962|Android|3|Mateus|Franco|10/1/2018|São Paulo|3400|NaN|10200|
|723|3315|HL1148|Câmera|1|Carlos|Portela|9/27/2018|São Paulo|2100|NaN|2100|
|724|3316|HL1148|Câmera|2|Carlos|Azevedo|7/19/2018|São Paulo|2100|NaN|4200|
|725|3321|HL8851|Notebook|4|Gabriela|Mello|3/27/2018|São Paulo|3500|NaN|14000|
|726|3323|HL7348|SmartWatch|1|Jéssica|Resinente|11/14/2018|São Paulo|1400|NaN|1400|
|727|3329|HL4379|Televisão|2|Livia|Corrêa|4/30/2018|São Paulo|2500|NaN|5000|
|728|3333|HL9962|Android|1|Michelle|Miura|10/29/2018|São Paulo|3400|NaN|3400|
|729|3335|HL1148|Câmera|3|Eduardo|Soares|10/2/2018|São Paulo|2100|NaN|6300|
|730|3337|HL2714|Tablet|5|Jeferson|Costa|1/11/2018|São Paulo|1600|NaN|8000|
|731|3344|HL1148|Câmera|2|Allan|Guedes|11/27/2018|São Paulo|2100|NaN|4200|
|732|3345|HL1918|iPhone|2|Gabriel|Azevedo|2/5/2018|São Paulo|5300|NaN|10600|
|733|3349|HL1918|iPhone|4|Jônatas|Castro|6/7/2018|São Paulo|5300|NaN|21200|
|734|3351|HL1918|iPhone|3|Gabriel|Garcia|12/4/2018|São Paulo|5300|NaN|15900|
|735|3363|HL9962|Android|1|Leandro|Ferreira|11/1/2018|São Paulo|3400|NaN|3400|
|736|3365|HL7348|SmartWatch|1|Luiz|Freire|6/24/2018|São Paulo|1400|NaN|1400|
|737|3366|HL4379|Televisão|2|Lucas|Neto|2/16/2018|São Paulo|2500|NaN|5000|
|738|3375|HL1918|iPhone|5|Amanda|Gontijo|12/15/2018|São Paulo|5300|NaN|26500|
|739|3389|HL1148|Câmera|4|Hércules|Moreira|5/21/2018|São Paulo|2100|NaN|8400|
|740|3392|HL8851|Notebook|2|Ana|Silva|8/24/2018|São Paulo|3500|NaN|7000|
|741|3397|HL8851|Notebook|1|Beatriz|Cavalcanti|4/23/2018|São Paulo|3500|NaN|3500|
|742|3405|HL4379|Televisão|2|Jéssica|Netto|5/3/2018|São Paulo|2500|NaN|5000|
|743|3411|HL8851|Notebook|3|Maria|Assumpção|9/16/2018|São Paulo|3500|NaN|10500|
|744|3413|HL1148|Câmera|4|Priscila|Carvalho|8/7/2018|São Paulo|2100|NaN|8400|
|745|3414|HL1918|iPhone|3|Julia|Penteado|2/25/2018|São Paulo|5300|NaN|15900|
|746|3419|HL4379|Televisão|2|Anízio|Carvalho|1/14/2018|São Paulo|2500|NaN|5000|
|747|3420|HL1918|iPhone|1|Leonardo|Faria|9/20/2018|São Paulo|5300|NaN|5300|
|748|3421|HL1148|Câmera|4|Lívia|Marques|3/18/2018|São Paulo|2100|NaN|8400|
|749|3422|HL7348|SmartWatch|3|Caio|Caldas|7/20/2018|São Paulo|1400|NaN|4200|
|750|3423|HL9962|Android|2|João|Guadagnino|9/30/2018|São Paulo|3400|NaN|6800|
|751|3428|HL9962|Android|2|Gustavo|Gomes|5/4/2018|São Paulo|3400|NaN|6800|
|752|3430|HL1918|iPhone|1|Hanna|Fonseca|3/14/2018|São Paulo|5300|NaN|5300|
|753|3444|HL7348|SmartWatch|2|Breno|Varella|1/14/2018|São Paulo|1400|NaN|2800|
|754|3445|HL2714|Tablet|4|Itai|Puntel|9/28/2018|São Paulo|1600|NaN|6400|
|755|3462|HL7348|SmartWatch|4|Beatriz|Santos|6/27/2018|São Paulo|1400|NaN|5600|
|756|3467|HL8851|Notebook|2|Thomaz|Ferreira|5/27/2018|São Paulo|3500|NaN|7000|
|757|3478|HL8851|Notebook|5|Letícia|Leal|12/30/2018|São Paulo|3500|NaN|17500|
|758|3479|HL4379|Televisão|3|Leandro|Melo|8/17/2018|São Paulo|2500|NaN|7500|
|759|3481|HL4379|Televisão|5|Lucas|Almeida|6/17/2018|São Paulo|2500|NaN|12500|
|760|3484|HL9962|Android|5|Amanda|Procaci|1/10/2018|São Paulo|3400|NaN|17000|
|761|3485|HL4379|Televisão|5|Carlos|Cardoso|5/18/2018|São Paulo|2500|NaN|12500|
|762|3486|HL4379|Televisão|1|Livia|Codeceira|8/5/2018|São Paulo|2500|NaN|2500|
|763|3490|HL1918|iPhone|1|André|Alves|3/28/2018|São Paulo|5300|NaN|5300|
|764|3492|HL4379|Televisão|2|Paula|Isbelle|12/5/2018|São Paulo|2500|NaN|5000|
|765|3498|HL1918|iPhone|3|Larissa|Vasconcellos|1/22/2018|São Paulo|5300|NaN|15900|
|766|3499|HL7348|SmartWatch|5|Guilherme|Lima|9/7/2018|São Paulo|1400|NaN|7000|
|767|3502|HL9962|Android|5|Hanna|Fonseca|7/11/2018|São Paulo|3400|NaN|17000|
|768|3513|HL1918|iPhone|1|Bruno|Temporal|3/23/2018|São Paulo|5300|NaN|5300|
|769|3519|HL1148|Câmera|5|Breno|Varella|7/13/2018|São Paulo|2100|NaN|10500|
|770|3535|HL7348|SmartWatch|4|Luiz|Freire|7/10/2018|São Paulo|1400|NaN|5600|
|771|3540|HL4379|Televisão|1|Maike|Pereira|8/16/2018|São Paulo|2500|NaN|2500|
|772|3547|HL2714|Tablet|2|Bruno|Salomão|10/21/2018|São Paulo|1600|NaN|3200|
|773|3548|HL1918|iPhone|2|Giulia|Pessanha|9/26/2018|São Paulo|5300|NaN|10600|
|774|3555|HL4379|Televisão|2|Guilherme|Monteiro|10/17/2018|São Paulo|2500|NaN|5000|
|775|3557|HL1918|iPhone|3|Carlos|Cardoso|12/6/2018|São Paulo|5300|NaN|15900|
|776|3559|HL8851|Notebook|3|Giulia|Lopes|11/1/2018|São Paulo|3500|NaN|10500|
|777|3560|HL2714|Tablet|4|Monique|Vasconcelos|12/17/2018|São Paulo|1600|NaN|6400|
|778|3562|HL2714|Tablet|3|Juliana|Goes|8/9/2018|São Paulo|1600|NaN|4800|
|779|3567|HL2714|Tablet|2|Lucas|Neto|8/11/2018|São Paulo|1600|NaN|3200|
|780|3575|HL4379|Televisão|1|Gabrielle|Wanderley|10/20/2018|São Paulo|2500|NaN|2500|
|781|3589|HL4379|Televisão|2|Lucas|Fontoura|1/29/2018|São Paulo|2500|NaN|5000|
|782|3590|HL7348|SmartWatch|2|Igor|Lima|5/9/2018|São Paulo|1400|NaN|2800|
|783|3591|HL2714|Tablet|4|Raísa|Rodrigues|9/17/2018|São Paulo|1600|NaN|6400|
|784|3599|HL9962|Android|4|Beatriz|Biase|8/1/2018|São Paulo|3400|NaN|13600|
|785|3608|HL1918|iPhone|4|Carolina|Rocha|6/30/2018|São Paulo|5300|NaN|21200|
|786|3610|HL2714|Tablet|2|Ulisses|Quinto|4/17/2018|São Paulo|1600|NaN|3200|
|787|3616|HL8851|Notebook|4|Guilherme|Assis|6/13/2018|São Paulo|3500|NaN|14000|
|788|3625|HL7348|SmartWatch|5|Gabriel|Puntel|2/22/2018|São Paulo|1400|NaN|7000|
|789|3629|HL1918|iPhone|1|Caio|Fernandes|10/27/2018|São Paulo|5300|NaN|5300|
|790|3633|HL4379|Televisão|3|Ives|Pinheiro|9/18/2018|São Paulo|2500|NaN|7500|
|791|3634|HL9962|Android|4|Daniel|Alcoforado|7/8/2018|São Paulo|3400|NaN|13600|
|792|3636|HL1918|iPhone|2|Silvio|Fahrnholz|9/22/2018|São Paulo|5300|NaN|10600|
|793|3637|HL7348|SmartWatch|3|David|Assumpção|4/12/2018|São Paulo|1400|NaN|4200|
|794|3645|HL1918|iPhone|5|Guilherme|Seixas|9/23/2018|São Paulo|5300|NaN|26500|
|795|3646|HL9962|Android|1|Daniel|Monteiro|10/8/2018|São Paulo|3400|NaN|3400|
|796|3653|HL8851|Notebook|4|Paula|Carneiro|3/18/2018|São Paulo|3500|NaN|14000|
|797|3655|HL4379|Televisão|3|Raissa|Maia|12/12/2018|São Paulo|2500|NaN|7500|
|798|3662|HL7348|SmartWatch|3|Maria|Gasperi|10/8/2018|São Paulo|1400|NaN|4200|
|799|3666|HL9962|Android|4|Caio|Cardoso|4/28/2018|São Paulo|3400|NaN|13600|
|800|3669|HL1148|Câmera|2|Ana|Campos|8/6/2018|São Paulo|2100|NaN|4200|
|801|3676|HL8851|Notebook|2|Victor|Ferreira|1/8/2018|São Paulo|3500|NaN|7000|
|802|3682|HL1918|iPhone|4|Luiza|Johnson|6/11/2018|São Paulo|5300|NaN|21200|
|803|3683|HL4379|Televisão|3|Lenon|Fernandes|6/19/2018|São Paulo|2500|NaN|7500|
|804|3684|HL2714|Tablet|2|Anízio|Carvalho|4/22/2018|São Paulo|1600|NaN|3200|
|805|3691|HL1918|iPhone|3|Kim|Ferreira|3/5/2018|São Paulo|5300|NaN|15900|
|806|3692|HL1148|Câmera|3|Maria|Correa|1/21/2018|São Paulo|2100|NaN|6300|
|807|3693|HL1148|Câmera|1|Carolina|Rachide|12/5/2018|São Paulo|2100|NaN|2100|
|808|3695|HL8851|Notebook|2|Nicolas|Monteiro|7/7/2018|São Paulo|3500|NaN|7000|
|809|3697|HL4379|Televisão|1|Camila|Sobral|5/12/2018|São Paulo|2500|NaN|2500|
|810|3700|HL9962|Android|3|Vinícius|Antunes|12/25/2018|São Paulo|3400|NaN|10200|
|811|3704|HL7348|SmartWatch|4|Isabelle|Firmino|9/6/2018|São Paulo|1400|NaN|5600|
|812|3710|HL1918|iPhone|4|Rogério|Gentile|6/1/2018|São Paulo|5300|NaN|21200|
|813|3713|HL1148|Câmera|3|Bárbara|Lima|9/29/2018|São Paulo|2100|NaN|6300|
|814|3720|HL1918|iPhone|3|Breno|Costa|6/21/2018|São Paulo|5300|NaN|15900|
|815|3723|HL2714|Tablet|5|Jônatas|Soares|5/3/2018|São Paulo|1600|NaN|8000|
|816|3729|HL2714|Tablet|2|Beatriz|Rocha|5/22/2018|São Paulo|1600|NaN|3200|
|817|3733|HL4379|Televisão|3|Iuri|Barbosa|5/31/2018|São Paulo|2500|NaN|7500|
|818|3748|HL4379|Televisão|3|Caio|Fernandes|11/11/2018|São Paulo|2500|NaN|7500|
|819|3753|HL4379|Televisão|2|Marcelo|Rosa|10/6/2018|São Paulo|2500|NaN|5000|
|820|3756|HL1148|Câmera|4|Dykson|Silva|3/14/2018|São Paulo|2100|NaN|8400|
|821|3763|HL4379|Televisão|3|Thainá|Binello|5/6/2018|São Paulo|2500|NaN|7500|
|822|3773|HL1918|iPhone|3|Yasmim|Bittencourt|11/13/2018|São Paulo|5300|NaN|15900|
|823|3777|HL7348|SmartWatch|4|Carlos|Araujo|4/15/2018|São Paulo|1400|NaN|5600|
|824|3779|HL1918|iPhone|5|Giselia|Thiele|2/19/2018|São Paulo|5300|NaN|26500|
|825|3781|HL1918|iPhone|1|Juliana|Mesquita|7/15/2018|São Paulo|5300|NaN|5300|
|826|3784|HL1918|iPhone|3|Henrique|Lencastre|5/12/2018|São Paulo|5300|NaN|15900|
|827|3793|HL8851|Notebook|5|Juliana|Mesquita|7/14/2018|São Paulo|3500|NaN|17500|
|828|3796|HL1148|Câmera|3|Thais|Rodrigues|7/16/2018|São Paulo|2100|NaN|6300|
|829|3805|HL2714|Tablet|5|Bruno|Salomão|4/20/2018|São Paulo|1600|NaN|8000|
|830|3809|HL8851|Notebook|2|Breno|Farias|10/23/2018|São Paulo|3500|NaN|7000|
|831|3817|HL4379|Televisão|2|Henrique|Oliveira|4/21/2018|São Paulo|2500|NaN|5000|
|832|3821|HL1918|iPhone|4|Milena|Alcoforado|4/23/2018|São Paulo|5300|NaN|21200|
|833|3827|HL9962|Android|2|Caio|Fernandes|11/9/2018|São Paulo|3400|NaN|6800|
|834|3828|HL1918|iPhone|4|Fernanda|Bhering|6/19/2018|São Paulo|5300|NaN|21200|
|835|3831|HL1918|iPhone|3|Isabel|Leite|1/4/2018|São Paulo|5300|NaN|15900|
|836|3835|HL4379|Televisão|5|Cassio|Faria|7/12/2018|São Paulo|2500|NaN|12500|
|837|3839|HL7348|SmartWatch|3|Hanna|Fonseca|12/7/2018|São Paulo|1400|NaN|4200|
|838|3846|HL1918|iPhone|1|Renan|Firmino|2/25/2018|São Paulo|5300|NaN|5300|
|839|3847|HL1148|Câmera|3|Julia|Teixeira|3/31/2018|São Paulo|2100|NaN|6300|
|840|3851|HL9962|Android|4|Thomaz|Ferreira|5/21/2018|São Paulo|3400|NaN|13600|
|841|3853|HL4379|Televisão|3|Larissa|Nauenberg|12/4/2018|São Paulo|2500|NaN|7500|
|842|3857|HL1918|iPhone|2|Alon|Fahrnholz|3/9/2018|São Paulo|5300|NaN|10600|
|843|3864|HL9962|Android|3|Silvio|Provenzano|1/26/2018|São Paulo|3400|NaN|10200|
|844|3866|HL4379|Televisão|2|Bernardo|Soares|9/11/2018|São Paulo|2500|NaN|5000|
|845|3872|HL1918|iPhone|1|Breno|Britto|4/12/2018|São Paulo|5300|NaN|5300|
|846|3881|HL2714|Tablet|3|Raphael|Machado|2/3/2018|São Paulo|1600|NaN|4800|
|847|3886|HL2714|Tablet|1|Julia|Penteado|9/26/2018|São Paulo|1600|NaN|1600|
|848|3887|HL8851|Notebook|4|Fabio|Sepúlveda|2/1/2018|São Paulo|3500|NaN|14000|
|849|3890|HL1918|iPhone|1|Lucas|Aragão|10/16/2018|São Paulo|5300|NaN|5300|
|850|3892|HL1918|iPhone|2|Rubens|Valente|4/11/2018|São Paulo|5300|NaN|10600|
|851|3895|HL2714|Tablet|3|Lucas|Villanova|8/25/2018|São Paulo|1600|NaN|4800|
|852|3896|HL8851|Notebook|3|Hércules|Júnior|1/19/2018|São Paulo|3500|NaN|10500|
|853|3899|HL9962|Android|3|Karina|Camara|7/11/2018|São Paulo|3400|NaN|10200|
|854|3910|HL1148|Câmera|1|Marcelo|Rosa|2/13/2018|São Paulo|2100|NaN|2100|
|855|3911|HL9962|Android|1|Amanda|Gontijo|5/26/2018|São Paulo|3400|NaN|3400|
|856|3915|HL4379|Televisão|2|Lucas|Rodrigues|6/17/2018|São Paulo|2500|NaN|5000|
|857|3917|HL9962|Android|1|Renan|Nucci|11/10/2018|São Paulo|3400|NaN|3400|
|858|3921|HL1148|Câmera|2|Isabella|Scalabrin|1/19/2018|São Paulo|2100|NaN|4200|
|859|3924|HL1918|iPhone|5|Rogério|Pereira|9/20/2018|São Paulo|5300|NaN|26500|
|860|3930|HL4379|Televisão|4|Gustavo|Accardo|3/16/2018|São Paulo|2500|NaN|10000|
|861|3937|HL9962|Android|1|Paloma|Sperandei|4/22/2018|São Paulo|3400|NaN|3400|
|862|3957|HL4379|Televisão|2|Rafaela|Ferreira|10/4/2018|São Paulo|2500|NaN|5000|
|863|3968|HL1918|iPhone|5|Pedro|Dalforne|4/14/2018|São Paulo|5300|NaN|26500|
|864|3973|HL7348|SmartWatch|4|Bruno|Velucci|8/27/2018|São Paulo|1400|NaN|5600|
|865|3982|HL4379|Televisão|2|Silvio|Fahrnholz|10/28/2018|São Paulo|2500|NaN|5000|
|866|3983|HL8851|Notebook|3|Guilherme|Merotto|10/9/2018|São Paulo|3500|NaN|10500|
|867|3988|HL1148|Câmera|5|João|Oliveira|2/24/2018|São Paulo|2100|NaN|10500|
|868|3995|HL4379|Televisão|3|Henrique|Villanova|6/17/2018|São Paulo|2500|NaN|7500|
|869|4001|HL7348|SmartWatch|5|Rodrigo|Alves|1/8/2018|São Paulo|1400|NaN|7000|
|870|4004|HL1918|iPhone|3|Bianca|Procaci|11/30/2018|São Paulo|5300|NaN|15900|
|871|4009|HL1148|Câmera|3|Henrique|Oliveira|4/23/2018|São Paulo|2100|NaN|6300|
|872|4016|HL4379|Televisão|2|Amanda|Machado|10/30/2018|São Paulo|2500|NaN|5000|
|873|4018|HL9962|Android|2|Carolina|Vasconcelos|6/4/2018|São Paulo|3400|NaN|6800|
|874|4025|HL7348|SmartWatch|5|Carolina|Motta|10/8/2018|São Paulo|1400|NaN|7000|
|875|4026|HL1148|Câmera|3|Bianca|Ferezin|4/2/2018|São Paulo|2100|NaN|6300|
|876|4028|HL9962|Android|1|Jeferson|Costa|5/17/2018|São Paulo|3400|NaN|3400|
|877|4029|HL4379|Televisão|1|Larissa|Nauenberg|1/12/2018|São Paulo|2500|NaN|2500|
|878|4033|HL4379|Televisão|5|Célio|Xavier|3/11/2018|São Paulo|2500|NaN|12500|
|879|4034|HL9962|Android|2|Raphael|Mattos|3/8/2018|São Paulo|3400|NaN|6800|
|880|4046|HL4379|Televisão|2|Mateus|Polastri|8/7/2018|São Paulo|2500|NaN|5000|
|881|4049|HL8851|Notebook|3|Bruno|Ferreira|2/11/2018|São Paulo|3500|NaN|10500|
|882|4058|HL9962|Android|5|Caio|Moraes|4/14/2018|São Paulo|3400|NaN|17000|
|883|4069|HL1148|Câmera|1|Lucas|Fontoura|3/24/2018|São Paulo|2100|NaN|2100|
|884|4071|HL1918|iPhone|1|Priscila|Vogel|12/17/2018|São Paulo|5300|NaN|5300|
|885|4072|HL4379|Televisão|4|Mariana|Freire|2/14/2018|São Paulo|2500|NaN|10000|
|886|4074|HL2714|Tablet|5|Clarissa|Santos|5/9/2018|São Paulo|1600|NaN|8000|
|887|4082|HL9962|Android|1|Wellington|Duarte|2/9/2018|São Paulo|3400|NaN|3400|
|888|4088|HL1918|iPhone|4|Luiz|Conceição|12/6/2018|São Paulo|5300|NaN|21200|
|889|4097|HL2714|Tablet|2|Wen|Braga|1/13/2018|São Paulo|1600|NaN|3200|
|890|4098|HL2714|Tablet|3|Livia|Cozendey|10/5/2018|São Paulo|1600|NaN|4800|
|891|4099|HL1918|iPhone|1|Eduardo|Vargas|12/21/2018|São Paulo|5300|NaN|5300|
|892|4108|HL9962|Android|5|Gabriel|Ribeiro|3/3/2018|São Paulo|3400|NaN|17000|
|893|4119|HL8851|Notebook|3|Guilherme|Barbosa|4/2/2018|São Paulo|3500|NaN|10500|
|894|4127|HL1918|iPhone|3|Eduardo|Pacheco|12/17/2018|São Paulo|5300|NaN|15900|
|895|4147|HL7348|SmartWatch|3|Raul|Silveira|11/18/2018|São Paulo|1400|NaN|4200|
|896|4148|HL9962|Android|4|Hygor|Essaber|10/3/2018|São Paulo|3400|NaN|13600|
|897|4151|HL1918|iPhone|4|Isabel|Mesquita|7/1/2018|São Paulo|5300|NaN|21200|
|898|4154|HL8851|Notebook|2|Rogério|Gentile|2/24/2018|São Paulo|3500|NaN|7000|
|899|4162|HL4379|Televisão|2|Juliana|Pacheco|9/25/2018|São Paulo|2500|NaN|5000|
|900|4163|HL9962|Android|3|Carolina|Costa|3/13/2018|São Paulo|3400|NaN|10200|
|901|4165|HL2714|Tablet|5|Patrick|Silva|8/13/2018|São Paulo|1600|NaN|8000|
|902|4169|HL1918|iPhone|5|Gabriela|Mello|8/7/2018|São Paulo|5300|NaN|26500|
|903|4171|HL7348|SmartWatch|3|Thainá|Binello|5/15/2018|São Paulo|1400|NaN|4200|
|904|4177|HL1918|iPhone|1|João|Peçanha|6/5/2018|São Paulo|5300|NaN|5300|
|905|4178|HL1918|iPhone|4|Joao|Silva|3/22/2018|São Paulo|5300|NaN|21200|
|906|4184|HL1918|iPhone|5|Paulo|Campos|7/31/2018|São Paulo|5300|NaN|26500|
|907|4193|HL2714|Tablet|1|Adrielle|Forte|6/21/2018|São Paulo|1600|NaN|1600|
|908|4195|HL1918|iPhone|2|Marcelo|Guadagnino|2/21/2018|São Paulo|5300|NaN|10600|
|909|4201|HL1918|iPhone|2|Eduardo|Peluzo|8/22/2018|São Paulo|5300|NaN|10600|
|910|4208|HL1918|iPhone|4|Luiza|Marques|12/30/2018|São Paulo|5300|NaN|21200|
|911|4212|HL1918|iPhone|1|Daniel|Sousa|8/10/2018|São Paulo|5300|NaN|5300|
|912|4214|HL1918|iPhone|3|Ana|Michetti|9/28/2018|São Paulo|5300|NaN|15900|
|913|4220|HL1918|iPhone|1|Giuseppe|Borges|5/21/2018|São Paulo|5300|NaN|5300|
|914|4225|HL2714|Tablet|1|Caroline|Delgado|10/18/2018|São Paulo|1600|NaN|1600|
|915|4230|HL1918|iPhone|5|Milena|Alcoforado|10/19/2018|São Paulo|5300|NaN|26500|
|916|4233|HL2714|Tablet|2|Bianca|Paz|4/17/2018|São Paulo|1600|NaN|3200|
|917|4234|HL7348|SmartWatch|3|Fabio|Boccaletti|1/15/2018|São Paulo|1400|NaN|4200|
|918|4237|HL1148|Câmera|3|Vitor|Campos|1/1/2018|São Paulo|2100|NaN|6300|
|919|4238|HL1148|Câmera|2|Lucas|Lima|12/12/2018|São Paulo|2100|NaN|4200|
|920|4239|HL7348|SmartWatch|4|Julia|Teixeira|9/18/2018|São Paulo|1400|NaN|5600|
|921|4244|HL1918|iPhone|2|Bruna|Soares|7/9/2018|São Paulo|5300|NaN|10600|
|922|4253|HL1918|iPhone|1|Bruna|Rangel|7/1/2018|São Paulo|5300|NaN|5300|
|923|4259|HL2714|Tablet|1|Amanda|Procaci|9/13/2018|São Paulo|1600|NaN|1600|
|924|4263|HL4379|Televisão|3|Luíza|Garcia|7/3/2018|São Paulo|2500|NaN|7500|
|925|4272|HL1918|iPhone|2|Mariana|Rotava|7/21/2018|São Paulo|5300|NaN|10600|
|926|4277|HL1918|iPhone|3|Elena|Barreto|8/24/2018|São Paulo|5300|NaN|15900|
|927|4280|HL7348|SmartWatch|5|Raísa|Rodrigues|8/12/2018|São Paulo|1400|NaN|7000|
|928|4282|HL7348|SmartWatch|3|Jeferson|Costa|3/23/2018|São Paulo|1400|NaN|4200|
|929|4283|HL2714|Tablet|4|Luana|Santos|11/14/2018|São Paulo|1600|NaN|6400|
|930|4285|HL7348|SmartWatch|4|Pedro|Ayres|5/10/2018|São Paulo|1400|NaN|5600|
|931|4286|HL9962|Android|4|Gabriel|Thome|1/30/2018|São Paulo|3400|NaN|13600|
|932|4288|HL2714|Tablet|3|Pedro|Bitencourt|12/7/2018|São Paulo|1600|NaN|4800|
|933|4293|HL1148|Câmera|1|Marina|Cormack|4/9/2018|São Paulo|2100|NaN|2100|
|934|4299|HL1148|Câmera|3|Fillipe|Almeida|6/8/2018|São Paulo|2100|NaN|6300|
|935|4301|HL8851|Notebook|5|Julia|Leig|6/29/2018|São Paulo|3500|NaN|17500|
|936|4302|HL4379|Televisão|3|Andreza|Ramos|10/27/2018|São Paulo|2500|NaN|7500|
|937|4307|HL9962|Android|5|Arthur|Fernandes|8/23/2018|São Paulo|3400|NaN|17000|
|938|4315|HL4379|Televisão|5|Caio|Silva|12/23/2018|São Paulo|2500|NaN|12500|
|939|4316|HL1148|Câmera|2|Thiago|Veloso|4/23/2018|São Paulo|2100|NaN|4200|
|940|4319|HL1918|iPhone|4|Rodrigo|Mendes|5/31/2018|São Paulo|5300|NaN|21200|
|941|4331|HL1148|Câmera|5|Pedro|Lyra|2/14/2018|São Paulo|2100|NaN|10500|
|942|4336|HL1918|iPhone|3|Beatriz|Perdomo|1/5/2018|São Paulo|5300|NaN|15900|
|943|4338|HL4379|Televisão|1|Rafaela|Feio|9/29/2018|São Paulo|2500|NaN|2500|
|944|4342|HL8851|Notebook|2|Eduardo|Peluzo|4/3/2018|São Paulo|3500|NaN|7000|
|945|4343|HL1918|iPhone|4|Felipe|Paulo|9/1/2018|São Paulo|5300|NaN|21200|
|946|4356|HL1918|iPhone|3|Ulisses|Quinto|9/29/2018|São Paulo|5300|NaN|15900|
|947|4357|HL4379|Televisão|3|Ian|Almeida|7/17/2018|São Paulo|2500|NaN|7500|
|948|4360|HL4379|Televisão|1|Wilson|Meirelles|3/30/2018|São Paulo|2500|NaN|2500|
|949|4364|HL9962|Android|1|Ana|Felippe|10/19/2018|São Paulo|3400|NaN|3400|
|950|4370|HL1918|iPhone|4|Eduardo|Quindeler|7/11/2018|São Paulo|5300|NaN|21200|
|951|4375|HL8851|Notebook|1|Matheus|Miranda|5/11/2018|São Paulo|3500|NaN|3500|
|952|4389|HL1148|Câmera|2|Wilson|Miranda|1/15/2018|São Paulo|2100|NaN|4200|
|953|4404|HL1148|Câmera|2|João|Capitulo|9/19/2018|São Paulo|2100|NaN|4200|
|954|4407|HL1148|Câmera|3|Eduardo|Pacheco|1/26/2018|São Paulo|2100|NaN|6300|
|955|4408|HL1148|Câmera|2|Jônatas|Soares|12/30/2018|São Paulo|2100|NaN|4200|
|956|4410|HL9962|Android|5|Rachel|Silva|6/4/2018|São Paulo|3400|NaN|17000|
|957|4416|HL1148|Câmera|3|Sandy|Figueiredo|10/25/2018|São Paulo|2100|NaN|6300|
|958|4423|HL8851|Notebook|3|Juliana|Goes|4/19/2018|São Paulo|3500|NaN|10500|
|959|4426|HL7348|SmartWatch|1|Luiza|Marques|6/15/2018|São Paulo|1400|NaN|1400|
|960|4427|HL2714|Tablet|4|Julia|Penteado|7/14/2018|São Paulo|1600|NaN|6400|
|961|4433|HL4379|Televisão|4|Thais|Rodrigues|1/4/2018|São Paulo|2500|NaN|10000|
|962|4435|HL1918|iPhone|2|Victor|Soares|11/29/2018|São Paulo|5300|NaN|10600|
|963|4437|HL4379|Televisão|3|Stefan|Santos|6/10/2018|São Paulo|2500|NaN|7500|
|964|4438|HL4379|Televisão|4|Bernard|Pedrosa|8/29/2018|São Paulo|2500|NaN|10000|
|965|4443|HL1918|iPhone|2|Kim|Ferreira|7/6/2018|São Paulo|5300|NaN|10600|
|966|4450|HL1918|iPhone|4|Matheus|Gomes|11/25/2018|São Paulo|5300|NaN|21200|
|967|4451|HL1918|iPhone|2|Bárbara|Cavalcante|9/22/2018|São Paulo|5300|NaN|10600|
|968|4455|HL2714|Tablet|5|Thayane|Resende|11/24/2018|São Paulo|1600|NaN|8000|
|969|4460|HL1918|iPhone|2|Livia|Codeceira|3/13/2018|São Paulo|5300|NaN|10600|
|970|4472|HL1918|iPhone|4|Eduardo|Ferreira|2/18/2018|São Paulo|5300|NaN|21200|
|971|4475|HL2714|Tablet|3|Tayla|Lima|8/31/2018|São Paulo|1600|NaN|4800|
|972|4484|HL1148|Câmera|5|Vanessa|Rodrigues|10/16/2018|São Paulo|2100|NaN|10500|
|973|4487|HL8851|Notebook|4|Wilson|Meirelles|6/15/2018|São Paulo|3500|NaN|14000|
|974|4488|HL1918|iPhone|2|Mariana|Baptista|10/2/2018|São Paulo|5300|NaN|10600|
|975|4493|HL4379|Televisão|4|Michelle|Pereira|6/9/2018|São Paulo|2500|NaN|10000|
|976|4495|HL1148|Câmera|2|Tadeu|Sousa|7/16/2018|São Paulo|2100|NaN|4200|
|977|4497|HL4379|Televisão|4|Priscila|Garcia|11/11/2018|São Paulo|2500|NaN|10000|
|978|4501|HL4379|Televisão|5|Rafaella|Mello|3/18/2018|São Paulo|2500|NaN|12500|
|979|4503|HL7348|SmartWatch|3|Fernanda|Rubim|10/8/2018|São Paulo|1400|NaN|4200|
|980|4508|HL4379|Televisão|3|David|Assumpção|9/11/2018|São Paulo|2500|NaN|7500|
|981|4515|HL9962|Android|4|Danilo|Alves|9/8/2018|São Paulo|3400|NaN|13600|
|982|4518|HL1918|iPhone|1|Marina|Delgado|10/2/2018|São Paulo|5300|NaN|5300|
|983|4525|HL4379|Televisão|1|Wen|Braga|2/4/2018|São Paulo|2500|NaN|2500|
|984|4529|HL9962|Android|4|Carolina|Brum|2/4/2018|São Paulo|3400|NaN|13600|
|985|4537|HL1918|iPhone|4|Ulisses|Quinto|4/5/2018|São Paulo|5300|NaN|21200|
|986|4538|HL8851|Notebook|4|Gabriella|Lopes|11/23/2018|São Paulo|3500|NaN|14000|
|987|4543|HL4379|Televisão|5|Daniel|Monteiro|3/5/2018|São Paulo|2500|NaN|12500|
|988|4544|HL7348|SmartWatch|5|Thales|Santos|1/23/2018|São Paulo|1400|NaN|7000|
|989|4550|HL8851|Notebook|5|Laura|Araujo|4/17/2018|São Paulo|3500|NaN|17500|
|990|4551|HL1918|iPhone|5|Felipe|Cavalcanti|6/9/2018|São Paulo|5300|NaN|26500|
|991|4552|HL4379|Televisão|3|Leandro|Rodrigues|5/19/2018|São Paulo|2500|NaN|7500|
|992|4558|HL1918|iPhone|4|Pedro|Conceição|7/30/2018|São Paulo|5300|NaN|21200|
|993|4574|HL4379|Televisão|5|Ulisses|Filho|10/1/2018|São Paulo|2500|NaN|12500|
|994|4575|HL1918|iPhone|4|Arthur|Fernandes|10/27/2018|São Paulo|5300|NaN|21200|
|995|4577|HL1918|iPhone|4|Jessica|Ferreira|5/27/2018|São Paulo|5300|NaN|21200|
|996|4583|HL4379|Televisão|5|Isabella|Rodrigues|2/5/2018|São Paulo|2500|NaN|12500|
|997|4586|HL1918|iPhone|5|Pedro|Oliveira|2/6/2018|São Paulo|5300|NaN|26500|
|998|4588|HL1148|Câmera|5|Adrielle|Gabriel|11/26/2018|São Paulo|2100|NaN|10500|
|999|4590|HL1148|Câmera|1|Ana|Leite|12/31/2018|São Paulo|2100|NaN|2100|
|1000|4592|HL4379|Televisão|5|João|Costa|1/28/2018|São Paulo|2500|NaN|12500|
|1001|4595|HL1918|iPhone|1|Matheus|Sapir|8/21/2018|São Paulo|5300|NaN|5300|
|1002|4598|HL1918|iPhone|2|Renan|Nascimento|4/19/2018|São Paulo|5300|NaN|10600|
|1003|4612|HL4379|Televisão|2|Rafaela|Rodrigues|1/22/2018|São Paulo|2500|NaN|5000|
|1004|4613|HL1148|Câmera|1|Wen|Braga|8/23/2018|São Paulo|2100|NaN|2100|
|1005|4619|HL1918|iPhone|2|Priscila|Suzano|1/19/2018|São Paulo|5300|NaN|10600|
|1006|4622|HL4379|Televisão|1|Caio|Fernandes|6/3/2018|São Paulo|2500|NaN|2500|
|1007|4632|HL4379|Televisão|2|Bruna|Londero|6/26/2018|São Paulo|2500|NaN|5000|
|1008|4637|HL2714|Tablet|1|Rafael|Portela|5/1/2018|São Paulo|1600|NaN|1600|
|1009|4643|HL1148|Câmera|1|Lenon|Fernandes|6/1/2018|São Paulo|2100|NaN|2100|
|1010|4659|HL1918|iPhone|5|Thomáz|Bôas|9/18/2018|São Paulo|5300|NaN|26500|
|1011|4661|HL2714|Tablet|1|Manuela|Merege|6/18/2018|São Paulo|1600|NaN|1600|
|1012|4663|HL1148|Câmera|1|Gabrielle|Wanderley|3/22/2018|São Paulo|2100|NaN|2100|
|1013|4667|HL4379|Televisão|4|Carolina|Costa|8/3/2018|São Paulo|2500|NaN|10000|
|1014|4678|HL9962|Android|4|Gabrielle|Viríssimo|7/6/2018|São Paulo|3400|NaN|13600|
|1015|4683|HL8851|Notebook|2|Sthefeson|Barroso|12/15/2018|São Paulo|3500|NaN|7000|
|1016|4685|HL4379|Televisão|5|Catarina|Teixeira|1/27/2018|São Paulo|2500|NaN|12500|
|1017|4688|HL1918|iPhone|4|Bruno|Velucci|9/2/2018|São Paulo|5300|NaN|21200|
|1018|4691|HL7348|SmartWatch|4|Raissa|Negrelli|2/11/2018|São Paulo|1400|NaN|5600|
|1019|4692|HL1918|iPhone|2|Júlio|Fraga|1/23/2018|São Paulo|5300|NaN|10600|
|1020|4699|HL7348|SmartWatch|3|Victor|Lira|4/8/2018|São Paulo|1400|NaN|4200|
|1021|4700|HL1148|Câmera|4|Izabel|Lopes|6/22/2018|São Paulo|2100|NaN|8400|
|1022|4701|HL2714|Tablet|2|Rafael|Rocha|1/17/2018|São Paulo|1600|NaN|3200|
|1023|4706|HL1148|Câmera|1|Aline|Mello|2/25/2018|São Paulo|2100|NaN|2100|
|1024|4709|HL7348|SmartWatch|5|Mariana|Rotava|6/17/2018|São Paulo|1400|NaN|7000|
|1025|4711|HL7348|SmartWatch|4|Raissa|Pinheiro|12/20/2018|São Paulo|1400|NaN|5600|
|1026|4714|HL7348|SmartWatch|5|Débora|Lopes|9/11/2018|São Paulo|1400|NaN|7000|
|1027|4724|HL8851|Notebook|3|Fillipe|Almeida|5/31/2018|São Paulo|3500|NaN|10500|
|1028|4726|HL7348|SmartWatch|4|João|Guadagnino|3/31/2018|São Paulo|1400|NaN|5600|
|1029|4728|HL1918|iPhone|4|Carlos|Azevedo|3/1/2018|São Paulo|5300|NaN|21200|
|1030|4730|HL4379|Televisão|2|Thomáz|Rodriguez|8/4/2018|São Paulo|2500|NaN|5000|
|1031|4734|HL2714|Tablet|3|Ravena|Bhering|10/2/2018|São Paulo|1600|NaN|4800|
|1032|4737|HL7348|SmartWatch|1|Ana|Gomes|10/24/2018|São Paulo|1400|NaN|1400|
|1033|4747|HL2714|Tablet|1|Rilson|Dias|7/10/2018|São Paulo|1600|NaN|1600|
|1034|4751|HL2714|Tablet|1|Larissa|Nauenberg|6/6/2018|São Paulo|1600|NaN|1600|
|1035|4768|HL8851|Notebook|1|Antonio|Manhães|7/23/2018|São Paulo|3500|NaN|3500|
|1036|4769|HL1918|iPhone|1|Paloma|Sperandei|8/11/2018|São Paulo|5300|NaN|5300|
|1037|4776|HL9962|Android|3|Joyce|Souza|6/24/2018|São Paulo|3400|NaN|10200|
|1038|4778|HL4379|Televisão|4|Mariana|Rotava|2/25/2018|São Paulo|2500|NaN|10000|
|1039|4780|HL1148|Câmera|1|Pedro|Lyra|8/14/2018|São Paulo|2100|NaN|2100|
|1040|4789|HL8851|Notebook|2|Adriane|Chagas|8/5/2018|São Paulo|3500|NaN|7000|
|1041|4808|HL2714|Tablet|3|João|Junior|5/15/2018|São Paulo|1600|NaN|4800|
|1042|4812|HL2714|Tablet|1|Igor|Azevedo|8/8/2018|São Paulo|1600|NaN|1600|
|1043|4813|HL1918|iPhone|1|Marina|Miranda|6/27/2018|São Paulo|5300|NaN|5300|
|1044|4823|HL1918|iPhone|1|Eduardo|Lopes|11/19/2018|São Paulo|5300|NaN|5300|
|1045|4826|HL1918|iPhone|4|Guilherme|Lima|4/29/2018|São Paulo|5300|NaN|21200|
|1046|4830|HL1918|iPhone|5|Silvio|Fahrnholz|11/19/2018|São Paulo|5300|NaN|26500|
|1047|4836|HL7348|SmartWatch|2|Ives|Barbosa|2/14/2018|São Paulo|1400|NaN|2800|
|1048|4855|HL9962|Android|4|Adriana|Carneiro|10/22/2018|São Paulo|3400|NaN|13600|
|1049|4869|HL4379|Televisão|3|Eduardo|Silva|7/30/2018|São Paulo|2500|NaN|7500|
|1050|4870|HL9962|Android|5|Rodrigo|Ramos|1/28/2018|São Paulo|3400|NaN|17000|
|1051|4871|HL1918|iPhone|1|Bruna|Silva|7/18/2018|São Paulo|5300|NaN|5300|
|1052|4874|HL4379|Televisão|2|Giuseppe|Borges|4/15/2018|São Paulo|2500|NaN|5000|
|1053|4879|HL1918|iPhone|2|Felipe|Paulo|12/4/2018|São Paulo|5300|NaN|10600|
|1054|4881|HL4379|Televisão|5|Rodrigo|Feijo|10/15/2018|São Paulo|2500|NaN|12500|
|1055|4901|HL1918|iPhone|1|Carlos|Cardoso|6/14/2018|São Paulo|5300|NaN|5300|
|1056|4904|HL8851|Notebook|5|Thiago|Costa|3/15/2018|São Paulo|3500|NaN|17500|
|1057|4911|HL7348|SmartWatch|2|Carlos|Assis|12/23/2018|São Paulo|1400|NaN|2800|
|1058|4912|HL1918|iPhone|5|Lucas|Baptista|7/21/2018|São Paulo|5300|NaN|26500|
|1059|4913|HL1148|Câmera|2|Beatriz|Santos|2/23/2018|São Paulo|2100|NaN|4200|
|1060|4914|HL9962|Android|3|Wellington|Duarte|8/4/2018|São Paulo|3400|NaN|10200|
|1061|4922|HL2714|Tablet|3|Clara|Silveira|8/30/2018|São Paulo|1600|NaN|4800|
|1062|4923|HL1918|iPhone|2|Rogério|Pereira|1/16/2018|São Paulo|5300|NaN|10600|
|1063|4926|HL7348|SmartWatch|2|Bruno|Souza|6/21/2018|São Paulo|1400|NaN|2800|
|1064|4929|HL1148|Câmera|2|Antônio|Oliveira|4/5/2018|São Paulo|2100|NaN|4200|
|1065|4931|HL4379|Televisão|5|Guilherme|Lima|2/18/2018|São Paulo|2500|NaN|12500|
|1066|4934|HL1918|iPhone|5|Daniel|Cardoso|10/21/2018|São Paulo|5300|NaN|26500|
|1067|4935|HL7348|SmartWatch|5|Thomáz|Bôas|8/8/2018|São Paulo|1400|NaN|7000|
|1068|4947|HL1918|iPhone|2|Ana|Fioretti|2/22/2018|São Paulo|5300|NaN|10600|
|1069|4961|HL8851|Notebook|2|João|Monteiro|4/25/2018|São Paulo|3500|NaN|7000|
|1070|4964|HL9962|Android|4|Isabela|Resende|4/20/2018|São Paulo|3400|NaN|13600|
|1071|4968|HL1918|iPhone|1|Anderson|Barreto|7/16/2018|São Paulo|5300|NaN|5300|
|1072|4971|HL1918|iPhone|5|Lucas|Lemos|8/16/2018|São Paulo|5300|NaN|26500|
|1073|4972|HL1148|Câmera|1|Iuri|Barbosa|3/29/2018|São Paulo|2100|NaN|2100|
|1074|4974|HL9962|Android|3|Caroline|Aquino|7/2/2018|São Paulo|3400|NaN|10200|
|1075|4980|HL8851|Notebook|3|Guilherme|Vianna|10/23/2018|São Paulo|3500|NaN|10500|
|1076|4982|HL4379|Televisão|3|Daniel|Monteiro|6/21/2018|São Paulo|2500|NaN|7500|
|1077|4992|HL7348|SmartWatch|5|Carolina|Brum|8/18/2018|São Paulo|1400|NaN|7000|
|1078|4998|HL9962|Android|5|João|Capitulo|4/24/2018|São Paulo|3400|NaN|17000|
|1079|4999|HL8851|Notebook|4|Barbara|Procaci|4/6/2018|São Paulo|3500|NaN|14000|
|1080|5003|HL1918|iPhone|1|Livia|Codeceira|12/31/2018|São Paulo|5300|NaN|5300|
|1081|5005|HL9962|Android|3|Arthur|Pereira|10/10/2018|São Paulo|3400|NaN|10200|
|1082|5011|HL9962|Android|4|Wilson|Meirelles|3/1/2018|São Paulo|3400|NaN|13600|
|1083|5012|HL7348|SmartWatch|1|Gabriel|Rubim|1/21/2018|São Paulo|1400|NaN|1400|
|1084|5013|HL1918|iPhone|4|Lucas|Junior|7/28/2018|São Paulo|5300|NaN|21200|
|1085|5017|HL8851|Notebook|1|Diogo|Peixoto|7/3/2018|São Paulo|3500|NaN|3500|
|1086|5018|HL7348|SmartWatch|3|Caio|Moraes|9/25/2018|São Paulo|1400|NaN|4200|
|1087|5026|HL1148|Câmera|1|Thomáz|Bôas|12/28/2018|São Paulo|2100|NaN|2100|
|1088|5027|HL1148|Câmera|5|Raíssa|Oros|2/12/2018|São Paulo|2100|NaN|10500|
|1089|5029|HL4379|Televisão|4|José|Seixas|5/21/2018|São Paulo|2500|NaN|10000|
|1090|5031|HL9962|Android|3|Marina|Mesquita|6/21/2018|São Paulo|3400|NaN|10200|
|1091|5032|HL4379|Televisão|2|Renan|Melo|2/4/2018|São Paulo|2500|NaN|5000|
|1092|5033|HL1918|iPhone|4|Carlos|Melo|1/16/2018|São Paulo|5300|NaN|21200|
|1093|5038|HL1148|Câmera|1|Lucas|Lima|12/14/2018|São Paulo|2100|NaN|2100|
|1094|5039|HL8851|Notebook|5|Jorge|Carvalho|8/31/2018|São Paulo|3500|NaN|17500|
|1095|5041|HL7348|SmartWatch|2|Victor|Corrêa|7/7/2018|São Paulo|1400|NaN|2800|
|1096|5044|HL7348|SmartWatch|1|Bruno|Velucci|4/24/2018|São Paulo|1400|NaN|1400|
|1097|5046|HL7348|SmartWatch|4|Rogério|Pereira|3/3/2018|São Paulo|1400|NaN|5600|
|1098|5052|HL1918|iPhone|3|Matheus|Delgado|8/17/2018|São Paulo|5300|NaN|15900|
|1099|5053|HL4379|Televisão|5|Henrique|Lencastre|6/19/2018|São Paulo|2500|NaN|12500|
|1100|5057|HL2714|Tablet|3|Ana|Leite|4/29/2018|São Paulo|1600|NaN|4800|
|1101|5061|HL1918|iPhone|3|Vanessa|Neves|9/11/2018|São Paulo|5300|NaN|15900|
|1102|5062|HL7348|SmartWatch|3|Matheus|Delgado|5/18/2018|São Paulo|1400|NaN|4200|
|1103|5066|HL7348|SmartWatch|4|Roberta|Pimenta|12/13/2018|São Paulo|1400|NaN|5600|
|1104|5067|HL1918|iPhone|4|Daniel|Terra|12/23/2018|São Paulo|5300|NaN|21200|
|1105|5068|HL1148|Câmera|1|Letícia|Leal|7/26/2018|São Paulo|2100|NaN|2100|
|1106|5069|HL1918|iPhone|5|Monique|Vasconcelos|11/12/2018|São Paulo|5300|NaN|26500|
|1107|5075|HL1918|iPhone|3|Raíssa|Oros|2/19/2018|São Paulo|5300|NaN|15900|
|1108|5082|HL1918|iPhone|2|Matheus|Figueiredo|5/26/2018|São Paulo|5300|NaN|10600|
|1109|5085|HL1918|iPhone|5|Natalia|Andrade|10/14/2018|São Paulo|5300|NaN|26500|
|1110|5091|HL9962|Android|2|Daniel|Alcoforado|4/15/2018|São Paulo|3400|NaN|6800|
|1111|5097|HL1918|iPhone|1|Gabriel|Thome|5/13/2018|São Paulo|5300|NaN|5300|
|1112|5108|HL7348|SmartWatch|1|Bruno|Freitas|11/22/2018|São Paulo|1400|NaN|1400|
|1113|5113|HL1148|Câmera|1|Daniela|Pereira|2/1/2018|São Paulo|2100|NaN|2100|
|1114|5121|HL9962|Android|3|Débora|Lopes|5/17/2018|São Paulo|3400|NaN|10200|
|1115|5128|HL4379|Televisão|5|Bruno|Silva|10/25/2018|São Paulo|2500|NaN|12500|
|1116|5132|HL1148|Câmera|3|Lucas|Destri|11/23/2018|São Paulo|2100|NaN|6300|
|1117|5133|HL4379|Televisão|5|Carolina|Costa|2/27/2018|São Paulo|2500|NaN|12500|
|1118|5134|HL1918|iPhone|4|Daniel|Araujo|3/3/2018|São Paulo|5300|NaN|21200|
|1119|5141|HL1918|iPhone|3|Breno|Caputo|2/22/2018|São Paulo|5300|NaN|15900|
|1120|5143|HL1918|iPhone|3|Pedro|Santana|1/24/2018|São Paulo|5300|NaN|15900|
|1121|5144|HL7348|SmartWatch|2|Felipe|Freitas|4/2/2018|São Paulo|1400|NaN|2800|
|1122|5151|HL1918|iPhone|4|Amanda|Amaral|10/8/2018|São Paulo|5300|NaN|21200|
|1123|5155|HL7348|SmartWatch|2|Anna|Maia|11/12/2018|São Paulo|1400|NaN|2800|
|1124|5157|HL7348|SmartWatch|3|Patrícia|Fernandes|6/23/2018|São Paulo|1400|NaN|4200|
|1125|5160|HL8851|Notebook|2|Ives|Barbosa|4/1/2018|São Paulo|3500|NaN|7000|
|1126|5171|HL8851|Notebook|5|Gabriella|Sagrillo|5/11/2018|São Paulo|3500|NaN|17500|
|1127|5172|HL9962|Android|5|Ana|Carvalho|9/22/2018|São Paulo|3400|NaN|17000|
|1128|5173|HL4379|Televisão|5|Luiz|Marinho|10/5/2018|São Paulo|2500|NaN|12500|
|1129|5179|HL1918|iPhone|2|Tayla|Lima|3/23/2018|São Paulo|5300|NaN|10600|
|1130|5185|HL1918|iPhone|1|Stephanie|Oliveira|6/10/2018|São Paulo|5300|NaN|5300|
|1131|5188|HL7348|SmartWatch|5|Carla|Zakhm|11/11/2018|São Paulo|1400|NaN|7000|
|1132|5192|HL4379|Televisão|2|Maria|Junior|11/28/2018|São Paulo|2500|NaN|5000|
|1133|5197|HL4379|Televisão|3|Júlio|Freire|8/18/2018|São Paulo|2500|NaN|7500|
|1134|5209|HL7348|SmartWatch|2|Carolina|Alfradique|12/3/2018|São Paulo|1400|NaN|2800|
|1135|5211|HL1918|iPhone|2|Maria|Junior|6/11/2018|São Paulo|5300|NaN|10600|
|1136|5216|HL1918|iPhone|1|Anderson|Martins|8/27/2018|São Paulo|5300|NaN|5300|
|1137|5218|HL2714|Tablet|1|Hygor|Essaber|2/2/2018|São Paulo|1600|NaN|1600|
|1138|5219|HL1918|iPhone|2|Joao|Silva|10/20/2018|São Paulo|5300|NaN|10600|
|1139|5225|HL4379|Televisão|4|Lucas|Cavalcanti|12/1/2018|São Paulo|2500|NaN|10000|
|1140|5229|HL4379|Televisão|1|Beatriz|Nogueira|7/30/2018|São Paulo|2500|NaN|2500|
|1141|5233|HL9962|Android|3|Wilson|Farias|5/9/2018|São Paulo|3400|NaN|10200|
|1142|5237|HL7348|SmartWatch|2|Rafaela|Rodrigues|10/24/2018|São Paulo|1400|NaN|2800|
|1143|5242|HL2714|Tablet|4|Guilherme|Castilho|9/25/2018|São Paulo|1600|NaN|6400|
|1144|5243|HL1918|iPhone|1|Lucas|Villanova|5/13/2018|São Paulo|5300|NaN|5300|
|1145|5245|HL1918|iPhone|2|Isabella|Montanholi|4/21/2018|São Paulo|5300|NaN|10600|
|1146|5253|HL1918|iPhone|3|Michelle|Figueiredo|4/17/2018|São Paulo|5300|NaN|15900|
|1147|5258|HL1148|Câmera|5|Eduardo|Quindeler|10/30/2018|São Paulo|2100|NaN|10500|
|1148|5259|HL4379|Televisão|2|Joana|Calmon|8/8/2018|São Paulo|2500|NaN|5000|
|1149|5268|HL7348|SmartWatch|1|Amanda|Braga|4/20/2018|São Paulo|1400|NaN|1400|
|1150|5278|HL1918|iPhone|3|Sandy|Figueiredo|10/13/2018|São Paulo|5300|NaN|15900|
|1151|5282|HL8851|Notebook|5|Lucas|Chagas|11/13/2018|São Paulo|3500|NaN|17500|
|1152|5286|HL1918|iPhone|1|Camilla|Guimarães|1/14/2018|São Paulo|5300|NaN|5300|
|1153|5288|HL4379|Televisão|2|Julia|Leite|9/10/2018|São Paulo|2500|NaN|5000|
|1154|5294|HL1918|iPhone|2|Diego|Mello|10/15/2018|São Paulo|5300|NaN|10600|
|1155|5296|HL1918|iPhone|5|Thomaz|Ferreira|1/22/2018|São Paulo|5300|NaN|26500|
|1156|5299|HL7348|SmartWatch|1|Roberta|Pimenta|1/20/2018|São Paulo|1400|NaN|1400|
|1157|5303|HL9962|Android|4|Carlos|Azevedo|6/10/2018|São Paulo|3400|NaN|13600|
|1158|5304|HL1918|iPhone|5|Giulia|Lopes|8/13/2018|São Paulo|5300|NaN|26500|
|1159|5305|HL8851|Notebook|5|Luiza|Cabral|3/22/2018|São Paulo|3500|NaN|17500|
|1160|5306|HL2714|Tablet|1|Marcelo|Pereira|3/1/2018|São Paulo|1600|NaN|1600|
|1161|5321|HL1918|iPhone|1|Bruno|Silva|11/14/2018|São Paulo|5300|NaN|5300|
|1162|5322|HL4379|Televisão|3|José|Vieira|3/7/2018|São Paulo|2500|NaN|7500|
|1163|5324|HL2714|Tablet|5|Bernardo|Nauenberg|7/16/2018|São Paulo|1600|NaN|8000|
|1164|5325|HL4379|Televisão|2|Célio|Xavier|1/6/2018|São Paulo|2500|NaN|5000|
|1165|5326|HL4379|Televisão|4|Katharina|Barros|9/28/2018|São Paulo|2500|NaN|10000|
|1166|5329|HL1918|iPhone|1|Mayara|Soares|5/31/2018|São Paulo|5300|NaN|5300|
|1167|5334|HL1918|iPhone|3|Philipe|Morete|10/15/2018|São Paulo|5300|NaN|15900|
|1168|5343|HL1918|iPhone|2|Pedro|Lyra|12/6/2018|São Paulo|5300|NaN|10600|
|1169|5346|HL1918|iPhone|4|Anderson|Martins|1/29/2018|São Paulo|5300|NaN|21200|
|1170|5347|HL4379|Televisão|1|Izabel|Miura|6/14/2018|São Paulo|2500|NaN|2500|
|1171|5351|HL9962|Android|3|Daniel|Terra|12/29/2018|São Paulo|3400|NaN|10200|
|1172|5354|HL1918|iPhone|4|Marcelo|Pereira|5/11/2018|São Paulo|5300|NaN|21200|
|1173|5356|HL1918|iPhone|3|Bruno|Mota|11/16/2018|São Paulo|5300|NaN|15900|
|1174|5357|HL1918|iPhone|1|Lucas|Junior|3/29/2018|São Paulo|5300|NaN|5300|
|1175|5366|HL8851|Notebook|4|Audir|Franco|11/28/2018|São Paulo|3500|NaN|14000|
|1176|5369|HL1918|iPhone|2|Luiz|Limp|3/19/2018|São Paulo|5300|NaN|10600|
|1177|5370|HL4379|Televisão|4|Thayna|Martins|11/30/2018|São Paulo|2500|NaN|10000|
|1178|5372|HL9962|Android|5|João|Pedrazza|10/12/2018|São Paulo|3400|NaN|17000|
|1179|5373|HL1918|iPhone|1|Bárbara|Lima|10/30/2018|São Paulo|5300|NaN|5300|
|1180|5380|HL4379|Televisão|3|Dandara|Reis|12/2/2018|São Paulo|2500|NaN|7500|
|1181|5381|HL2714|Tablet|3|Roberto|Mattos|8/20/2018|São Paulo|1600|NaN|4800|
|1182|5382|HL1148|Câmera|5|Roberta|Pimenta|9/26/2018|São Paulo|2100|NaN|10500|
|1183|5389|HL1918|iPhone|3|Amanda|Braga|8/14/2018|São Paulo|5300|NaN|15900|
|1184|5413|HL4379|Televisão|4|Lucas|Chagas|7/23/2018|São Paulo|2500|NaN|10000|
|1185|5414|HL7348|SmartWatch|2|Juliana|Correa|12/16/2018|São Paulo|1400|NaN|2800|
|1186|5420|HL1918|iPhone|1|Anderson|Barreto|8/27/2018|São Paulo|5300|NaN|5300|
|1187|5423|HL4379|Televisão|4|Bruna|Rosa|4/9/2018|São Paulo|2500|NaN|10000|
|1188|5425|HL2714|Tablet|5|João|Aires|12/7/2018|São Paulo|1600|NaN|8000|
|1189|5437|HL8851|Notebook|2|Rubens|Netto|10/30/2018|São Paulo|3500|NaN|7000|
|1190|5444|HL7348|SmartWatch|4|Guilherme|Lima|6/13/2018|São Paulo|1400|NaN|5600|
|1191|5448|HL9962|Android|4|Anna|Maia|1/28/2018|São Paulo|3400|NaN|13600|
|1192|5452|HL1918|iPhone|2|Juan|Fernandes|9/18/2018|São Paulo|5300|NaN|10600|
|1193|5455|HL1148|Câmera|2|Marcelo|Magalhães|8/25/2018|São Paulo|2100|NaN|4200|
|1194|5456|HL1918|iPhone|5|Andreza|Ramos|4/15/2018|São Paulo|5300|NaN|26500|
|1195|5458|HL1918|iPhone|1|Luis|Garcia|7/15/2018|São Paulo|5300|NaN|5300|
|1196|5492|HL9962|Android|1|Carlos|Assis|9/7/2018|São Paulo|3400|NaN|3400|
|1197|5493|HL8851|Notebook|4|Wen|Braga|1/3/2018|São Paulo|3500|NaN|14000|
|1198|5495|HL1148|Câmera|5|Fernanda|Bhering|1/16/2018|São Paulo|2100|NaN|10500|
|1199|5506|HL2714|Tablet|1|Sylvio|Bernhardt|8/20/2018|São Paulo|1600|NaN|1600|
|1200|5507|HL1148|Câmera|2|Hiaiune|Valim|6/2/2018|São Paulo|2100|NaN|4200|
|1201|5509|HL1918|iPhone|1|Felipe|Cavalcanti|4/4/2018|São Paulo|5300|NaN|5300|
|1202|5511|HL1918|iPhone|5|Laís|Oliveira|5/13/2018|São Paulo|5300|NaN|26500|
|1203|5518|HL1918|iPhone|1|João|Costa|10/24/2018|São Paulo|5300|NaN|5300|
|1204|5519|HL9962|Android|3|Bruna|Brandao|6/27/2018|São Paulo|3400|NaN|10200|
|1205|5524|HL2714|Tablet|2|Wilson|Vianna|8/6/2018|São Paulo|1600|NaN|3200|
|1206|5526|HL7348|SmartWatch|1|João|Capitulo|2/23/2018|São Paulo|1400|NaN|1400|
|1207|5529|HL1918|iPhone|4|Luiza|Cabral|1/19/2018|São Paulo|5300|NaN|21200|
|1208|5531|HL8851|Notebook|4|Barbara|Procaci|4/19/2018|São Paulo|3500|NaN|14000|
|1209|5535|HL8851|Notebook|4|Tadeu|Nakayama|12/11/2018|São Paulo|3500|NaN|14000|
|1210|5536|HL1918|iPhone|4|Camille|Silva|10/1/2018|São Paulo|5300|NaN|21200|
|1211|5537|HL1148|Câmera|3|Lucas|Lima|4/15/2018|São Paulo|2100|NaN|6300|
|1212|5538|HL1918|iPhone|3|Paloma|Sperandei|1/26/2018|São Paulo|5300|NaN|15900|
|1213|5539|HL8851|Notebook|5|Luis|Silva|4/29/2018|São Paulo|3500|NaN|17500|
|1214|5540|HL9962|Android|3|Allan|Guedes|11/3/2018|São Paulo|3400|NaN|10200|
|1215|5550|HL8851|Notebook|3|Iuri|Neto|7/7/2018|São Paulo|3500|NaN|10500|
|1216|5551|HL4379|Televisão|5|Ana|Gonzaga|1/21/2018|São Paulo|2500|NaN|12500|
|1217|5552|HL9962|Android|2|Desirée|Heimlich|2/17/2018|São Paulo|3400|NaN|6800|
|1218|5555|HL4379|Televisão|3|Mateus|Franco|3/30/2018|São Paulo|2500|NaN|7500|
|1219|5559|HL9962|Android|2|Michelle|Pereira|5/9/2018|São Paulo|3400|NaN|6800|
|1220|5565|HL2714|Tablet|4|Caroline|Cavalcanti|4/23/2018|São Paulo|1600|NaN|6400|
|1221|5568|HL1918|iPhone|3|Beatriz|Santos|11/7/2018|São Paulo|5300|NaN|15900|
|1222|5569|HL8851|Notebook|3|Livia|Corrêa|1/10/2018|São Paulo|3500|NaN|10500|
|1223|5574|HL1918|iPhone|3|Raíssa|Oros|6/2/2018|São Paulo|5300|NaN|15900|
|1224|5575|HL2714|Tablet|5|Beatriz|Santos|9/29/2018|São Paulo|1600|NaN|8000|
|1225|5586|HL1918|iPhone|3|Victor|Magalhães|4/25/2018|São Paulo|5300|NaN|15900|
|1226|5588|HL9962|Android|2|Larissa|Florim|5/5/2018|São Paulo|3400|NaN|6800|
|1227|5589|HL7348|SmartWatch|5|Wilson|Vianna|5/30/2018|São Paulo|1400|NaN|7000|
|1228|5592|HL1148|Câmera|2|Julia|Silva|7/1/2018|São Paulo|2100|NaN|4200|
|1229|5600|HL2714|Tablet|2|Rafaela|Gomes|4/16/2018|São Paulo|1600|NaN|3200|
|1230|5602|HL7348|SmartWatch|1|Lucas|Coelho|7/16/2018|São Paulo|1400|NaN|1400|
|1231|5603|HL1918|iPhone|5|Carolina|Rocha|7/28/2018|São Paulo|5300|NaN|26500|
|1232|5606|HL1918|iPhone|4|Andressa|Chou|1/1/2018|São Paulo|5300|NaN|21200|
|1233|5614|HL1918|iPhone|4|Sthefeson|Pereira|9/2/2018|São Paulo|5300|NaN|21200|
|1234|5615|HL1148|Câmera|1|Paloma|Sperandei|10/11/2018|São Paulo|2100|NaN|2100|
|1235|5616|HL7348|SmartWatch|1|Wilson|Vianna|3/11/2018|São Paulo|1400|NaN|1400|
|1236|5623|HL1918|iPhone|4|Rubens|Valente|1/18/2018|São Paulo|5300|NaN|21200|
|1237|5636|HL4379|Televisão|2|Rafaela|Ferreira|12/7/2018|São Paulo|2500|NaN|5000|
|1238|5656|HL9962|Android|1|Kim|Ferreira|2/3/2018|São Paulo|3400|NaN|3400|
|1239|5657|HL4379|Televisão|3|Rodrigo|Bruno|10/5/2018|São Paulo|2500|NaN|7500|
|1240|5665|HL1918|iPhone|1|Daniel|Monteiro|8/19/2018|São Paulo|5300|NaN|5300|
|1241|5667|HL8851|Notebook|5|João|Abraçado|10/13/2018|São Paulo|3500|NaN|17500|
|1242|5668|HL2714|Tablet|5|Guilherme|Jordao|9/8/2018|São Paulo|1600|NaN|8000|
|1243|5678|HL8851|Notebook|1|Pedro|Delgado|4/22/2018|São Paulo|3500|NaN|3500|
|1244|5693|HL7348|SmartWatch|4|Isabella|Rodrigues|2/27/2018|São Paulo|1400|NaN|5600|
|1245|5699|HL8851|Notebook|5|Ylana|Teraoka|2/16/2018|São Paulo|3500|NaN|17500|
|1246|5701|HL1918|iPhone|2|Caio|Ferreira|11/23/2018|São Paulo|5300|NaN|10600|
|1247|5702|HL8851|Notebook|2|Juliana|Huon|8/16/2018|São Paulo|3500|NaN|7000|
|1248|5704|HL1148|Câmera|5|Raphael|Mattos|6/15/2018|São Paulo|2100|NaN|10500|
|1249|5710|HL4379|Televisão|2|Gabrielle|Costa|12/10/2018|São Paulo|2500|NaN|5000|
|1250|5711|HL4379|Televisão|2|Thomáz|Bôas|5/7/2018|São Paulo|2500|NaN|5000|
|1251|5718|HL1918|iPhone|3|Lucas|Rocha|8/10/2018|São Paulo|5300|NaN|15900|
|1252|5728|HL1918|iPhone|5|Isabella|Santos|12/29/2018|São Paulo|5300|NaN|26500|
|1253|5736|HL8851|Notebook|2|Jéssica|Netto|7/7/2018|São Paulo|3500|NaN|7000|
|1254|5741|HL2714|Tablet|2|Maria|Assumpção|9/30/2018|São Paulo|1600|NaN|3200|
|1255|5742|HL4379|Televisão|2|Marina|Gama|8/10/2018|São Paulo|2500|NaN|5000|
|1256|5755|HL4379|Televisão|1|Wellington|Duarte|12/30/2018|São Paulo|2500|NaN|2500|
|1257|5757|HL1918|iPhone|1|Guilherme|Santos|11/8/2018|São Paulo|5300|NaN|5300|
|1258|5759|HL8851|Notebook|2|Vanessa|Neves|1/26/2018|São Paulo|3500|NaN|7000|
|1259|5763|HL9962|Android|4|Vanessa|Neves|11/14/2018|São Paulo|3400|NaN|13600|
|1260|5764|HL4379|Televisão|5|Letícia|Araujo|3/19/2018|São Paulo|2500|NaN|12500|
|1261|5767|HL9962|Android|1|Stephanie|Oliveira|6/22/2018|São Paulo|3400|NaN|3400|
|1262|5770|HL4379|Televisão|5|Luiz|Limp|12/19/2018|São Paulo|2500|NaN|12500|
|1263|5772|HL9962|Android|4|Luã|Sá|7/31/2018|São Paulo|3400|NaN|13600|
|1264|5776|HL7348|SmartWatch|3|Rebeca|Taylor|7/28/2018|São Paulo|1400|NaN|4200|
|1265|5779|HL1918|iPhone|3|Bruno|Souza|10/26/2018|São Paulo|5300|NaN|15900|
|1266|5789|HL1918|iPhone|3|Pedro|Dalforne|3/1/2018|São Paulo|5300|NaN|15900|
|1267|5791|HL1148|Câmera|2|Rodrigo|Mendes|2/6/2018|São Paulo|2100|NaN|4200|
|1268|5792|HL1918|iPhone|2|Camila|Sobral|12/30/2018|São Paulo|5300|NaN|10600|
|1269|5797|HL8851|Notebook|5|Matheus|Ramos|12/4/2018|São Paulo|3500|NaN|17500|
|1270|5801|HL1918|iPhone|3|Juliana|Guimarães|9/5/2018|São Paulo|5300|NaN|15900|
|1271|5817|HL8851|Notebook|1|Camille|Silva|4/24/2018|São Paulo|3500|NaN|3500|
|1272|5820|HL1148|Câmera|3|Lucas|Chagas|10/23/2018|São Paulo|2100|NaN|6300|
|1273|5821|HL9962|Android|5|Arthur|Fernandes|11/11/2018|São Paulo|3400|NaN|17000|
|1274|5822|HL1918|iPhone|1|Khaio|Mesquita|1/15/2018|São Paulo|5300|NaN|5300|
|1275|5824|HL1918|iPhone|2|Larissa|Florim|4/24/2018|São Paulo|5300|NaN|10600|
|1276|5825|HL1918|iPhone|4|Kim|Ferreira|2/5/2018|São Paulo|5300|NaN|21200|
|1277|5828|HL7348|SmartWatch|3|Juliana|Silva|11/30/2018|São Paulo|1400|NaN|4200|
|1278|5829|HL1918|iPhone|2|Caroline|Delgado|2/5/2018|São Paulo|5300|NaN|10600|
|1279|5832|HL1918|iPhone|2|Thayna|Martins|7/27/2018|São Paulo|5300|NaN|10600|
|1280|5840|HL7348|SmartWatch|3|Gabrielle|Porto|10/26/2018|São Paulo|1400|NaN|4200|
|1281|5841|HL1148|Câmera|5|Daniela|Pereira|3/16/2018|São Paulo|2100|NaN|10500|
|1282|5845|HL9962|Android|2|Bernardo|Borges|6/28/2018|São Paulo|3400|NaN|6800|
|1283|5848|HL1918|iPhone|1|João|Peçanha|8/14/2018|São Paulo|5300|NaN|5300|
|1284|5854|HL1918|iPhone|5|Carlos|Cardoso|2/21/2018|São Paulo|5300|NaN|26500|
|1285|5856|HL9962|Android|4|Ulisses|Filho|1/13/2018|São Paulo|3400|NaN|13600|
|1286|5857|HL1918|iPhone|3|Samara|Pinto|11/12/2018|São Paulo|5300|NaN|15900|
|1287|5859|HL1148|Câmera|3|Carolina|Motta|3/28/2018|São Paulo|2100|NaN|6300|
|1288|5860|HL9962|Android|2|Breno|Costa|10/26/2018|São Paulo|3400|NaN|6800|
|1289|5862|HL1918|iPhone|2|Marina|Marins|5/9/2018|São Paulo|5300|NaN|10600|
|1290|5866|HL1918|iPhone|4|Thales|Fanara|9/19/2018|São Paulo|5300|NaN|21200|
|1291|5870|HL9962|Android|3|João|Capitulo|2/5/2018|São Paulo|3400|NaN|10200|
|1292|5873|HL1918|iPhone|4|Gabriel|Puntel|8/20/2018|São Paulo|5300|NaN|21200|
|1293|5877|HL4379|Televisão|1|Carolina|Bernardes|6/19/2018|São Paulo|2500|NaN|2500|
|1294|5879|HL9962|Android|4|Sandy|Ribeiro|3/21/2018|São Paulo|3400|NaN|13600|
|1295|5881|HL2714|Tablet|1|Daniel|Monteiro|5/29/2018|São Paulo|1600|NaN|1600|
|1296|5883|HL1918|iPhone|1|João|Júnior|5/10/2018|São Paulo|5300|NaN|5300|
|1297|5892|HL1918|iPhone|1|Mariana|Sousa|6/20/2018|São Paulo|5300|NaN|5300|
|1298|5895|HL1148|Câmera|3|João|Peçanha|11/2/2018|São Paulo|2100|NaN|6300|
|1299|5896|HL7348|SmartWatch|5|Adrielle|Forte|1/27/2018|São Paulo|1400|NaN|7000|
|1300|5900|HL9962|Android|4|Vinícius|Antunes|6/16/2018|São Paulo|3400|NaN|13600|
|1301|5910|HL4379|Televisão|5|Luã|Sá|1/3/2018|São Paulo|2500|NaN|12500|
|1302|5917|HL1918|iPhone|5|Helvio|Pedrosa|8/19/2018|São Paulo|5300|NaN|26500|
|1303|5924|HL8851|Notebook|4|Amanda|Braga|11/7/2018|São Paulo|3500|NaN|14000|
|1304|5927|HL8851|Notebook|2|Renan|Cunha|1/19/2018|São Paulo|3500|NaN|7000|
|1305|5929|HL4379|Televisão|1|Eduardo|Ferreira|4/6/2018|São Paulo|2500|NaN|2500|
|1306|5943|HL8851|Notebook|5|Lara|Moreira|4/17/2018|São Paulo|3500|NaN|17500|
|1307|5944|HL1918|iPhone|4|Paola|Abreu|11/21/2018|São Paulo|5300|NaN|21200|
|1308|5947|HL1918|iPhone|5|Larissa|Florim|5/31/2018|São Paulo|5300|NaN|26500|
|1309|5954|HL4379|Televisão|3|Aline|Morais|3/20/2018|São Paulo|2500|NaN|7500|
|1310|5958|HL4379|Televisão|3|Jackson|Derossi|12/21/2018|São Paulo|2500|NaN|7500|
|1311|5964|HL1918|iPhone|2|João|Castilho|12/22/2018|São Paulo|5300|NaN|10600|
|1312|5966|HL1918|iPhone|5|Juliana|Correa|3/23/2018|São Paulo|5300|NaN|26500|
|1313|5972|HL7348|SmartWatch|4|Fillipe|Almeida|5/20/2018|São Paulo|1400|NaN|5600|
|1314|5975|HL1918|iPhone|4|Marcelo|Pereira|1/23/2018|São Paulo|5300|NaN|21200|
|1315|5976|HL1148|Câmera|2|Ana|Michetti|4/16/2018|São Paulo|2100|NaN|4200|
|1316|5981|HL1148|Câmera|3|Hércules|Júnior|3/17/2018|São Paulo|2100|NaN|6300|
|1317|5982|HL7348|SmartWatch|2|Pedro|Ronfini|8/11/2018|São Paulo|1400|NaN|2800|
|1318|5984|HL4379|Televisão|5|João|Pedrazza|1/19/2018|São Paulo|2500|NaN|12500|
|1319|5991|HL1918|iPhone|4|Luíza|Goulart|6/19/2018|São Paulo|5300|NaN|21200|
|1320|5993|HL4379|Televisão|2|Bruna|Brandao|12/18/2018|São Paulo|2500|NaN|5000|
|1321|6011|HL1918|iPhone|1|Lucas|Wanderley|12/22/2018|São Paulo|5300|NaN|5300|
|1322|6013|HL1918|iPhone|5|Wilson|Miranda|11/12/2018|São Paulo|5300|NaN|26500|
|1323|6025|HL9962|Android|3|Luis|Garcia|5/25/2018|São Paulo|3400|NaN|10200|
|1324|6029|HL1918|iPhone|1|Luiz|Limp|4/15/2018|São Paulo|5300|NaN|5300|
|1325|6033|HL4379|Televisão|3|Juliana|Silva|8/20/2018|São Paulo|2500|NaN|7500|
|1326|6036|HL1918|iPhone|1|Carlos|Galvão|9/5/2018|São Paulo|5300|NaN|5300|
|1327|6037|HL7348|SmartWatch|5|André|Alves|9/21/2018|São Paulo|1400|NaN|7000|
|1328|6039|HL1918|iPhone|1|Bruna|Franco|11/22/2018|São Paulo|5300|NaN|5300|
|1329|6048|HL8851|Notebook|4|Juliana|Souza|12/11/2018|São Paulo|3500|NaN|14000|
|1330|6053|HL7348|SmartWatch|5|Norman|Jimbo|10/5/2018|São Paulo|1400|NaN|7000|
|1331|6055|HL1148|Câmera|1|Guilherme|Santos|12/14/2018|São Paulo|2100|NaN|2100|
|1332|6056|HL8851|Notebook|3|Thales|Gouvêa|8/17/2018|São Paulo|3500|NaN|10500|
|1333|6058|HL1148|Câmera|1|André|Alves|4/20/2018|São Paulo|2100|NaN|2100|
|1334|6060|HL9962|Android|2|Leticia|Mesquita|5/12/2018|São Paulo|3400|NaN|6800|
|1335|6068|HL9962|Android|3|Bruna|Rangel|4/18/2018|São Paulo|3400|NaN|10200|
|1336|6071|HL4379|Televisão|1|Carlos|Barbosa|4/6/2018|São Paulo|2500|NaN|2500|
|1337|6077|HL8851|Notebook|2|Bruno|Freitas|1/17/2018|São Paulo|3500|NaN|7000|
|1338|6078|HL4379|Televisão|1|David|Campelo|6/1/2018|São Paulo|2500|NaN|2500|
|1339|6079|HL7348|SmartWatch|2|Lucas|Neto|5/17/2018|São Paulo|1400|NaN|2800|
|1340|6090|HL9962|Android|5|Eduardo|Soares|3/7/2018|São Paulo|3400|NaN|17000|
|1341|6094|HL2714|Tablet|5|Thales|Gouvêa|4/17/2018|São Paulo|1600|NaN|8000|
|1342|6098|HL1918|iPhone|4|Caio|Fernandes|9/30/2018|São Paulo|5300|NaN|21200|
|1343|6099|HL9962|Android|4|Joyce|Medina|9/7/2018|São Paulo|3400|NaN|13600|
|1344|6100|HL9962|Android|4|Ives|Barbosa|1/31/2018|São Paulo|3400|NaN|13600|
|1345|6102|HL1918|iPhone|4|Bruno|Silva|10/2/2018|São Paulo|5300|NaN|21200|
|1346|6107|HL4379|Televisão|4|Guilherme|Seixas|4/12/2018|São Paulo|2500|NaN|10000|
|1347|6109|HL9962|Android|4|Rachel|Restum|7/6/2018|São Paulo|3400|NaN|13600|
|1348|6113|HL1918|iPhone|1|Gabriel|Assis|11/8/2018|São Paulo|5300|NaN|5300|
|1349|6118|HL8851|Notebook|5|Iuri|Neto|5/21/2018|São Paulo|3500|NaN|17500|
|1350|6119|HL7348|SmartWatch|2|Stephanie|Gonçalves|1/28/2018|São Paulo|1400|NaN|2800|
|1351|6121|HL4379|Televisão|3|Renan|Firmino|3/30/2018|São Paulo|2500|NaN|7500|
|1352|6122|HL1918|iPhone|2|Lucas|Reis|5/16/2018|São Paulo|5300|NaN|10600|
|1353|6126|HL4379|Televisão|4|Jéssica|Teixeira|2/16/2018|São Paulo|2500|NaN|10000|
|1354|6127|HL1918|iPhone|4|Karina|Camara|3/11/2018|São Paulo|5300|NaN|21200|
|1355|6128|HL1918|iPhone|4|Thales|Andrade|2/9/2018|São Paulo|5300|NaN|21200|
|1356|6136|HL4379|Televisão|2|Aline|Morais|7/24/2018|São Paulo|2500|NaN|5000|
|1357|6138|HL1918|iPhone|4|Thiago|Veloso|5/28/2018|São Paulo|5300|NaN|21200|
|1358|6140|HL1918|iPhone|2|Daniel|Terra|2/19/2018|São Paulo|5300|NaN|10600|
|1359|6150|HL8851|Notebook|2|Diego|Barros|6/25/2018|São Paulo|3500|NaN|7000|
|1360|6151|HL1918|iPhone|2|Wellington|Duarte|7/11/2018|São Paulo|5300|NaN|10600|
|1361|6152|HL1918|iPhone|3|Sthefeson|Pereira|11/14/2018|São Paulo|5300|NaN|15900|
|1362|6155|HL1918|iPhone|3|Luiz|Mendonça|9/12/2018|São Paulo|5300|NaN|15900|
|1363|6156|HL1148|Câmera|3|Stephanie|Oliveira|6/19/2018|São Paulo|2100|NaN|6300|
|1364|6158|HL4379|Televisão|3|Hygor|Essaber|4/13/2018|São Paulo|2500|NaN|7500|
|1365|6160|HL1918|iPhone|1|Filipe|Barros|8/28/2018|São Paulo|5300|NaN|5300|
|1366|6164|HL2714|Tablet|1|Leandro|Melo|10/4/2018|São Paulo|1600|NaN|1600|
|1367|6178|HL4379|Televisão|5|Julia|Aliani|1/21/2018|São Paulo|2500|NaN|12500|
|1368|6184|HL9962|Android|2|Michelle|Miura|7/27/2018|São Paulo|3400|NaN|6800|
|1369|6187|HL1918|iPhone|1|Aline|Andrade|8/8/2018|São Paulo|5300|NaN|5300|
|1370|6190|HL4379|Televisão|2|Sthefeson|Kohn|9/28/2018|São Paulo|2500|NaN|5000|
|1371|6193|HL4379|Televisão|5|Rodrigo|Ramos|7/21/2018|São Paulo|2500|NaN|12500|
|1372|6196|HL2714|Tablet|5|Joyce|Souza|1/19/2018|São Paulo|1600|NaN|8000|
|1373|6206|HL1918|iPhone|4|Maria|Motta|6/27/2018|São Paulo|5300|NaN|21200|
|1374|6207|HL4379|Televisão|4|Jônatas|Tanaka|7/14/2018|São Paulo|2500|NaN|10000|
|1375|6218|HL1918|iPhone|5|Paulo|Campos|12/29/2018|São Paulo|5300|NaN|26500|
|1376|6225|HL8851|Notebook|1|Juliana|Pacheco|11/5/2018|São Paulo|3500|NaN|3500|
|1377|6228|HL8851|Notebook|4|Mariane|Ferreira|12/18/2018|São Paulo|3500|NaN|14000|
|1378|6230|HL4379|Televisão|4|Monique|Vasconcelos|6/30/2018|São Paulo|2500|NaN|10000|
|1379|6233|HL1918|iPhone|1|Wilson|Farias|5/23/2018|São Paulo|5300|NaN|5300|
|1380|6236|HL2714|Tablet|1|Gabriel|Soares|1/9/2018|São Paulo|1600|NaN|1600|
|1381|6241|HL7348|SmartWatch|3|João|Castilho|11/14/2018|São Paulo|1400|NaN|4200|
|1382|6255|HL7348|SmartWatch|5|Gabriel|Silva|11/1/2018|São Paulo|1400|NaN|7000|
|1383|6256|HL8851|Notebook|2|Eduardo|Silva|4/4/2018|São Paulo|3500|NaN|7000|
|1384|6259|HL1918|iPhone|1|Luis|Silva|9/14/2018|São Paulo|5300|NaN|5300|
|1385|6263|HL7348|SmartWatch|3|Wilson|Vianna|9/8/2018|São Paulo|1400|NaN|4200|
|1386|6265|HL8851|Notebook|4|Gabriel|Ribeiro|9/2/2018|São Paulo|3500|NaN|14000|
|1387|6266|HL9962|Android|2|João|Menezes|4/14/2018|São Paulo|3400|NaN|6800|
|1388|6267|HL8851|Notebook|5|Raul|Junqueira|9/15/2018|São Paulo|3500|NaN|17500|
|1389|6276|HL8851|Notebook|5|Alexandre|Rodriguez|1/9/2018|São Paulo|3500|NaN|17500|
|1390|6280|HL9962|Android|4|João|Guadagnino|1/16/2018|São Paulo|3400|NaN|13600|
|1391|6281|HL4379|Televisão|4|Jéssica|Stefanelli|7/17/2018|São Paulo|2500|NaN|10000|
|1392|6283|HL9962|Android|2|Ruan|Lopes|10/17/2018|São Paulo|3400|NaN|6800|
|1393|6286|HL7348|SmartWatch|1|Luiz|Mendonça|5/31/2018|São Paulo|1400|NaN|1400|
|1394|6287|HL2714|Tablet|1|Thales|Santos|12/15/2018|São Paulo|1600|NaN|1600|
|1395|6296|HL8851|Notebook|4|Wilson|Farias|12/12/2018|São Paulo|3500|NaN|14000|
|1396|6297|HL1148|Câmera|2|Beatriz|Silva|4/3/2018|São Paulo|2100|NaN|4200|
|1397|6299|HL2714|Tablet|3|Guilherme|Assis|11/13/2018|São Paulo|1600|NaN|4800|
|1398|6301|HL8851|Notebook|2|Camila|Bastazini|11/6/2018|São Paulo|3500|NaN|7000|
|1399|6305|HL1918|iPhone|2|Luiza|Procaci|1/13/2018|São Paulo|5300|NaN|10600|
|1400|6306|HL1918|iPhone|4|Thiago|Nóbrega|10/3/2018|São Paulo|5300|NaN|21200|
|1401|6318|HL4379|Televisão|3|Eric|Júnior|10/17/2018|São Paulo|2500|NaN|7500|
|1402|6325|HL4379|Televisão|5|Luis|Oliveira|7/9/2018|São Paulo|2500|NaN|12500|
|1403|6328|HL8851|Notebook|5|Mariana|Rotava|1/29/2018|São Paulo|3500|NaN|17500|
|1404|6335|HL7348|SmartWatch|5|Gabriel|Almeida|4/19/2018|São Paulo|1400|NaN|7000|
|1405|6339|HL1918|iPhone|2|Danilo|Alves|6/7/2018|São Paulo|5300|NaN|10600|
|1406|6342|HL7348|SmartWatch|4|Roger|Rosa|10/17/2018|São Paulo|1400|NaN|5600|
|1407|6343|HL8851|Notebook|1|Lázaro|Villanova|10/12/2018|São Paulo|3500|NaN|3500|
|1408|6349|HL1918|iPhone|4|Guilherme|Merotto|7/1/2018|São Paulo|5300|NaN|21200|
|1409|6351|HL1918|iPhone|2|Julia|Teixeira|4/9/2018|São Paulo|5300|NaN|10600|
|1410|6354|HL4379|Televisão|4|Danilo|Mendonça|8/4/2018|São Paulo|2500|NaN|10000|
|1411|6357|HL8851|Notebook|4|Marcelo|Pereira|10/20/2018|São Paulo|3500|NaN|14000|
|1412|6358|HL1918|iPhone|3|Daniela|Andrada|4/20/2018|São Paulo|5300|NaN|15900|
|1413|6360|HL9962|Android|2|Lucas|Machado|3/3/2018|São Paulo|3400|NaN|6800|
|1414|6368|HL7348|SmartWatch|2|Roberto|Mattos|2/2/2018|São Paulo|1400|NaN|2800|
|1415|6375|HL1148|Câmera|4|Ana|Campos|5/14/2018|São Paulo|2100|NaN|8400|
|1416|6379|HL2714|Tablet|3|Victor|Soares|7/6/2018|São Paulo|1600|NaN|4800|
|1417|6384|HL1918|iPhone|1|Rafael|Ramos|6/23/2018|São Paulo|5300|NaN|5300|
|1418|6386|HL1148|Câmera|4|Rodrigo|Bruno|6/21/2018|São Paulo|2100|NaN|8400|
|1419|6407|HL4379|Televisão|5|Jorge|Fonseca|11/16/2018|São Paulo|2500|NaN|12500|
|1420|6410|HL4379|Televisão|3|Wilson|Meirelles|10/20/2018|São Paulo|2500|NaN|7500|
|1421|6411|HL4379|Televisão|1|Luiza|Johnson|3/19/2018|São Paulo|2500|NaN|2500|
|1422|6412|HL2714|Tablet|3|Luis|Souza|9/21/2018|São Paulo|1600|NaN|4800|
|1423|6415|HL4379|Televisão|3|Larissa|Jesus|1/10/2018|São Paulo|2500|NaN|7500|
|1424|6419|HL1148|Câmera|1|Brenno|Santos|8/31/2018|São Paulo|2100|NaN|2100|
|1425|6426|HL9962|Android|4|Kimberly|Sad|7/30/2018|São Paulo|3400|NaN|13600|
|1426|6431|HL7348|SmartWatch|3|Allan|Candido|12/28/2018|São Paulo|1400|NaN|4200|
|1427|6432|HL1918|iPhone|1|Juliana|Guimarães|7/27/2018|São Paulo|5300|NaN|5300|
|1428|6435|HL4379|Televisão|5|Pedro|Ferrari|2/6/2018|São Paulo|2500|NaN|12500|
|1429|6443|HL4379|Televisão|4|Gabriella|Sagrillo|8/10/2018|São Paulo|2500|NaN|10000|
|1430|6448|HL4379|Televisão|5|Roberta|Pimenta|4/8/2018|São Paulo|2500|NaN|12500|
|1431|6449|HL9962|Android|4|Letícia|Leal|8/16/2018|São Paulo|3400|NaN|13600|
|1432|6450|HL7348|SmartWatch|5|Natalia|Guedes|6/10/2018|São Paulo|1400|NaN|7000|
|1433|6457|HL1918|iPhone|5|Luiza|Marques|5/31/2018|São Paulo|5300|NaN|26500|
|1434|6461|HL1148|Câmera|3|Pedro|Bitencourt|12/3/2018|São Paulo|2100|NaN|6300|
|1435|6469|HL2714|Tablet|2|Isabel|Lacerda|9/23/2018|São Paulo|1600|NaN|3200|
|1436|6474|HL1918|iPhone|2|Gustavo|Erthal|12/22/2018|São Paulo|5300|NaN|10600|
|1437|6478|HL9962|Android|4|João|Guadagnino|8/22/2018|São Paulo|3400|NaN|13600|
|1438|6480|HL1148|Câmera|5|Lucas|Machado|5/21/2018|São Paulo|2100|NaN|10500|
|1439|6485|HL1918|iPhone|1|Victor|Franco|6/9/2018|São Paulo|5300|NaN|5300|
|1440|6488|HL1918|iPhone|5|Henrique|Oliveira|10/11/2018|São Paulo|5300|NaN|26500|
|1441|6493|HL1148|Câmera|5|Thiago|Nóbrega|3/3/2018|São Paulo|2100|NaN|10500|
|1442|6497|HL2714|Tablet|3|Audir|Franco|4/21/2018|São Paulo|1600|NaN|4800|
|1443|6499|HL4379|Televisão|2|Marina|Gama|4/3/2018|São Paulo|2500|NaN|5000|
|1444|6501|HL1918|iPhone|1|Raísa|Berto|2/13/2018|São Paulo|5300|NaN|5300|
|1445|6507|HL4379|Televisão|5|Ana|Monte|1/30/2018|São Paulo|2500|NaN|12500|
|1446|6511|HL9962|Android|5|Thomáz|Bôas|5/2/2018|São Paulo|3400|NaN|17000|
|1447|6522|HL1918|iPhone|4|Amanda|Amaral|7/18/2018|São Paulo|5300|NaN|21200|
|1448|6535|HL1918|iPhone|2|Julia|Leig|1/21/2018|São Paulo|5300|NaN|10600|
|1449|6538|HL1918|iPhone|3|Eric|Neves|7/13/2018|São Paulo|5300|NaN|15900|
|1450|6541|HL8851|Notebook|1|Priscila|Vogel|11/18/2018|São Paulo|3500|NaN|3500|
|1451|6554|HL1918|iPhone|5|Camila|Bastazini|4/10/2018|São Paulo|5300|NaN|26500|
|1452|6555|HL8851|Notebook|5|Juliana|Barreira|6/3/2018|São Paulo|3500|NaN|17500|
|1453|6558|HL1918|iPhone|2|Juan|Barbosa|6/28/2018|São Paulo|5300|NaN|10600|
|1454|6562|HL1918|iPhone|1|Marina|Perdomo|5/16/2018|São Paulo|5300|NaN|5300|
|1455|6566|HL9962|Android|1|Matheus|Miranda|10/17/2018|São Paulo|3400|NaN|3400|
|1456|6569|HL8851|Notebook|1|Mateus|Duque|6/10/2018|São Paulo|3500|NaN|3500|
|1457|6572|HL4379|Televisão|1|Myllena|Carneiro|11/15/2018|São Paulo|2500|NaN|2500|
|1458|6574|HL2714|Tablet|3|Hanna|Fonseca|4/1/2018|São Paulo|1600|NaN|4800|
|1459|6576|HL7348|SmartWatch|5|Hércules|Moreira|11/8/2018|São Paulo|1400|NaN|7000|
|1460|6581|HL1918|iPhone|1|Maria|Assumpção|5/1/2018|São Paulo|5300|NaN|5300|
|1461|6583|HL1918|iPhone|2|Bernardo|Ribeiro|8/12/2018|São Paulo|5300|NaN|10600|
|1462|6585|HL4379|Televisão|3|Natalia|Marinho|4/16/2018|São Paulo|2500|NaN|7500|
|1463|6593|HL7348|SmartWatch|3|Pedro|Delgado|3/17/2018|São Paulo|1400|NaN|4200|
|1464|6595|HL9962|Android|3|Carolina|Rocha|11/1/2018|São Paulo|3400|NaN|10200|
|1465|6598|HL1918|iPhone|3|Roberto|Tiradentes|12/18/2018|São Paulo|5300|NaN|15900|
|1466|6601|HL8851|Notebook|2|Ana|Carvalho|7/21/2018|São Paulo|3500|NaN|7000|
|1467|6602|HL1918|iPhone|1|Renan|Ventura|8/29/2018|São Paulo|5300|NaN|5300|
|1468|6609|HL1918|iPhone|3|Caio|Vianna|3/16/2018|São Paulo|5300|NaN|15900|
|1469|6610|HL8851|Notebook|1|Miguel|Carneiro|10/20/2018|São Paulo|3500|NaN|3500|
|1470|6614|HL4379|Televisão|1|Bruno|Ferreira|10/6/2018|São Paulo|2500|NaN|2500|
|1471|6618|HL2714|Tablet|5|Juliana|Barreira|12/27/2018|São Paulo|1600|NaN|8000|
|1472|6623|HL1148|Câmera|5|Allan|Candido|3/18/2018|São Paulo|2100|NaN|10500|
|1473|6628|HL9962|Android|3|Pedro|Rodrigues|2/12/2018|São Paulo|3400|NaN|10200|
|1474|6631|HL1148|Câmera|5|Leandro|Ferreira|11/22/2018|São Paulo|2100|NaN|10500|
|1475|6632|HL2714|Tablet|2|Rafael|Rocha|12/8/2018|São Paulo|1600|NaN|3200|
|1476|6644|HL1148|Câmera|2|Bianca|Tatsch|2/23/2018|São Paulo|2100|NaN|4200|
|1477|6646|HL7348|SmartWatch|1|Joana|Calmon|8/7/2018|São Paulo|1400|NaN|1400|
|1478|6647|HL8851|Notebook|4|Patrícia|Amaral|6/27/2018|São Paulo|3500|NaN|14000|
|1479|6656|HL4379|Televisão|2|Gabriel|Thoni|3/13/2018|São Paulo|2500|NaN|5000|
|1480|6670|HL1148|Câmera|1|Gabriel|Thoni|3/23/2018|São Paulo|2100|NaN|2100|
|1481|6671|HL9962|Android|5|Lucas|Coelho|6/30/2018|São Paulo|3400|NaN|17000|
|1482|6678|HL4379|Televisão|4|Ian|Almeida|1/20/2018|São Paulo|2500|NaN|10000|
|1483|6680|HL2714|Tablet|4|Maria|Gasperi|8/22/2018|São Paulo|1600|NaN|6400|
|1484|6688|HL7348|SmartWatch|1|Marcelo|Magalhães|9/26/2018|São Paulo|1400|NaN|1400|
|1485|6692|HL8851|Notebook|5|Ana|Carvalho|7/26/2018|São Paulo|3500|NaN|17500|
|1486|6698|HL1148|Câmera|4|Luíza|Melo|11/5/2018|São Paulo|2100|NaN|8400|
|1487|6701|HL4379|Televisão|3|Gabriel|Almeida|6/28/2018|São Paulo|2500|NaN|7500|
|1488|6702|HL4379|Televisão|2|Wellington|Duarte|8/22/2018|São Paulo|2500|NaN|5000|
|1489|6703|HL2714|Tablet|4|Débora|Lopes|3/26/2018|São Paulo|1600|NaN|6400|
|1490|6704|HL1918|iPhone|4|João|Abraçado|4/27/2018|São Paulo|5300|NaN|21200|
|1491|6716|HL1148|Câmera|3|Roberto|Nogueira|9/15/2018|São Paulo|2100|NaN|6300|
|1492|6717|HL8851|Notebook|4|Marcelo|Rosa|5/2/2018|São Paulo|3500|NaN|14000|
|1493|6721|HL4379|Televisão|5|Jônatas|Soares|6/25/2018|São Paulo|2500|NaN|12500|
|1494|6728|HL1918|iPhone|3|Rafaella|Mello|6/26/2018|São Paulo|5300|NaN|15900|
|1495|6745|HL1918|iPhone|3|Nathan|Morelli|9/7/2018|São Paulo|5300|NaN|15900|
|1496|6747|HL1918|iPhone|4|Maria|Cardoso|4/3/2018|São Paulo|5300|NaN|21200|
|1497|6749|HL1918|iPhone|5|Raíssa|Oliveira|2/14/2018|São Paulo|5300|NaN|26500|
|1498|6758|HL9962|Android|1|Andre|Sampaio|7/31/2018|São Paulo|3400|NaN|3400|
|1499|6760|HL4379|Televisão|5|Bárbara|Lima|7/29/2018|São Paulo|2500|NaN|12500|
|1500|6763|HL1918|iPhone|1|Raíssa|Oliveira|2/8/2018|São Paulo|5300|NaN|5300|
|1501|6773|HL4379|Televisão|5|Milena|Alcoforado|4/8/2018|São Paulo|2500|NaN|12500|
|1502|6779|HL8851|Notebook|5|Sthefeson|Barroso|8/18/2018|São Paulo|3500|NaN|17500|
|1503|6783|HL1918|iPhone|3|Gabriella|Sagrillo|8/27/2018|São Paulo|5300|NaN|15900|
|1504|6786|HL1918|iPhone|5|Wilson|Farias|4/16/2018|São Paulo|5300|NaN|26500|
|1505|6788|HL1918|iPhone|5|Victor|Gomes|8/11/2018|São Paulo|5300|NaN|26500|
|1506|6789|HL8851|Notebook|2|Luis|Oliveira|12/29/2018|São Paulo|3500|NaN|7000|
|1507|6797|HL2714|Tablet|1|Alon|Palmeira|7/21/2018|São Paulo|1600|NaN|1600|
|1508|6802|HL2714|Tablet|4|Letícia|Leal|12/4/2018|São Paulo|1600|NaN|6400|
|1509|6815|HL7348|SmartWatch|5|Clarissa|Santos|2/18/2018|São Paulo|1400|NaN|7000|
|1510|6818|HL1148|Câmera|3|José|Fonseca|12/6/2018|São Paulo|2100|NaN|6300|
|1511|6822|HL1918|iPhone|2|Caio|Vianna|10/31/2018|São Paulo|5300|NaN|10600|
|1512|6823|HL4379|Televisão|3|Giulia|Pessanha|5/20/2018|São Paulo|2500|NaN|7500|
|1513|6825|HL7348|SmartWatch|1|Tayla|Lima|11/3/2018|São Paulo|1400|NaN|1400|
|1514|6826|HL4379|Televisão|1|Julia|Aliani|4/8/2018|São Paulo|2500|NaN|2500|
|1515|6827|HL8851|Notebook|2|Jônatas|Soares|8/3/2018|São Paulo|3500|NaN|7000|
|1516|6831|HL8851|Notebook|4|Marcela|Gasperi|11/7/2018|São Paulo|3500|NaN|14000|
|1517|6836|HL4379|Televisão|3|Cézar|Santos|11/24/2018|São Paulo|2500|NaN|7500|
|1518|6844|HL1918|iPhone|1|Roberta|Nogueira|3/9/2018|São Paulo|5300|NaN|5300|
|1519|6852|HL2714|Tablet|5|Raphael|Kurtz|9/30/2018|São Paulo|1600|NaN|8000|
|1520|6856|HL1918|iPhone|3|Giuseppe|Bhering|1/31/2018|São Paulo|5300|NaN|15900|
|1521|6860|HL9962|Android|1|Eduardo|Veiga|10/16/2018|São Paulo|3400|NaN|3400|
|1522|6866|HL4379|Televisão|4|Danilo|Alves|8/10/2018|São Paulo|2500|NaN|10000|
|1523|6875|HL2714|Tablet|5|Sthefeson|Barroso|4/20/2018|São Paulo|1600|NaN|8000|
|1524|6878|HL8851|Notebook|4|Caio|Affonso|9/22/2018|São Paulo|3500|NaN|14000|
|1525|6881|HL8851|Notebook|4|Thaís|Moura|4/19/2018|São Paulo|3500|NaN|14000|
|1526|6882|HL1918|iPhone|1|Nathan|Morelli|8/6/2018|São Paulo|5300|NaN|5300|
|1527|6892|HL1918|iPhone|4|Jônatas|Tanaka|6/29/2018|São Paulo|5300|NaN|21200|
|1528|6898|HL7348|SmartWatch|5|Michelle|Pereira|3/16/2018|São Paulo|1400|NaN|7000|
|1529|6902|HL8851|Notebook|5|Roberto|Mattos|11/17/2018|São Paulo|3500|NaN|17500|
|1530|6906|HL1918|iPhone|4|Danilo|Mendonça|4/15/2018|São Paulo|5300|NaN|21200|
|1531|6909|HL1918|iPhone|3|Gustavo|Guimarães|8/13/2018|São Paulo|5300|NaN|15900|
|1532|6914|HL4379|Televisão|3|Caroline|Aquino|4/2/2018|São Paulo|2500|NaN|7500|
|1533|6915|HL4379|Televisão|5|Camila|Sobral|4/5/2018|São Paulo|2500|NaN|12500|
|1534|6919|HL1918|iPhone|5|Juliana|Huon|4/15/2018|São Paulo|5300|NaN|26500|
|1535|6924|HL8851|Notebook|3|João|Bach|6/28/2018|São Paulo|3500|NaN|10500|
|1536|6925|HL1918|iPhone|5|Adriane|Gomes|9/23/2018|São Paulo|5300|NaN|26500|
|1537|6929|HL2714|Tablet|5|Maria|Motta|12/7/2018|São Paulo|1600|NaN|8000|
|1538|6933|HL9962|Android|1|Vanessa|Neves|2/21/2018|São Paulo|3400|NaN|3400|
|1539|6936|HL1918|iPhone|2|Marina|Delgado|7/6/2018|São Paulo|5300|NaN|10600|
|1540|6946|HL1918|iPhone|2|Fernanda|Rubim|4/12/2018|São Paulo|5300|NaN|10600|
|1541|6955|HL1918|iPhone|5|Luiz|Mendonça|1/31/2018|São Paulo|5300|NaN|26500|
|1542|6958|HL8851|Notebook|5|Gustavo|Thome|8/28/2018|São Paulo|3500|NaN|17500|
|1543|6960|HL1918|iPhone|1|Aline|Morais|8/21/2018|São Paulo|5300|NaN|5300|
|1544|6963|HL4379|Televisão|2|Yasmim|Verly|10/30/2018|São Paulo|2500|NaN|5000|
|1545|6965|HL7348|SmartWatch|4|Luiza|Marques|5/2/2018|São Paulo|1400|NaN|5600|
|1546|6972|HL1148|Câmera|3|Camilla|Vieira|6/28/2018|São Paulo|2100|NaN|6300|
|1547|6975|HL7348|SmartWatch|1|Eduardo|Silva|2/26/2018|São Paulo|1400|NaN|1400|
|1548|6978|HL2714|Tablet|3|Célio|Xavier|9/9/2018|São Paulo|1600|NaN|4800|
|1549|6984|HL1918|iPhone|4|Thayane|Resende|9/24/2018|São Paulo|5300|NaN|21200|
|1550|6985|HL4379|Televisão|4|Luíza|Melo|6/18/2018|São Paulo|2500|NaN|10000|
|1551|6999|HL1148|Câmera|2|Isabella|Montanholi|12/28/2018|São Paulo|2100|NaN|4200|
|1552|7003|HL9962|Android|3|Gabriel|Thoni|4/6/2018|São Paulo|3400|NaN|10200|
|1553|7011|HL1918|iPhone|5|Carlos|Souza|6/27/2018|São Paulo|5300|NaN|26500|
|1554|7017|HL1918|iPhone|4|Lázaro|Villanova|12/17/2018|São Paulo|5300|NaN|21200|
|1555|7020|HL2714|Tablet|2|Bianca|Ferezin|6/11/2018|São Paulo|1600|NaN|3200|
|1556|7029|HL8851|Notebook|2|David|Vasconcelos|9/7/2018|São Paulo|3500|NaN|7000|
|1557|7032|HL1918|iPhone|3|Guilherme|Lima|6/10/2018|São Paulo|5300|NaN|15900|
|1558|7039|HL1918|iPhone|2|Luiz|Freire|6/29/2018|São Paulo|5300|NaN|10600|
|1559|7041|HL2714|Tablet|3|Carolina|Vasconcelos|1/13/2018|São Paulo|1600|NaN|4800|
|1560|7053|HL1148|Câmera|5|Camilla|Cardeman|4/8/2018|São Paulo|2100|NaN|10500|
|1561|7056|HL8851|Notebook|2|Rafaela|Gonçalves|1/19/2018|São Paulo|3500|NaN|7000|
|1562|7057|HL4379|Televisão|3|José|Seixas|6/1/2018|São Paulo|2500|NaN|7500|
|1563|7058|HL1918|iPhone|5|Marcelo|Guadagnino|4/8/2018|São Paulo|5300|NaN|26500|
|1564|7060|HL1918|iPhone|5|David|Campelo|7/3/2018|São Paulo|5300|NaN|26500|
|1565|7066|HL1918|iPhone|1|Eduardo|Nunes|5/29/2018|São Paulo|5300|NaN|5300|
|1566|7067|HL2714|Tablet|1|Juliana|Correa|7/8/2018|São Paulo|1600|NaN|1600|
|1567|7071|HL1918|iPhone|5|Gustavo|Guimarães|6/5/2018|São Paulo|5300|NaN|26500|
|1568|7080|HL4379|Televisão|2|Roberto|Mattos|3/14/2018|São Paulo|2500|NaN|5000|
|1569|7085|HL1148|Câmera|4|Gabrielle|Porto|12/25/2018|São Paulo|2100|NaN|8400|
|1570|7092|HL1148|Câmera|4|Juliana|Souza|3/28/2018|São Paulo|2100|NaN|8400|
|1571|7094|HL4379|Televisão|5|Lorena|Kohn|9/13/2018|São Paulo|2500|NaN|12500|
|1572|7096|HL9962|Android|4|Rodrigo|Mendes|5/15/2018|São Paulo|3400|NaN|13600|
|1573|7097|HL9962|Android|1|Debora|Silva|5/10/2018|São Paulo|3400|NaN|3400|
|1574|7102|HL1148|Câmera|3|José|Marques|6/19/2018|São Paulo|2100|NaN|6300|
|1575|7107|HL1918|iPhone|4|Clara|Silveira|11/1/2018|São Paulo|5300|NaN|21200|
|1576|7115|HL1918|iPhone|5|Isabella|Santos|9/12/2018|São Paulo|5300|NaN|26500|
|1577|7119|HL1918|iPhone|4|Luis|Silva|9/23/2018|São Paulo|5300|NaN|21200|
|1578|7121|HL1918|iPhone|3|Juliana|Correa|2/5/2018|São Paulo|5300|NaN|15900|
|1579|7122|HL1918|iPhone|2|Rilson|Dias|3/26/2018|São Paulo|5300|NaN|10600|
|1580|7125|HL1918|iPhone|3|Lucas|Cavalcanti|4/3/2018|São Paulo|5300|NaN|15900|
|1581|7126|HL9962|Android|2|Amanda|Machado|8/5/2018|São Paulo|3400|NaN|6800|
|1582|7127|HL4379|Televisão|2|Ulisses|Quinto|11/2/2018|São Paulo|2500|NaN|5000|
|1583|7142|HL4379|Televisão|3|Izabel|Lopes|9/13/2018|São Paulo|2500|NaN|7500|
|1584|7143|HL9962|Android|1|Carla|Zakhm|8/23/2018|São Paulo|3400|NaN|3400|
|1585|7155|HL1918|iPhone|2|Leandro|Melo|10/15/2018|São Paulo|5300|NaN|10600|
|1586|7156|HL8851|Notebook|1|Gustavo|Accardo|12/15/2018|São Paulo|3500|NaN|3500|
|1587|7157|HL1148|Câmera|2|Lucas|Reis|5/21/2018|São Paulo|2100|NaN|4200|
|1588|7161|HL4379|Televisão|5|Livia|Corrêa|10/1/2018|São Paulo|2500|NaN|12500|
|1589|7168|HL1918|iPhone|1|Natália|Appel|10/29/2018|São Paulo|5300|NaN|5300|
|1590|7169|HL1148|Câmera|5|Platini|Heimlich|7/12/2018|São Paulo|2100|NaN|10500|
|1591|7174|HL4379|Televisão|3|Pedro|Bitencourt|9/13/2018|São Paulo|2500|NaN|7500|
|1592|7177|HL1148|Câmera|2|Lucas|Monte|9/30/2018|São Paulo|2100|NaN|4200|
|1593|7185|HL4379|Televisão|4|Adrielle|Gabriel|9/1/2018|São Paulo|2500|NaN|10000|
|1594|7189|HL7348|SmartWatch|2|Carolina|Motta|10/20/2018|São Paulo|1400|NaN|2800|
|1595|7191|HL7348|SmartWatch|1|Rebeca|Taylor|3/29/2018|São Paulo|1400|NaN|1400|
|1596|7193|HL2714|Tablet|3|Samara|Pinto|10/5/2018|São Paulo|1600|NaN|4800|
|1597|7198|HL4379|Televisão|4|Juliana|Huon|5/18/2018|São Paulo|2500|NaN|10000|
|1598|7199|HL8851|Notebook|1|Renan|Firmino|7/18/2018|São Paulo|3500|NaN|3500|
|1599|7201|HL1918|iPhone|5|Maria|Junior|12/26/2018|São Paulo|5300|NaN|26500|
|1600|7206|HL7348|SmartWatch|1|Júlio|Freire|1/2/2018|São Paulo|1400|NaN|1400|
|1601|7211|HL4379|Televisão|4|Guilherme|Lima|10/17/2018|São Paulo|2500|NaN|10000|
|1602|7219|HL1918|iPhone|5|Matheus|Silva|2/4/2018|São Paulo|5300|NaN|26500|
|1603|7223|HL4379|Televisão|3|Juliana|Barreira|11/11/2018|São Paulo|2500|NaN|7500|
|1604|7228|HL1148|Câmera|4|Juliana|Silva|8/19/2018|São Paulo|2100|NaN|8400|
|1605|7231|HL2714|Tablet|4|Caroline|Delgado|5/5/2018|São Paulo|1600|NaN|6400|
|1606|7239|HL1918|iPhone|1|Letícia|Leal|9/15/2018|São Paulo|5300|NaN|5300|
|1607|7242|HL1148|Câmera|2|Breno|Costa|10/2/2018|São Paulo|2100|NaN|4200|
|1608|7249|HL8851|Notebook|5|Ana|Felippe|1/6/2018|São Paulo|3500|NaN|17500|
|1609|7256|HL2714|Tablet|5|Thayna|Martins|2/11/2018|São Paulo|1600|NaN|8000|
|1610|7263|HL4379|Televisão|3|Gabriel|Assis|3/25/2018|São Paulo|2500|NaN|7500|
|1611|7267|HL7348|SmartWatch|3|Daniela|Rosa|6/3/2018|São Paulo|1400|NaN|4200|
|1612|7273|HL1918|iPhone|1|Ana|Leite|6/24/2018|São Paulo|5300|NaN|5300|
|1613|7277|HL1918|iPhone|4|Pedro|Ronfini|6/18/2018|São Paulo|5300|NaN|21200|
|1614|7286|HL2714|Tablet|2|Matheus|Miranda|12/12/2018|São Paulo|1600|NaN|3200|
|1615|7291|HL1918|iPhone|2|Raphael|Kurtz|7/19/2018|São Paulo|5300|NaN|10600|
|1616|7292|HL1918|iPhone|2|Myllena|Carneiro|7/3/2018|São Paulo|5300|NaN|10600|
|1617|7295|HL1918|iPhone|1|Rafael|Portela|1/20/2018|São Paulo|5300|NaN|5300|
|1618|7297|HL1148|Câmera|2|Amanda|Gontijo|2/24/2018|São Paulo|2100|NaN|4200|
|1619|7298|HL9962|Android|5|Pedro|Buraco|12/25/2018|São Paulo|3400|NaN|17000|
|1620|7300|HL7348|SmartWatch|2|Maike|Pereira|5/16/2018|São Paulo|1400|NaN|2800|
|1621|7301|HL4379|Televisão|5|Tadeu|Nakayama|1/28/2018|São Paulo|2500|NaN|12500|
|1622|7304|HL8851|Notebook|5|Leandro|Rodrigues|10/1/2018|São Paulo|3500|NaN|17500|
|1623|7309|HL4379|Televisão|5|Giselia|Thiele|7/28/2018|São Paulo|2500|NaN|12500|
|1624|7310|HL1918|iPhone|5|Larissa|Jesus|10/20/2018|São Paulo|5300|NaN|26500|
|1625|7315|HL2714|Tablet|2|Izabel|Lopes|3/25/2018|São Paulo|1600|NaN|3200|
|1626|7321|HL4379|Televisão|5|Thales|Fanara|2/17/2018|São Paulo|2500|NaN|12500|
|1627|7323|HL2714|Tablet|3|Paulo|Campos|4/24/2018|São Paulo|1600|NaN|4800|
|1628|7324|HL1148|Câmera|5|Breno|Godoy|12/15/2018|São Paulo|2100|NaN|10500|
|1629|7325|HL1918|iPhone|4|Nathan|Morelli|7/12/2018|São Paulo|5300|NaN|21200|
|1630|7329|HL4379|Televisão|2|Bruna|Londero|8/30/2018|São Paulo|2500|NaN|5000|
|1631|7330|HL4379|Televisão|3|Giuseppe|Borges|1/11/2018|São Paulo|2500|NaN|7500|
|1632|7339|HL1148|Câmera|2|Daniel|Nauenberg|12/12/2018|São Paulo|2100|NaN|4200|
|1633|7340|HL9962|Android|4|Michelle|Miura|3/9/2018|São Paulo|3400|NaN|13600|
|1634|7342|HL1918|iPhone|4|Guilherme|Assis|5/10/2018|São Paulo|5300|NaN|21200|
|1635|7344|HL1918|iPhone|4|Jéssica|Teixeira|11/27/2018|São Paulo|5300|NaN|21200|
|1636|7345|HL4379|Televisão|1|Beatriz|Perdomo|12/23/2018|São Paulo|2500|NaN|2500|
|1637|7360|HL2714|Tablet|3|Danilo|Alves|12/29/2018|São Paulo|1600|NaN|4800|
|1638|7362|HL1918|iPhone|5|Ana|Miura|9/1/2018|São Paulo|5300|NaN|26500|
|1639|7364|HL1148|Câmera|1|Alexandre|Rodriguez|11/6/2018|São Paulo|2100|NaN|2100|
|1640|7370|HL1918|iPhone|5|Victor|Franco|1/31/2018|São Paulo|5300|NaN|26500|
|1641|7375|HL4379|Televisão|5|Eric|Neves|4/2/2018|São Paulo|2500|NaN|12500|
|1642|7377|HL1918|iPhone|5|João|Bach|9/17/2018|São Paulo|5300|NaN|26500|
|1643|7380|HL1918|iPhone|1|Rogério|Pereira|6/26/2018|São Paulo|5300|NaN|5300|
|1644|7382|HL4379|Televisão|4|Gabriel|Garcia|9/9/2018|São Paulo|2500|NaN|10000|
|1645|7383|HL1918|iPhone|4|Silvio|Fahrnholz|3/8/2018|São Paulo|5300|NaN|21200|
|1646|7394|HL7348|SmartWatch|1|Anna|Silva|9/14/2018|São Paulo|1400|NaN|1400|
|1647|7406|HL4379|Televisão|3|Anna|Silva|7/10/2018|São Paulo|2500|NaN|7500|
|1648|7409|HL4379|Televisão|2|Caio|Silva|5/8/2018|São Paulo|2500|NaN|5000|
|1649|7415|HL4379|Televisão|4|Ruan|Lopes|3/15/2018|São Paulo|2500|NaN|10000|
|1650|7416|HL9962|Android|4|Antonio|Bernhardt|10/14/2018|São Paulo|3400|NaN|13600|
|1651|7417|HL2714|Tablet|4|David|Assumpção|3/22/2018|São Paulo|1600|NaN|6400|
|1652|7422|HL1918|iPhone|1|Melissa|Nucci|3/2/2018|São Paulo|5300|NaN|5300|
|1653|7427|HL4379|Televisão|4|Thiago|Miura|12/11/2018|São Paulo|2500|NaN|10000|
|1654|7431|HL1918|iPhone|3|Larissa|Nauenberg|3/3/2018|São Paulo|5300|NaN|15900|
|1655|7434|HL4379|Televisão|4|Thainá|Binello|10/26/2018|São Paulo|2500|NaN|10000|
|1656|7435|HL2714|Tablet|1|Bruna|Franco|12/30/2018|São Paulo|1600|NaN|1600|
|1657|7436|HL4379|Televisão|2|Pedro|Santana|7/16/2018|São Paulo|2500|NaN|5000|
|1658|7437|HL1918|iPhone|1|Maria|Correa|7/7/2018|São Paulo|5300|NaN|5300|
|1659|7442|HL8851|Notebook|4|Andre|Nóbrega|5/2/2018|São Paulo|3500|NaN|14000|
|1660|7443|HL1918|iPhone|2|Júlio|Freire|5/18/2018|São Paulo|5300|NaN|10600|
|1661|7454|HL1148|Câmera|2|Jorge|Carvalho|2/24/2018|São Paulo|2100|NaN|4200|
|1662|7459|HL7348|SmartWatch|5|Matheus|Tostes|1/25/2018|São Paulo|1400|NaN|7000|
|1663|7460|HL1918|iPhone|2|Sthefeson|Kohn|6/24/2018|São Paulo|5300|NaN|10600|
|1664|7463|HL8851|Notebook|3|Gustavo|Gomes|5/25/2018|São Paulo|3500|NaN|10500|
|1665|7469|HL9962|Android|4|Juliana|Silva|12/23/2018|São Paulo|3400|NaN|13600|
|1666|7474|HL2714|Tablet|4|Rodrigo|Feijo|8/1/2018|São Paulo|1600|NaN|6400|
|1667|7475|HL1918|iPhone|4|Rebeca|Taylor|1/21/2018|São Paulo|5300|NaN|21200|
|1668|7476|HL2714|Tablet|5|Felipe|Júnior|2/8/2018|São Paulo|1600|NaN|8000|
|1669|7481|HL7348|SmartWatch|5|Gabriel|Silva|1/28/2018|São Paulo|1400|NaN|7000|
|1670|7482|HL4379|Televisão|4|Leandro|Melo|11/29/2018|São Paulo|2500|NaN|10000|
|1671|7483|HL1918|iPhone|4|Alon|Fahrnholz|10/28/2018|São Paulo|5300|NaN|21200|
|1672|7485|HL2714|Tablet|1|Victor|Lira|9/19/2018|São Paulo|1600|NaN|1600|
|1673|7492|HL4379|Televisão|5|Gustavo|Junior|9/4/2018|São Paulo|2500|NaN|12500|
|1674|7497|HL8851|Notebook|3|Julia|Aliani|10/8/2018|São Paulo|3500|NaN|10500|
|1675|7505|HL9962|Android|4|Pedro|Macckione|2/6/2018|São Paulo|3400|NaN|13600|
|1676|7515|HL9962|Android|1|Morgana|Correa|5/13/2018|São Paulo|3400|NaN|3400|
|1677|7520|HL1918|iPhone|5|Rebeca|Manhães|9/29/2018|São Paulo|5300|NaN|26500|
|1678|7522|HL9962|Android|2|Gabriel|Rubim|6/13/2018|São Paulo|3400|NaN|6800|
|1679|7525|HL7348|SmartWatch|1|Gabrielle|Vasconcelos|9/29/2018|São Paulo|1400|NaN|1400|
|1680|7530|HL1918|iPhone|1|Andressa|Chou|7/30/2018|São Paulo|5300|NaN|5300|
|1681|7533|HL4379|Televisão|5|Bianca|Tatsch|3/14/2018|São Paulo|2500|NaN|12500|
|1682|7539|HL4379|Televisão|4|Raissa|Negrelli|5/25/2018|São Paulo|2500|NaN|10000|
|1683|7555|HL1918|iPhone|3|Gustavo|Accardo|7/9/2018|São Paulo|5300|NaN|15900|
|1684|7557|HL9962|Android|1|Ana|Monte|6/26/2018|São Paulo|3400|NaN|3400|
|1685|7568|HL2714|Tablet|5|Beatriz|Cavalcanti|2/15/2018|São Paulo|1600|NaN|8000|
|1686|7569|HL4379|Televisão|2|Mariana|Baptista|6/19/2018|São Paulo|2500|NaN|5000|
|1687|7570|HL1918|iPhone|1|Milena|Almeida|6/24/2018|São Paulo|5300|NaN|5300|
|1688|7574|HL1918|iPhone|4|Wilson|Brandão|7/26/2018|São Paulo|5300|NaN|21200|
|1689|7577|HL2714|Tablet|2|Hanna|Fonseca|5/29/2018|São Paulo|1600|NaN|3200|
|1690|7582|HL4379|Televisão|3|Samara|Pinto|3/5/2018|São Paulo|2500|NaN|7500|
|1691|7583|HL7348|SmartWatch|1|Ana|Campos|12/17/2018|São Paulo|1400|NaN|1400|
|1692|7587|HL9962|Android|5|Luiz|Marinho|8/3/2018|São Paulo|3400|NaN|17000|
|1693|7601|HL1918|iPhone|2|Lívia|Marques|12/3/2018|São Paulo|5300|NaN|10600|
|1694|7610|HL1918|iPhone|3|Ana|Bôas|5/9/2018|São Paulo|5300|NaN|15900|
|1695|7623|HL1148|Câmera|4|Thales|Portillo|10/26/2018|São Paulo|2100|NaN|8400|
|1696|7638|HL1918|iPhone|4|Lucas|Baptista|7/11/2018|São Paulo|5300|NaN|21200|
|1697|7639|HL1918|iPhone|4|Paloma|Sperandei|3/16/2018|São Paulo|5300|NaN|21200|
|1698|7648|HL1148|Câmera|3|Catarina|Teixeira|6/10/2018|São Paulo|2100|NaN|6300|
|1699|7650|HL8851|Notebook|4|Rebeca|Reis|12/28/2018|São Paulo|3500|NaN|14000|
|1700|7654|HL1918|iPhone|3|Luiza|Johnson|10/31/2018|São Paulo|5300|NaN|15900|
|1701|7664|HL4379|Televisão|5|Carolina|Figueiredo|11/12/2018|São Paulo|2500|NaN|12500|
|1702|7666|HL1918|iPhone|2|Luiza|Farias|2/7/2018|São Paulo|5300|NaN|10600|
|1703|7680|HL1918|iPhone|4|Marcela|Medeiros|9/19/2018|São Paulo|5300|NaN|21200|
|1704|7683|HL7348|SmartWatch|4|Gabrielle|Wanderley|7/14/2018|São Paulo|1400|NaN|5600|
|1705|7695|HL8851|Notebook|2|Marcela|Medeiros|7/15/2018|São Paulo|3500|NaN|7000|
|1706|7698|HL1918|iPhone|3|Paula|Calbucci|9/19/2018|São Paulo|5300|NaN|15900|
|1707|7700|HL1918|iPhone|2|Rodrigo|Mendes|2/5/2018|São Paulo|5300|NaN|10600|
|1708|7707|HL1148|Câmera|5|Marcela|Gasperi|10/9/2018|São Paulo|2100|NaN|10500|
|1709|7709|HL1918|iPhone|1|Sthefeson|Kohn|3/9/2018|São Paulo|5300|NaN|5300|
|1710|7710|HL1918|iPhone|5|Juan|Fernandes|12/21/2018|São Paulo|5300|NaN|26500|
|1711|7711|HL2714|Tablet|3|Ana|Leite|11/28/2018|São Paulo|1600|NaN|4800|
|1712|7733|HL9962|Android|3|Julia|Leig|4/8/2018|São Paulo|3400|NaN|10200|
|1713|7734|HL9962|Android|3|Matheus|Ramos|11/3/2018|São Paulo|3400|NaN|10200|
|1714|7740|HL8851|Notebook|5|Diego|Barros|12/25/2018|São Paulo|3500|NaN|17500|
|1715|7741|HL2714|Tablet|1|Sandy|Moreira|3/19/2018|São Paulo|1600|NaN|1600|
|1716|7744|HL7348|SmartWatch|2|Thayane|Resende|8/15/2018|São Paulo|1400|NaN|2800|
|1717|7745|HL1148|Câmera|5|Jorge|Carvalho|2/27/2018|São Paulo|2100|NaN|10500|
|1718|7746|HL4379|Televisão|5|Rafael|Ramos|7/26/2018|São Paulo|2500|NaN|12500|
|1719|7749|HL1148|Câmera|1|Débora|Lopes|6/21/2018|São Paulo|2100|NaN|2100|
|1720|7753|HL9962|Android|2|Andressa|Rotsztejn|12/5/2018|São Paulo|3400|NaN|6800|
|1721|7754|HL1148|Câmera|1|Cézar|Santos|1/22/2018|São Paulo|2100|NaN|2100|
|1722|7757|HL7348|SmartWatch|3|Jônatas|Tanaka|11/14/2018|São Paulo|1400|NaN|4200|
|1723|7758|HL9962|Android|1|Dykson|Silva|1/8/2018|São Paulo|3400|NaN|3400|
|1724|7763|HL1918|iPhone|1|Victor|Oliveira|10/17/2018|São Paulo|5300|NaN|5300|
|1725|7771|HL4379|Televisão|4|Ives|Barbosa|4/2/2018|São Paulo|2500|NaN|10000|
|1726|7773|HL1918|iPhone|3|Diogo|Ressurreição|4/19/2018|São Paulo|5300|NaN|15900|
|1727|7786|HL1148|Câmera|3|Cláudio|Aragão|10/12/2018|São Paulo|2100|NaN|6300|
|1728|7787|HL7348|SmartWatch|5|Felipe|Cavalcanti|3/1/2018|São Paulo|1400|NaN|7000|
|1729|7789|HL9962|Android|1|Andre|Nóbrega|3/24/2018|São Paulo|3400|NaN|3400|
|1730|7794|HL1918|iPhone|2|Rodrigo|Silva|9/19/2018|São Paulo|5300|NaN|10600|
|1731|7806|HL4379|Televisão|5|Roberta|Pimenta|11/25/2018|São Paulo|2500|NaN|12500|
|1732|7807|HL9962|Android|3|Lucas|Machado|3/6/2018|São Paulo|3400|NaN|10200|
|1733|7810|HL4379|Televisão|4|Lívia|Tanaka|11/28/2018|São Paulo|2500|NaN|10000|
|1734|7813|HL1918|iPhone|5|Clara|Silveira|12/3/2018|São Paulo|5300|NaN|26500|
|1735|7814|HL7348|SmartWatch|4|Stephanie|Gonçalves|4/21/2018|São Paulo|1400|NaN|5600|
|1736|7818|HL8851|Notebook|4|Raíza|Lopes|3/25/2018|São Paulo|3500|NaN|14000|
|1737|7821|HL1918|iPhone|4|Victor|Oliveira|8/8/2018|São Paulo|5300|NaN|21200|
|1738|7822|HL1918|iPhone|5|Carlos|Barbosa|1/28/2018|São Paulo|5300|NaN|26500|
|1739|7826|HL4379|Televisão|1|Natalia|Accioly|7/20/2018|São Paulo|2500|NaN|2500|
|1740|7840|HL4379|Televisão|4|Lucas|Almeida|2/6/2018|São Paulo|2500|NaN|10000|
|1741|7843|HL1148|Câmera|3|Luíza|Goulart|10/9/2018|São Paulo|2100|NaN|6300|
|1742|7848|HL7348|SmartWatch|3|Victor|Zakhm|5/28/2018|São Paulo|1400|NaN|4200|
|1743|7853|HL1148|Câmera|3|Raissa|Pinheiro|9/1/2018|São Paulo|2100|NaN|6300|
|1744|7858|HL4379|Televisão|1|Guilherme|Barbosa|1/11/2018|São Paulo|2500|NaN|2500|
|1745|7861|HL1918|iPhone|5|Vitor|Boccaletti|1/27/2018|São Paulo|5300|NaN|26500|
|1746|7864|HL7348|SmartWatch|2|Stefan|Nunes|6/18/2018|São Paulo|1400|NaN|2800|
|1747|7868|HL4379|Televisão|3|Daniela|Pereira|6/2/2018|São Paulo|2500|NaN|7500|
|1748|7870|HL9962|Android|2|Thays|Castro|11/20/2018|São Paulo|3400|NaN|6800|
|1749|7873|HL1918|iPhone|4|Felipe|Mello|10/16/2018|São Paulo|5300|NaN|21200|
|1750|7874|HL1148|Câmera|4|Daniel|Araujo|12/12/2018|São Paulo|2100|NaN|8400|
|1751|7879|HL1918|iPhone|5|Pedro|Conceição|2/18/2018|São Paulo|5300|NaN|26500|
|1752|7882|HL4379|Televisão|2|Letícia|Leal|11/25/2018|São Paulo|2500|NaN|5000|
|1753|7885|HL8851|Notebook|4|Bernardo|Soares|11/30/2018|São Paulo|3500|NaN|14000|
|1754|7891|HL8851|Notebook|2|Thales|Andrade|11/19/2018|São Paulo|3500|NaN|7000|
|1755|7896|HL1918|iPhone|1|Arthur|Rocha|2/23/2018|São Paulo|5300|NaN|5300|
|1756|7906|HL7348|SmartWatch|4|Guilherme|Santos|2/23/2018|São Paulo|1400|NaN|5600|
|1757|7912|HL7348|SmartWatch|1|Rodrigo|Feijo|12/26/2018|São Paulo|1400|NaN|1400|
|1758|7914|HL4379|Televisão|3|Rodrigo|Ramos|10/8/2018|São Paulo|2500|NaN|7500|
|1759|7915|HL1918|iPhone|2|Livia|Cozendey|12/4/2018|São Paulo|5300|NaN|10600|
|1760|7927|HL4379|Televisão|2|João|Abraçado|4/24/2018|São Paulo|2500|NaN|5000|
|1761|7931|HL7348|SmartWatch|4|Maria|Moita|7/7/2018|São Paulo|1400|NaN|5600|
|1762|7934|HL2714|Tablet|4|Rafaela|Rodrigues|7/21/2018|São Paulo|1600|NaN|6400|
|1763|7940|HL7348|SmartWatch|1|Amanda|Procaci|10/10/2018|São Paulo|1400|NaN|1400|
|1764|7945|HL7348|SmartWatch|2|Hanna|Fonseca|7/14/2018|São Paulo|1400|NaN|2800|
|1765|7950|HL8851|Notebook|4|Thainá|Binello|2/26/2018|São Paulo|3500|NaN|14000|
|1766|7951|HL4379|Televisão|2|Daniela|Rosa|6/10/2018|São Paulo|2500|NaN|5000|
|1767|7953|HL2714|Tablet|5|Pedro|Santana|12/11/2018|São Paulo|1600|NaN|8000|
|1768|7955|HL1918|iPhone|5|Marcelo|Guadagnino|11/17/2018|São Paulo|5300|NaN|26500|
|1769|7967|HL2714|Tablet|4|Carlos|Barbosa|9/12/2018|São Paulo|1600|NaN|6400|
|1770|7973|HL9962|Android|5|Breno|Godoy|11/7/2018|São Paulo|3400|NaN|17000|
|1771|7976|HL1148|Câmera|5|Erick|Soares|8/14/2018|São Paulo|2100|NaN|10500|
|1772|7979|HL4379|Televisão|5|Eduardo|Soares|1/16/2018|São Paulo|2500|NaN|12500|
|1773|7984|HL1918|iPhone|3|Joao|Silva|6/8/2018|São Paulo|5300|NaN|15900|
|1774|7998|HL2714|Tablet|4|Alon|Pestana|3/16/2018|São Paulo|1600|NaN|6400|
|1775|7999|HL1918|iPhone|2|Victor|Oliveira|12/28/2018|São Paulo|5300|NaN|10600|
|1776|8003|HL1918|iPhone|5|Vittorio|Freitas|6/3/2018|São Paulo|5300|NaN|26500|
|1777|8010|HL1918|iPhone|3|Ana|Gomes|1/2/2018|São Paulo|5300|NaN|15900|
|1778|8016|HL2714|Tablet|2|Camille|Silva|11/12/2018|São Paulo|1600|NaN|3200|
|1779|8017|HL4379|Televisão|1|Jônatas|Soares|9/17/2018|São Paulo|2500|NaN|2500|
|1780|8021|HL1918|iPhone|2|Helena|Chafin|1/4/2018|São Paulo|5300|NaN|10600|
|1781|8023|HL1918|iPhone|3|Victor|Soares|1/28/2018|São Paulo|5300|NaN|15900|
|1782|8024|HL4379|Televisão|5|Eric|Júnior|6/19/2018|São Paulo|2500|NaN|12500|
|1783|8029|HL1918|iPhone|4|Pedro|Oliveira|5/24/2018|São Paulo|5300|NaN|21200|
|1784|8030|HL2714|Tablet|2|Lívia|Tanaka|4/3/2018|São Paulo|1600|NaN|3200|
|1785|8034|HL4379|Televisão|5|Lenon|Fernandes|4/8/2018|São Paulo|2500|NaN|12500|
|1786|8048|HL7348|SmartWatch|5|Isabella|Scalabrin|5/17/2018|São Paulo|1400|NaN|7000|
|1787|8049|HL1918|iPhone|5|Pedro|Oliveira|2/13/2018|São Paulo|5300|NaN|26500|
|1788|8050|HL1148|Câmera|5|Rodrigo|Silva|8/14/2018|São Paulo|2100|NaN|10500|
|1789|8053|HL1918|iPhone|2|Giovanna|Santos|4/11/2018|São Paulo|5300|NaN|10600|
|1790|8056|HL8851|Notebook|2|Sthefeson|Kohn|2/18/2018|São Paulo|3500|NaN|7000|
|1791|8061|HL8851|Notebook|2|Breno|Godoy|11/7/2018|São Paulo|3500|NaN|7000|
|1792|8068|HL1918|iPhone|4|Priscila|Garcia|4/17/2018|São Paulo|5300|NaN|21200|
|1793|8071|HL1148|Câmera|3|Marina|Perdomo|4/10/2018|São Paulo|2100|NaN|6300|
|1794|8072|HL9962|Android|1|Jorge|Carvalho|12/23/2018|São Paulo|3400|NaN|3400|
|1795|8075|HL7348|SmartWatch|1|Tainah|Nogueira|12/5/2018|São Paulo|1400|NaN|1400|
|1796|8076|HL8851|Notebook|4|Luíza|Melo|7/12/2018|São Paulo|3500|NaN|14000|
|1797|8077|HL8851|Notebook|4|Rafaela|Rodrigues|3/9/2018|São Paulo|3500|NaN|14000|
|1798|8087|HL1918|iPhone|5|Thayna|Martins|7/2/2018|São Paulo|5300|NaN|26500|
|1799|8096|HL1148|Câmera|1|Gabriel|Azevedo|3/3/2018|São Paulo|2100|NaN|2100|
|1800|8098|HL2714|Tablet|2|Caio|Cardoso|5/15/2018|São Paulo|1600|NaN|3200|
|1801|8102|HL8851|Notebook|1|Ylana|Teraoka|4/11/2018|São Paulo|3500|NaN|3500|
|1802|8105|HL4379|Televisão|5|Mariana|Miranda|8/14/2018|São Paulo|2500|NaN|12500|
|1803|8108|HL1918|iPhone|5|Roger|Rosa|3/15/2018|São Paulo|5300|NaN|26500|
|1804|8113|HL4379|Televisão|2|Anna|Silva|10/11/2018|São Paulo|2500|NaN|5000|
|1805|8122|HL1918|iPhone|1|Victor|Lira|7/7/2018|São Paulo|5300|NaN|5300|
|1806|8129|HL4379|Televisão|2|Matheus|Gomes|10/14/2018|São Paulo|2500|NaN|5000|
|1807|8135|HL4379|Televisão|2|Giovanna|Santos|8/3/2018|São Paulo|2500|NaN|5000|
|1808|8139|HL8851|Notebook|1|Isabelle|Gonçalves|4/28/2018|São Paulo|3500|NaN|3500|
|1809|8140|HL1918|iPhone|4|Maria|Gasperi|2/9/2018|São Paulo|5300|NaN|21200|
|1810|8144|HL2714|Tablet|1|Wen|Braga|9/16/2018|São Paulo|1600|NaN|1600|
|1811|8145|HL9962|Android|3|Pedro|Santos|10/18/2018|São Paulo|3400|NaN|10200|
|1812|8161|HL1918|iPhone|4|Luiz|Conceição|2/6/2018|São Paulo|5300|NaN|21200|
|1813|8163|HL4379|Televisão|5|Pedro|Cardoso|1/17/2018|São Paulo|2500|NaN|12500|
|1814|8172|HL1918|iPhone|5|Eduardo|Soares|9/5/2018|São Paulo|5300|NaN|26500|
|1815|8173|HL1918|iPhone|4|Diego|Marchesi|3/25/2018|São Paulo|5300|NaN|21200|
|1816|8179|HL1918|iPhone|5|Daniel|Nauenberg|7/8/2018|São Paulo|5300|NaN|26500|
|1817|8181|HL4379|Televisão|3|Maria|Motta|6/20/2018|São Paulo|2500|NaN|7500|
|1818|8182|HL9962|Android|1|Silvio|Provenzano|12/21/2018|São Paulo|3400|NaN|3400|
|1819|8187|HL1148|Câmera|1|Caio|Moraes|1/3/2018|São Paulo|2100|NaN|2100|
|1820|8193|HL8851|Notebook|1|Tainah|Nogueira|4/3/2018|São Paulo|3500|NaN|3500|
|1821|8194|HL1918|iPhone|3|Caio|Vianna|9/3/2018|São Paulo|5300|NaN|15900|
|1822|8198|HL1918|iPhone|2|João|Luz|7/22/2018|São Paulo|5300|NaN|10600|
|1823|8200|HL1918|iPhone|3|Bianca|Allevato|10/22/2018|São Paulo|5300|NaN|15900|
|1824|8209|HL1148|Câmera|3|Thales|Fanara|8/28/2018|São Paulo|2100|NaN|6300|
|1825|8213|HL2714|Tablet|3|Carlos|Azevedo|4/1/2018|São Paulo|1600|NaN|4800|
|1826|8217|HL1918|iPhone|5|Jeferson|Costa|3/28/2018|São Paulo|5300|NaN|26500|
|1827|8221|HL1918|iPhone|5|Chan|Santos|6/20/2018|São Paulo|5300|NaN|26500|
|1828|8223|HL1918|iPhone|5|Raphael|Guedes|7/26/2018|São Paulo|5300|NaN|26500|
|1829|8225|HL8851|Notebook|5|Carolina|Brum|3/5/2018|São Paulo|3500|NaN|17500|
|1830|8234|HL7348|SmartWatch|4|Eric|Carvalho|10/16/2018|São Paulo|1400|NaN|5600|
|1831|8236|HL2714|Tablet|4|Guilherme|Castilho|12/9/2018|São Paulo|1600|NaN|6400|
|1832|8242|HL9962|Android|4|Gustavo|Guimarães|10/16/2018|São Paulo|3400|NaN|13600|
|1833|8253|HL1918|iPhone|5|Sylvio|Bernhardt|12/19/2018|São Paulo|5300|NaN|26500|
|1834|8258|HL1918|iPhone|4|Cícero|Ramos|12/24/2018|São Paulo|5300|NaN|21200|
|1835|8266|HL4379|Televisão|2|Diego|Marchesi|9/30/2018|São Paulo|2500|NaN|5000|
|1836|8267|HL2714|Tablet|1|Felipe|Mendonça|2/28/2018|São Paulo|1600|NaN|1600|
|1837|8270|HL8851|Notebook|5|Marcela|Gasperi|6/16/2018|São Paulo|3500|NaN|17500|
|1838|8271|HL4379|Televisão|3|Sandy|Figueiredo|12/6/2018|São Paulo|2500|NaN|7500|
|1839|8274|HL1148|Câmera|2|Carla|Zakhm|9/1/2018|São Paulo|2100|NaN|4200|
|1840|8276|HL1148|Câmera|2|Luã|Sá|1/31/2018|São Paulo|2100|NaN|4200|
|1841|8281|HL1148|Câmera|4|Vanessa|Rodrigues|8/13/2018|São Paulo|2100|NaN|8400|
|1842|8298|HL1918|iPhone|2|Catarina|Teixeira|7/27/2018|São Paulo|5300|NaN|10600|
|1843|8303|HL1918|iPhone|5|Daniel|Ortiz|1/7/2018|São Paulo|5300|NaN|26500|
|1844|8306|HL1918|iPhone|4|Caio|Vianna|12/16/2018|São Paulo|5300|NaN|21200|
|1845|8316|HL9962|Android|1|Andre|Sampaio|3/30/2018|São Paulo|3400|NaN|3400|
|1846|8319|HL7348|SmartWatch|1|Breno|Godoy|3/4/2018|São Paulo|1400|NaN|1400|
|1847|8322|HL8851|Notebook|2|Daniel|Terra|10/9/2018|São Paulo|3500|NaN|7000|
|1848|8323|HL7348|SmartWatch|1|Bruno|Oliveira|5/16/2018|São Paulo|1400|NaN|1400|
|1849|8325|HL1918|iPhone|2|André|Alves|8/15/2018|São Paulo|5300|NaN|10600|
|1850|8327|HL2714|Tablet|2|Rebeca|Manhães|4/3/2018|São Paulo|1600|NaN|3200|
|1851|8330|HL4379|Televisão|4|Thaís|Moura|12/1/2018|São Paulo|2500|NaN|10000|
|1852|8331|HL2714|Tablet|4|Bernardo|Botelho|3/21/2018|São Paulo|1600|NaN|6400|
|1853|8334|HL8851|Notebook|2|Antônio|Soares|9/20/2018|São Paulo|3500|NaN|7000|
|1854|8344|HL8851|Notebook|1|Diego|Barros|10/30/2018|São Paulo|3500|NaN|3500|
|1855|8346|HL4379|Televisão|1|Adriana|Carneiro|9/11/2018|São Paulo|2500|NaN|2500|
|1856|8347|HL1918|iPhone|1|Bruna|Ramos|3/20/2018|São Paulo|5300|NaN|5300|
|1857|8353|HL2714|Tablet|4|Vitor|Arruda|12/30/2018|São Paulo|1600|NaN|6400|
|1858|8354|HL1918|iPhone|5|Rodrigo|Ramos|11/25/2018|São Paulo|5300|NaN|26500|
|1859|8361|HL2714|Tablet|3|Diego|Barros|6/10/2018|São Paulo|1600|NaN|4800|
|1860|8364|HL7348|SmartWatch|5|Hanna|Fonseca|12/31/2018|São Paulo|1400|NaN|7000|
|1861|8369|HL8851|Notebook|1|Raphael|Filho|11/23/2018|São Paulo|3500|NaN|3500|
|1862|8375|HL9962|Android|5|Bruno|Souza|10/8/2018|São Paulo|3400|NaN|17000|
|1863|8378|HL8851|Notebook|2|Beatriz|Cavalcanti|9/11/2018|São Paulo|3500|NaN|7000|
|1864|8379|HL4379|Televisão|1|David|Assumpção|12/26/2018|São Paulo|2500|NaN|2500|
|1865|8380|HL1918|iPhone|4|Lucas|Araújo|9/12/2018|São Paulo|5300|NaN|21200|
|1866|8388|HL8851|Notebook|2|Gustavo|Gomes|11/4/2018|São Paulo|3500|NaN|7000|
|1867|8392|HL1918|iPhone|2|Rafael|Guimarães|5/2/2018|São Paulo|5300|NaN|10600|
|1868|8394|HL4379|Televisão|3|Lívia|Tanaka|11/7/2018|São Paulo|2500|NaN|7500|
|1869|8399|HL7348|SmartWatch|1|Lucas|Freire|11/3/2018|São Paulo|1400|NaN|1400|
|1870|8408|HL9962|Android|4|Livia|Cozendey|4/29/2018|São Paulo|3400|NaN|13600|
|1871|8409|HL1918|iPhone|1|Lucas|Araújo|4/14/2018|São Paulo|5300|NaN|5300|
|1872|8411|HL1148|Câmera|3|Lenon|Fernandes|3/27/2018|São Paulo|2100|NaN|6300|
|1873|8417|HL1918|iPhone|3|Juliana|Hollander|5/17/2018|São Paulo|5300|NaN|15900|
|1874|8420|HL1918|iPhone|4|Thaís|Moura|10/9/2018|São Paulo|5300|NaN|21200|
|1875|8425|HL1918|iPhone|3|Bruna|Franco|7/30/2018|São Paulo|5300|NaN|15900|
|1876|8445|HL8851|Notebook|4|Luiz|Xavier|11/6/2018|São Paulo|3500|NaN|14000|
|1877|8448|HL4379|Televisão|1|Gabrielle|Silva|4/29/2018|São Paulo|2500|NaN|2500|
|1878|8449|HL9962|Android|2|Gustavo|Thome|1/27/2018|São Paulo|3400|NaN|6800|
|1879|8451|HL9962|Android|3|Lucas|Freitas|9/6/2018|São Paulo|3400|NaN|10200|
|1880|8457|HL1918|iPhone|2|Stephanie|Novak|9/27/2018|São Paulo|5300|NaN|10600|
|1881|8460|HL1918|iPhone|4|Matheus|Gomes|10/16/2018|São Paulo|5300|NaN|21200|
|1882|8461|HL9962|Android|2|Gabriella|Sagrillo|10/19/2018|São Paulo|3400|NaN|6800|
|1883|8463|HL1918|iPhone|3|Julia|Aliani|11/12/2018|São Paulo|5300|NaN|15900|
|1884|8466|HL8851|Notebook|3|Bruno|Barcessat|12/31/2018|São Paulo|3500|NaN|10500|
|1885|8471|HL4379|Televisão|5|Julie|Ferreira|6/21/2018|São Paulo|2500|NaN|12500|
|1886|8473|HL4379|Televisão|4|Audir|Franco|8/23/2018|São Paulo|2500|NaN|10000|
|1887|8475|HL1918|iPhone|4|Bárbara|Cavalcante|2/2/2018|São Paulo|5300|NaN|21200|
|1888|8479|HL1148|Câmera|3|Rafaela|Ferreira|12/28/2018|São Paulo|2100|NaN|6300|
|1889|8480|HL1148|Câmera|4|Fernanda|Junior|3/20/2018|São Paulo|2100|NaN|8400|
|1890|8481|HL1918|iPhone|5|Gustavo|Guimarães|12/13/2018|São Paulo|5300|NaN|26500|
|1891|8486|HL9962|Android|4|Victor|Ferreira|12/16/2018|São Paulo|3400|NaN|13600|
|1892|8487|HL8851|Notebook|3|Mariane|Racy|9/17/2018|São Paulo|3500|NaN|10500|
|1893|8495|HL7348|SmartWatch|2|Sthefeson|Kohn|1/25/2018|São Paulo|1400|NaN|2800|
|1894|8503|HL4379|Televisão|2|Pedro|Cardoso|8/8/2018|São Paulo|2500|NaN|5000|
|1895|8506|HL1918|iPhone|3|João|Silva|9/1/2018|São Paulo|5300|NaN|15900|
|1896|8512|HL4379|Televisão|2|Beatriz|Almeida|6/22/2018|São Paulo|2500|NaN|5000|
|1897|8513|HL2714|Tablet|3|Milena|Almeida|9/1/2018|São Paulo|1600|NaN|4800|
|1898|8514|HL1918|iPhone|2|Alessandra|Martins|6/7/2018|São Paulo|5300|NaN|10600|
|1899|8515|HL1148|Câmera|1|Lorena|Kohn|4/1/2018|São Paulo|2100|NaN|2100|
|1900|8516|HL1918|iPhone|4|Vinícius|Antunes|2/14/2018|São Paulo|5300|NaN|21200|
|1901|8525|HL2714|Tablet|4|Giovanna|Santos|11/10/2018|São Paulo|1600|NaN|6400|
|1902|8530|HL1918|iPhone|5|Lucas|Neto|6/27/2018|São Paulo|5300|NaN|26500|
|1903|8535|HL9962|Android|3|Sthefeson|Pereira|4/7/2018|São Paulo|3400|NaN|10200|
|1904|8542|HL9962|Android|4|Luiz|Campista|11/22/2018|São Paulo|3400|NaN|13600|
|1905|8549|HL1918|iPhone|5|Lucas|Cavalcanti|3/6/2018|São Paulo|5300|NaN|26500|
|1906|8557|HL9962|Android|5|Henrique|Oliveira|12/30/2018|São Paulo|3400|NaN|17000|
|1907|8563|HL4379|Televisão|1|Adrielle|Gabriel|1/3/2018|São Paulo|2500|NaN|2500|
|1908|8564|HL9962|Android|5|João|Júnior|1/24/2018|São Paulo|3400|NaN|17000|
|1909|8565|HL1148|Câmera|1|Lara|Moreira|4/23/2018|São Paulo|2100|NaN|2100|
|1910|8566|HL8851|Notebook|3|Thayane|Resende|3/14/2018|São Paulo|3500|NaN|10500|
|1911|8571|HL8851|Notebook|2|Pedro|Martins|1/8/2018|São Paulo|3500|NaN|7000|
|1912|8572|HL4379|Televisão|5|Matheus|Moraes|6/17/2018|São Paulo|2500|NaN|12500|
|1913|8587|HL7348|SmartWatch|2|Guilherme|Rachide|6/16/2018|São Paulo|1400|NaN|2800|
|1914|8592|HL4379|Televisão|2|Raíza|Lopes|3/13/2018|São Paulo|2500|NaN|5000|
|1915|8614|HL9962|Android|4|Desirée|Heimlich|4/10/2018|São Paulo|3400|NaN|13600|
|1916|8616|HL7348|SmartWatch|1|Michelle|Miura|6/1/2018|São Paulo|1400|NaN|1400|
|1917|8619|HL1918|iPhone|4|Victor|Ferreira|3/15/2018|São Paulo|5300|NaN|21200|
|1918|8626|HL1918|iPhone|1|Julia|Leig|8/7/2018|São Paulo|5300|NaN|5300|
|1919|8627|HL4379|Televisão|3|Caroline|Delgado|11/19/2018|São Paulo|2500|NaN|7500|
|1920|8628|HL9962|Android|3|Gabrielle|Figueiredo|7/28/2018|São Paulo|3400|NaN|10200|
|1921|8630|HL1148|Câmera|2|Eduardo|Lopes|8/7/2018|São Paulo|2100|NaN|4200|
|1922|8631|HL1148|Câmera|3|Eduardo|Pacheco|11/15/2018|São Paulo|2100|NaN|6300|
|1923|8637|HL8851|Notebook|2|Diego|Marchesi|5/25/2018|São Paulo|3500|NaN|7000|
|1924|8643|HL1918|iPhone|2|Carolina|Bernardes|9/13/2018|São Paulo|5300|NaN|10600|
|1925|8644|HL9962|Android|5|Larissa|Nauenberg|1/2/2018|São Paulo|3400|NaN|17000|
|1926|8646|HL1918|iPhone|4|Raphael|Ferman|10/1/2018|São Paulo|5300|NaN|21200|
|1927|8649|HL2714|Tablet|2|Luis|Garcia|11/7/2018|São Paulo|1600|NaN|3200|
|1928|8657|HL4379|Televisão|4|Gabriel|Assis|9/29/2018|São Paulo|2500|NaN|10000|
|1929|8659|HL1918|iPhone|2|Bruno|Oliveira|7/25/2018|São Paulo|5300|NaN|10600|
|1930|8680|HL1918|iPhone|2|Isabela|Resende|5/3/2018|São Paulo|5300|NaN|10600|
|1931|8686|HL1918|iPhone|5|José|Carvalho|3/7/2018|São Paulo|5300|NaN|26500|
|1932|8691|HL1148|Câmera|5|Diogo|Ressurreição|8/13/2018|São Paulo|2100|NaN|10500|
|1933|8696|HL4379|Televisão|1|Iuri|Neto|8/14/2018|São Paulo|2500|NaN|2500|
|1934|8699|HL1918|iPhone|1|Paula|Cavalcanti|4/15/2018|São Paulo|5300|NaN|5300|
|1935|8700|HL7348|SmartWatch|5|Julia|Silva|9/27/2018|São Paulo|1400|NaN|7000|
|1936|8703|HL1918|iPhone|3|Fernanda|Figueiredo|9/27/2018|São Paulo|5300|NaN|15900|
|1937|8722|HL1918|iPhone|1|Anna|Silva|10/29/2018|São Paulo|5300|NaN|5300|
|1938|8731|HL8851|Notebook|2|Bianca|Piero|2/17/2018|São Paulo|3500|NaN|7000|
|1939|8735|HL1918|iPhone|1|Pedro|Xavier|4/24/2018|São Paulo|5300|NaN|5300|
|1940|8737|HL7348|SmartWatch|1|João|Rodrigues|1/24/2018|São Paulo|1400|NaN|1400|
|1941|8744|HL7348|SmartWatch|5|Carolina|Alfradique|12/3/2018|São Paulo|1400|NaN|7000|
|1942|8752|HL1918|iPhone|3|Lucas|Assunção|3/27/2018|São Paulo|5300|NaN|15900|
|1943|8753|HL8851|Notebook|5|Lenon|Fernandes|2/17/2018|São Paulo|3500|NaN|17500|
|1944|8755|HL1918|iPhone|4|Wilson|Brandão|12/14/2018|São Paulo|5300|NaN|21200|
|1945|8759|HL1918|iPhone|5|Bernardo|Nauenberg|7/13/2018|São Paulo|5300|NaN|26500|
|1946|8762|HL2714|Tablet|4|Patrícia|Fernandes|6/24/2018|São Paulo|1600|NaN|6400|
|1947|8764|HL9962|Android|4|Isabella|Scalabrin|1/28/2018|São Paulo|3400|NaN|13600|
|1948|8765|HL1918|iPhone|2|Adrielle|Vieira|1/22/2018|São Paulo|5300|NaN|10600|
|1949|8766|HL2714|Tablet|1|Camille|Silva|2/18/2018|São Paulo|1600|NaN|1600|
|1950|8767|HL9962|Android|2|Marina|Marins|8/27/2018|São Paulo|3400|NaN|6800|
|1951|8768|HL1148|Câmera|3|Camille|Silva|6/22/2018|São Paulo|2100|NaN|6300|
|1952|8769|HL9962|Android|5|Roberto|Tiradentes|1/19/2018|São Paulo|3400|NaN|17000|
|1953|8770|HL4379|Televisão|5|Caio|Fernandes|2/20/2018|São Paulo|2500|NaN|12500|
|1954|8771|HL7348|SmartWatch|4|Matheus|Gomes|9/9/2018|São Paulo|1400|NaN|5600|
|1955|8776|HL9962|Android|2|Fernanda|Rubim|2/14/2018|São Paulo|3400|NaN|6800|
|1956|8777|HL1918|iPhone|2|Marina|Marins|4/12/2018|São Paulo|5300|NaN|10600|
|1957|8779|HL1918|iPhone|3|Karina|Camara|3/7/2018|São Paulo|5300|NaN|15900|
|1958|8780|HL4379|Televisão|3|Luiz|Xavier|10/20/2018|São Paulo|2500|NaN|7500|
|1959|8785|HL1918|iPhone|5|Antônio|Oliveira|12/21/2018|São Paulo|5300|NaN|26500|
|1960|8786|HL1918|iPhone|4|Guilherme|Rachide|7/20/2018|São Paulo|5300|NaN|21200|
|1961|8790|HL1918|iPhone|4|João|Bach|8/10/2018|São Paulo|5300|NaN|21200|
|1962|8794|HL2714|Tablet|3|Giuseppe|Bhering|12/17/2018|São Paulo|1600|NaN|4800|
|1963|8805|HL4379|Televisão|4|Hygor|Essaber|7/30/2018|São Paulo|2500|NaN|10000|
|1964|8807|HL4379|Televisão|4|Raíssa|Oliveira|6/27/2018|São Paulo|2500|NaN|10000|
|1965|8811|HL1918|iPhone|1|Paula|Cavalcanti|2/8/2018|São Paulo|5300|NaN|5300|
|1966|8812|HL9962|Android|4|Eduardo|Nunes|7/25/2018|São Paulo|3400|NaN|13600|
|1967|8813|HL1918|iPhone|2|Bianca|Ferezin|5/31/2018|São Paulo|5300|NaN|10600|
|1968|8815|HL1918|iPhone|5|Danilo|Alves|5/26/2018|São Paulo|5300|NaN|26500|
|1969|8816|HL9962|Android|3|Renan|Cunha|6/30/2018|São Paulo|3400|NaN|10200|
|1970|8818|HL1918|iPhone|1|Matheus|Delgado|3/3/2018|São Paulo|5300|NaN|5300|
|1971|8839|HL7348|SmartWatch|5|Juliana|Barreira|10/9/2018|São Paulo|1400|NaN|7000|
|1972|8851|HL4379|Televisão|1|Eduardo|Soares|6/22/2018|São Paulo|2500|NaN|2500|
|1973|8854|HL2714|Tablet|2|Joyce|Souza|4/19/2018|São Paulo|1600|NaN|3200|
|1974|8856|HL1918|iPhone|1|Tainah|Nogueira|3/26/2018|São Paulo|5300|NaN|5300|
|1975|8857|HL1148|Câmera|3|Tiago|Pereira|6/22/2018|São Paulo|2100|NaN|6300|
|1976|8863|HL7348|SmartWatch|3|Danilo|Rubim|7/5/2018|São Paulo|1400|NaN|4200|
|1977|8876|HL1918|iPhone|3|Caroline|Delgado|11/26/2018|São Paulo|5300|NaN|15900|
|1978|8882|HL8851|Notebook|5|Rafaella|Mello|10/2/2018|São Paulo|3500|NaN|17500|
|1979|8883|HL1918|iPhone|3|Bruno|Temporal|2/27/2018|São Paulo|5300|NaN|15900|
|1980|8884|HL4379|Televisão|1|Bruna|Ramos|11/14/2018|São Paulo|2500|NaN|2500|
|1981|8891|HL9962|Android|1|Roger|Rosa|2/5/2018|São Paulo|3400|NaN|3400|
|1982|8897|HL7348|SmartWatch|5|Raissa|Maia|5/17/2018|São Paulo|1400|NaN|7000|
|1983|8901|HL8851|Notebook|5|Gabriella|Sagrillo|6/28/2018|São Paulo|3500|NaN|17500|
|1984|8904|HL1918|iPhone|1|Stela|Mendonça|8/6/2018|São Paulo|5300|NaN|5300|
|1985|8907|HL4379|Televisão|1|Carlos|Mesquita|10/24/2018|São Paulo|2500|NaN|2500|
|1986|8908|HL2714|Tablet|2|Cassio|Faria|2/25/2018|São Paulo|1600|NaN|3200|
|1987|8909|HL2714|Tablet|3|Stephanie|Novak|3/8/2018|São Paulo|1600|NaN|4800|
|1988|8910|HL1148|Câmera|5|Débora|Lopes|5/25/2018|São Paulo|2100|NaN|10500|
|1989|8911|HL1918|iPhone|3|Rafael|Carneiro|10/29/2018|São Paulo|5300|NaN|15900|
|1990|8923|HL1918|iPhone|1|Wilson|Meirelles|12/25/2018|São Paulo|5300|NaN|5300|
|1991|8924|HL9962|Android|3|Ana|Gomes|12/5/2018|São Paulo|3400|NaN|10200|
|1992|8925|HL1918|iPhone|5|Victor|Ferreira|8/4/2018|São Paulo|5300|NaN|26500|
|1993|8933|HL1148|Câmera|3|Camilla|Guimarães|6/5/2018|São Paulo|2100|NaN|6300|
|1994|8935|HL4379|Televisão|1|Lucas|Araújo|9/13/2018|São Paulo|2500|NaN|2500|
|1995|8952|HL1918|iPhone|5|Rubens|Netto|1/4/2018|São Paulo|5300|NaN|26500|
|1996|8958|HL4379|Televisão|5|Thiago|Lima|6/23/2018|São Paulo|2500|NaN|12500|
|1997|8960|HL9962|Android|3|Amanda|Felippe|3/24/2018|São Paulo|3400|NaN|10200|
|1998|8966|HL4379|Televisão|3|Nina|Magalhães|12/29/2018|São Paulo|2500|NaN|7500|
|1999|8970|HL9962|Android|1|Marina|Gama|3/13/2018|São Paulo|3400|NaN|3400|
|2000|8982|HL1148|Câmera|1|Camilla|Vieira|1/6/2018|São Paulo|2100|NaN|2100|
|2001|8983|HL9962|Android|3|Tiago|Pereira|6/15/2018|São Paulo|3400|NaN|10200|
|2002|8992|HL9962|Android|1|Eduardo|Nunes|5/16/2018|São Paulo|3400|NaN|3400|
|2003|8996|HL9962|Android|4|Pedro|Costa|11/29/2018|São Paulo|3400|NaN|13600|
|2004|8997|HL4379|Televisão|1|Lucas|Coelho|11/10/2018|São Paulo|2500|NaN|2500|
|2005|9001|HL1148|Câmera|2|Luíza|Melo|4/22/2018|São Paulo|2100|NaN|4200|
|2006|9007|HL8851|Notebook|4|Chan|Santos|1/7/2018|São Paulo|3500|NaN|14000|
|2007|9010|HL7348|SmartWatch|1|Rodrigo|Mendes|7/18/2018|São Paulo|1400|NaN|1400|
|2008|9016|HL1918|iPhone|3|Wendela|Mariz|2/6/2018|São Paulo|5300|NaN|15900|
|2009|9018|HL4379|Televisão|5|Lais|Candido|12/28/2018|São Paulo|2500|NaN|12500|
|2010|9019|HL2714|Tablet|2|Joao|Silva|9/20/2018|São Paulo|1600|NaN|3200|
|2011|9031|HL4379|Televisão|5|Karina|Camara|8/9/2018|São Paulo|2500|NaN|12500|
|2012|9032|HL7348|SmartWatch|5|Guilherme|Lima|2/28/2018|São Paulo|1400|NaN|7000|
|2013|9033|HL8851|Notebook|3|Guilherme|Lima|6/10/2018|São Paulo|3500|NaN|10500|
|2014|9034|HL9962|Android|2|Caio|Moura|9/15/2018|São Paulo|3400|NaN|6800|
|2015|9035|HL1918|iPhone|4|Laura|Araujo|11/21/2018|São Paulo|5300|NaN|21200|
|2016|9038|HL4379|Televisão|5|Kim|Ferreira|4/13/2018|São Paulo|2500|NaN|12500|
|2017|9042|HL1918|iPhone|4|Caio|Vianna|4/28/2018|São Paulo|5300|NaN|21200|
|2018|9049|HL8851|Notebook|4|Bianca|Piero|3/30/2018|São Paulo|3500|NaN|14000|
|2019|9054|HL8851|Notebook|3|Eduardo|Peluzo|2/20/2018|São Paulo|3500|NaN|10500|
|2020|9056|HL8851|Notebook|1|Isabella|Montanholi|7/21/2018|São Paulo|3500|NaN|3500|
|2021|9057|HL7348|SmartWatch|3|Thomaz|Ferreira|10/10/2018|São Paulo|1400|NaN|4200|
|2022|9059|HL1918|iPhone|3|Marina|Correa|7/25/2018|São Paulo|5300|NaN|15900|
|2023|9060|HL1918|iPhone|1|Bianca|Paz|9/5/2018|São Paulo|5300|NaN|5300|
|2024|9066|HL1918|iPhone|3|Carolina|Motta|1/5/2018|São Paulo|5300|NaN|15900|
|2025|9075|HL4379|Televisão|5|Thales|Portillo|7/31/2018|São Paulo|2500|NaN|12500|
|2026|9078|HL2714|Tablet|5|Adrielle|Vieira|1/23/2018|São Paulo|1600|NaN|8000|
|2027|9089|HL2714|Tablet|5|Lucas|Junior|5/4/2018|São Paulo|1600|NaN|8000|
|2028|9090|HL7348|SmartWatch|3|Isabel|Leite|4/13/2018|São Paulo|1400|NaN|4200|
|2029|9094|HL7348|SmartWatch|5|Thays|Castro|5/12/2018|São Paulo|1400|NaN|7000|
|2030|9097|HL1918|iPhone|2|Isabel|Leite|6/17/2018|São Paulo|5300|NaN|10600|
|2031|9104|HL9962|Android|4|Glenda|Santos|7/18/2018|São Paulo|3400|NaN|13600|
|2032|9106|HL1918|iPhone|1|Caio|Silva|1/22/2018|São Paulo|5300|NaN|5300|
|2033|9110|HL7348|SmartWatch|2|Andressa|Nóbrega|11/3/2018|São Paulo|1400|NaN|2800|
|2034|9114|HL2714|Tablet|5|Izabel|Lopes|8/9/2018|São Paulo|1600|NaN|8000|
|2035|9118|HL8851|Notebook|2|Matheus|Silva|5/9/2018|São Paulo|3500|NaN|7000|
|2036|9121|HL1918|iPhone|3|Ulisses|Quinto|10/10/2018|São Paulo|5300|NaN|15900|
|2037|9122|HL8851|Notebook|3|Victor|Gomes|11/18/2018|São Paulo|3500|NaN|10500|
|2038|9125|HL8851|Notebook|2|Raphael|Ferman|1/7/2018|São Paulo|3500|NaN|7000|
|2039|9127|HL8851|Notebook|3|Lucas|Destri|3/28/2018|São Paulo|3500|NaN|10500|
|2040|9128|HL8851|Notebook|4|Juliana|Correa|8/16/2018|São Paulo|3500|NaN|14000|
|2041|9129|HL2714|Tablet|2|Luiza|Cabral|3/19/2018|São Paulo|1600|NaN|3200|
|2042|9130|HL4379|Televisão|2|João|Matheus|6/11/2018|São Paulo|2500|NaN|5000|
|2043|9131|HL4379|Televisão|4|Gabriel|Soares|10/3/2018|São Paulo|2500|NaN|10000|
|2044|9135|HL1918|iPhone|4|Marcelo|Borges|8/11/2018|São Paulo|5300|NaN|21200|
|2045|9139|HL9962|Android|3|Natalia|Andrade|9/5/2018|São Paulo|3400|NaN|10200|
|2046|9140|HL1918|iPhone|1|Juliana|Hollander|3/22/2018|São Paulo|5300|NaN|5300|
|2047|9145|HL1918|iPhone|5|Rafaela|Gonçalves|1/22/2018|São Paulo|5300|NaN|26500|
|2048|9146|HL2714|Tablet|5|Julia|Penteado|10/28/2018|São Paulo|1600|NaN|8000|
|2049|9147|HL7348|SmartWatch|3|Priscila|Carvalho|8/15/2018|São Paulo|1400|NaN|4200|
|2050|9156|HL4379|Televisão|2|Miguel|Carneiro|7/14/2018|São Paulo|2500|NaN|5000|
|2051|9168|HL1918|iPhone|5|Matheus|Moraes|7/29/2018|São Paulo|5300|NaN|26500|
|2052|9171|HL2714|Tablet|5|Eduardo|Ferreira|2/26/2018|São Paulo|1600|NaN|8000|
|2053|9177|HL2714|Tablet|4|Anna|Maia|10/11/2018|São Paulo|1600|NaN|6400|
|2054|9179|HL2714|Tablet|1|Bruno|Barcessat|12/26/2018|São Paulo|1600|NaN|1600|
|2055|9181|HL1148|Câmera|1|Jonatas|Essaber|1/26/2018|São Paulo|2100|NaN|2100|
|2056|9196|HL9962|Android|4|José|Jesus|5/5/2018|São Paulo|3400|NaN|13600|
|2057|9209|HL9962|Android|2|João|Bach|3/26/2018|São Paulo|3400|NaN|6800|
|2058|9214|HL2714|Tablet|3|Caroline|Pinto|5/6/2018|São Paulo|1600|NaN|4800|
|2059|9223|HL7348|SmartWatch|4|Victor|Lira|6/21/2018|São Paulo|1400|NaN|5600|
|2060|9235|HL2714|Tablet|3|Dykson|Silva|4/11/2018|São Paulo|1600|NaN|4800|
|2061|9236|HL1918|iPhone|3|Gabriela|Cavalcanti|1/20/2018|São Paulo|5300|NaN|15900|
|2062|9242|HL1918|iPhone|3|Lucas|Costa|8/14/2018|São Paulo|5300|NaN|15900|
|2063|9244|HL7348|SmartWatch|4|Gabriel|Thome|3/25/2018|São Paulo|1400|NaN|5600|
|2064|9250|HL4379|Televisão|3|Victor|Gomes|9/9/2018|São Paulo|2500|NaN|7500|
|2065|9264|HL7348|SmartWatch|4|David|Campelo|7/4/2018|São Paulo|1400|NaN|5600|
|2066|9276|HL1148|Câmera|4|Guilherme|Monteiro|11/7/2018|São Paulo|2100|NaN|8400|
|2067|9291|HL1918|iPhone|3|Fernanda|Silva|12/19/2018|São Paulo|5300|NaN|15900|
|2068|9296|HL1918|iPhone|2|Marcos|Nucci|1/20/2018|São Paulo|5300|NaN|10600|
|2069|9302|HL1918|iPhone|3|Bruno|Temporal|6/25/2018|São Paulo|5300|NaN|15900|
|2070|9306|HL2714|Tablet|2|Raissa|Pinheiro|12/13/2018|São Paulo|1600|NaN|3200|
|2071|9307|HL8851|Notebook|4|Ives|Pinheiro|12/14/2018|São Paulo|3500|NaN|14000|
|2072|9312|HL4379|Televisão|5|Arthur|Souza|4/23/2018|São Paulo|2500|NaN|12500|
|2073|9315|HL2714|Tablet|2|Elaine|Santos|10/4/2018|São Paulo|1600|NaN|3200|
|2074|9330|HL7348|SmartWatch|5|Gabrielle|Porto|2/25/2018|São Paulo|1400|NaN|7000|
|2075|9335|HL1918|iPhone|5|Ana|Carvalho|7/17/2018|São Paulo|5300|NaN|26500|
|2076|9336|HL2714|Tablet|5|Patrick|Silva|9/9/2018|São Paulo|1600|NaN|8000|
|2077|9337|HL9962|Android|4|Gabrielle|Vasconcelos|2/28/2018|São Paulo|3400|NaN|13600|
|2078|9338|HL4379|Televisão|4|Bruno|Oliveira|9/27/2018|São Paulo|2500|NaN|10000|
|2079|9340|HL8851|Notebook|1|Camille|Silva|8/12/2018|São Paulo|3500|NaN|3500|
|2080|9342|HL1918|iPhone|4|Rodrigo|Silva|9/11/2018|São Paulo|5300|NaN|21200|
|2081|9346|HL4379|Televisão|3|Roberto|Mattos|8/27/2018|São Paulo|2500|NaN|7500|
|2082|9350|HL1148|Câmera|3|Manuela|Merege|12/9/2018|São Paulo|2100|NaN|6300|
|2083|9352|HL1918|iPhone|2|Roger|Rosa|9/18/2018|São Paulo|5300|NaN|10600|
|2084|9357|HL8851|Notebook|3|Fernanda|Bhering|1/12/2018|São Paulo|3500|NaN|10500|
|2085|9359|HL1148|Câmera|4|Jéssica|Teixeira|12/20/2018|São Paulo|2100|NaN|8400|
|2086|9360|HL1918|iPhone|2|Lucas|Junior|12/1/2018|São Paulo|5300|NaN|10600|
|2087|9363|HL1918|iPhone|1|Jeferson|Sone|9/15/2018|São Paulo|5300|NaN|5300|
|2088|9365|HL7348|SmartWatch|2|Beatriz|Rodrigues|5/26/2018|São Paulo|1400|NaN|2800|
|2089|9366|HL8851|Notebook|2|Lorena|Kohn|3/12/2018|São Paulo|3500|NaN|7000|
|2090|9370|HL1918|iPhone|2|Luíza|Melo|5/1/2018|São Paulo|5300|NaN|10600|
|2091|9379|HL1918|iPhone|1|Gabriela|Fernandes|5/18/2018|São Paulo|5300|NaN|5300|
|2092|9383|HL1918|iPhone|5|Izabel|Miura|7/19/2018|São Paulo|5300|NaN|26500|
|2093|9386|HL1918|iPhone|1|Pedro|Rodrigues|9/25/2018|São Paulo|5300|NaN|5300|
|2094|9388|HL4379|Televisão|2|Leticia|Mesquita|1/15/2018|São Paulo|2500|NaN|5000|
|2095|9391|HL1918|iPhone|5|Natalia|Accioly|6/6/2018|São Paulo|5300|NaN|26500|
|2096|9398|HL1918|iPhone|2|Carlos|Araujo|6/19/2018|São Paulo|5300|NaN|10600|
|2097|9403|HL2714|Tablet|5|Daniela|Rosa|3/28/2018|São Paulo|1600|NaN|8000|
|2098|9404|HL1148|Câmera|5|Gabriela|Mello|3/10/2018|São Paulo|2100|NaN|10500|
|2099|9413|HL1918|iPhone|4|Nathalia|Ventura|5/19/2018|São Paulo|5300|NaN|21200|
|2100|9417|HL1148|Câmera|1|Bruna|Londero|5/2/2018|São Paulo|2100|NaN|2100|
|2101|9419|HL8851|Notebook|3|Lucas|Machado|2/2/2018|São Paulo|3500|NaN|10500|
|2102|9424|HL9962|Android|5|Carlos|Souza|1/31/2018|São Paulo|3400|NaN|17000|
|2103|9436|HL1918|iPhone|4|Gabriel|Rocha|10/27/2018|São Paulo|5300|NaN|21200|
|2104|9439|HL7348|SmartWatch|4|Beatriz|Li|6/15/2018|São Paulo|1400|NaN|5600|
|2105|9459|HL4379|Televisão|1|Pedro|Buraco|7/23/2018|São Paulo|2500|NaN|2500|
|2106|9465|HL2714|Tablet|3|Juliana|Goes|6/26/2018|São Paulo|1600|NaN|4800|
|2107|9466|HL1148|Câmera|4|Bruna|Chein|6/18/2018|São Paulo|2100|NaN|8400|
|2108|9467|HL4379|Televisão|2|Matheus|Santos|11/27/2018|São Paulo|2500|NaN|5000|
|2109|9470|HL2714|Tablet|5|Gabrielle|Figueiredo|7/9/2018|São Paulo|1600|NaN|8000|
|2110|9474|HL1918|iPhone|2|Eduardo|Silva|9/28/2018|São Paulo|5300|NaN|10600|
|2111|9476|HL9962|Android|3|Natalia|Accioly|7/12/2018|São Paulo|3400|NaN|10200|
|2112|9478|HL4379|Televisão|5|Breno|Farias|3/11/2018|São Paulo|2500|NaN|12500|
|2113|9483|HL1148|Câmera|3|Felipe|Jorge|11/4/2018|São Paulo|2100|NaN|6300|
|2114|9488|HL1148|Câmera|2|Stephanie|Gonçalves|6/10/2018|São Paulo|2100|NaN|4200|
|2115|9490|HL2714|Tablet|3|Guilherme|Santos|12/22/2018|São Paulo|1600|NaN|4800|
|2116|9491|HL1148|Câmera|5|Eduardo|Pacheco|2/3/2018|São Paulo|2100|NaN|10500|
|2117|9498|HL4379|Televisão|3|Carla|Zakhm|7/20/2018|São Paulo|2500|NaN|7500|
|2118|9499|HL1918|iPhone|2|Aline|Morais|2/27/2018|São Paulo|5300|NaN|10600|
|2119|9500|HL1918|iPhone|2|João|Matheus|6/30/2018|São Paulo|5300|NaN|10600|
|2120|9505|HL4379|Televisão|1|Karina|Camara|9/28/2018|São Paulo|2500|NaN|2500|
|2121|9523|HL8851|Notebook|3|Jônatas|Soares|4/30/2018|São Paulo|3500|NaN|10500|
|2122|9527|HL2714|Tablet|2|Nicolas|Monteiro|12/19/2018|São Paulo|1600|NaN|3200|
|2123|9536|HL1918|iPhone|5|Laura|Araujo|12/6/2018|São Paulo|5300|NaN|26500|
|2124|9540|HL4379|Televisão|2|Thales|Portillo|7/26/2018|São Paulo|2500|NaN|5000|
|2125|9567|HL2714|Tablet|3|Gabriel|Puntel|2/26/2018|São Paulo|1600|NaN|4800|
|2126|9569|HL2714|Tablet|3|Guilherme|Rachide|9/25/2018|São Paulo|1600|NaN|4800|
|2127|9574|HL8851|Notebook|3|Luiz|Marinho|9/4/2018|São Paulo|3500|NaN|10500|
|2128|9577|HL4379|Televisão|4|Julia|Teixeira|3/13/2018|São Paulo|2500|NaN|10000|
|2129|9581|HL9962|Android|4|Caio|Cardoso|10/28/2018|São Paulo|3400|NaN|13600|
|2130|9583|HL2714|Tablet|1|Yasser|Calbucci|9/29/2018|São Paulo|1600|NaN|1600|
|2131|9585|HL8851|Notebook|1|Igor|Azevedo|9/23/2018|São Paulo|3500|NaN|3500|
|2132|9586|HL1918|iPhone|1|Joyce|Souza|8/13/2018|São Paulo|5300|NaN|5300|
|2133|9587|HL1918|iPhone|4|Allan|Guedes|5/23/2018|São Paulo|5300|NaN|21200|
|2134|9592|HL9962|Android|1|Guilherme|Monteiro|1/2/2018|São Paulo|3400|NaN|3400|
|2135|9607|HL1148|Câmera|3|Pedro|Santana|4/6/2018|São Paulo|2100|NaN|6300|
|2136|9608|HL1918|iPhone|5|Milena|Alcoforado|1/9/2018|São Paulo|5300|NaN|26500|
|2137|9609|HL1918|iPhone|1|Rafaela|Feio|11/15/2018|São Paulo|5300|NaN|5300|
|2138|9610|HL1148|Câmera|3|Maria|Cardoso|8/28/2018|São Paulo|2100|NaN|6300|
|2139|9613|HL9962|Android|4|Thais|Rodrigues|6/14/2018|São Paulo|3400|NaN|13600|
|2140|9623|HL1918|iPhone|1|Raíza|Lopes|12/18/2018|São Paulo|5300|NaN|5300|
|2141|9627|HL1918|iPhone|1|Renan|Nascimento|3/20/2018|São Paulo|5300|NaN|5300|
|2142|9628|HL9962|Android|3|Camilla|Cardeman|7/10/2018|São Paulo|3400|NaN|10200|
|2143|9629|HL1918|iPhone|3|Pedro|Ayres|7/17/2018|São Paulo|5300|NaN|15900|
|2144|9640|HL9962|Android|4|Amanda|Felippe|2/14/2018|São Paulo|3400|NaN|13600|
|2145|9641|HL1148|Câmera|5|Bernard|Pedrosa|2/9/2018|São Paulo|2100|NaN|10500|
|2146|9649|HL4379|Televisão|2|Bruna|Gomes|8/13/2018|São Paulo|2500|NaN|5000|
|2147|9653|HL1918|iPhone|3|William|Mendonça|6/29/2018|São Paulo|5300|NaN|15900|
|2148|9654|HL1148|Câmera|1|Juliana|Silva|8/26/2018|São Paulo|2100|NaN|2100|
|2149|9660|HL7348|SmartWatch|2|Isabela|Chagas|4/9/2018|São Paulo|1400|NaN|2800|
|2150|9663|HL7348|SmartWatch|5|Barbara|Procaci|11/14/2018|São Paulo|1400|NaN|7000|
|2151|9664|HL9962|Android|1|Arthur|Fernandes|7/19/2018|São Paulo|3400|NaN|3400|
|2152|9674|HL8851|Notebook|5|Henrique|Villanova|11/5/2018|São Paulo|3500|NaN|17500|
|2153|9685|HL1148|Câmera|3|Thales|Portillo|3/18/2018|São Paulo|2100|NaN|6300|
|2154|9687|HL1918|iPhone|2|Gabriel|Rubim|2/21/2018|São Paulo|5300|NaN|10600|
|2155|9700|HL4379|Televisão|2|Nina|Magalhães|3/10/2018|São Paulo|2500|NaN|5000|
|2156|9707|HL1148|Câmera|2|Beatriz|Biase|8/3/2018|São Paulo|2100|NaN|4200|
|2157|9712|HL1148|Câmera|4|Sandy|Figueiredo|8/7/2018|São Paulo|2100|NaN|8400|
|2158|9713|HL2714|Tablet|1|Bianca|Tatsch|7/15/2018|São Paulo|1600|NaN|1600|
|2159|9719|HL9962|Android|3|Melissa|Nucci|11/7/2018|São Paulo|3400|NaN|10200|
|2160|9722|HL2714|Tablet|3|Matheus|Santos|3/5/2018|São Paulo|1600|NaN|4800|
|2161|9724|HL2714|Tablet|2|Carlos|Silva|9/16/2018|São Paulo|1600|NaN|3200|
|2162|9725|HL1148|Câmera|2|Bruna|Londero|5/6/2018|São Paulo|2100|NaN|4200|
|2163|9742|HL1918|iPhone|1|Breno|Varella|7/9/2018|São Paulo|5300|NaN|5300|
|2164|9744|HL8851|Notebook|3|Maria|Motta|4/12/2018|São Paulo|3500|NaN|10500|
|2165|9747|HL1918|iPhone|5|Carlos|Melo|6/29/2018|São Paulo|5300|NaN|26500|
|2166|9750|HL7348|SmartWatch|4|Rodrigo|Silva|4/10/2018|São Paulo|1400|NaN|5600|
|2167|9753|HL1918|iPhone|2|Chan|Santos|11/28/2018|São Paulo|5300|NaN|10600|
|2168|9756|HL1148|Câmera|5|Carolina|Bernardes|4/17/2018|São Paulo|2100|NaN|10500|
|2169|9766|HL4379|Televisão|2|Lucas|Machado|5/8/2018|São Paulo|2500|NaN|5000|
|2170|9767|HL9962|Android|5|Diego|Mello|5/4/2018|São Paulo|3400|NaN|17000|
|2171|9777|HL4379|Televisão|4|Lucas|Assunção|6/4/2018|São Paulo|2500|NaN|10000|
|2172|9778|HL1918|iPhone|3|Hércules|Moreira|12/12/2018|São Paulo|5300|NaN|15900|
|2173|9782|HL1148|Câmera|2|Ruan|Lopes|1/24/2018|São Paulo|2100|NaN|4200|
|2174|9783|HL4379|Televisão|5|Deysiane|Medronho|7/13/2018|São Paulo|2500|NaN|12500|
|2175|9786|HL8851|Notebook|2|Eric|Júnior|6/3/2018|São Paulo|3500|NaN|7000|
|2176|9790|HL9962|Android|3|Jônatas|Castro|5/1/2018|São Paulo|3400|NaN|10200|
|2177|9801|HL1918|iPhone|5|Gabriela|Cavalcanti|10/9/2018|São Paulo|5300|NaN|26500|
|2178|9810|HL1918|iPhone|5|Renan|Ventura|9/5/2018|São Paulo|5300|NaN|26500|
|2179|9814|HL2714|Tablet|2|Milena|Alcoforado|3/25/2018|São Paulo|1600|NaN|3200|
|2180|9817|HL1918|iPhone|4|Marcelo|Pereira|3/21/2018|São Paulo|5300|NaN|21200|
|2181|9820|HL4379|Televisão|1|Lucas|Lemos|7/5/2018|São Paulo|2500|NaN|2500|
|2182|9827|HL4379|Televisão|4|Roberta|Nogueira|1/10/2018|São Paulo|2500|NaN|10000|
|2183|9831|HL1918|iPhone|3|Rodrigo|Feijo|3/4/2018|São Paulo|5300|NaN|15900|
|2184|9838|HL7348|SmartWatch|1|Caio|Silva|1/6/2018|São Paulo|1400|NaN|1400|
|2185|9839|HL4379|Televisão|3|Aline|Andrade|1/11/2018|São Paulo|2500|NaN|7500|
|2186|9841|HL8851|Notebook|3|Lucas|Fontoura|11/19/2018|São Paulo|3500|NaN|10500|
|2187|9846|HL8851|Notebook|5|Bruno|Oliveira|11/1/2018|São Paulo|3500|NaN|17500|
|2188|9847|HL4379|Televisão|2|Luiz|Xavier|2/9/2018|São Paulo|2500|NaN|5000|
|2189|9852|HL4379|Televisão|2|Ana|Campos|9/4/2018|São Paulo|2500|NaN|5000|
|2190|9855|HL2714|Tablet|1|Andressa|Rotsztejn|12/23/2018|São Paulo|1600|NaN|1600|
|2191|9856|HL4379|Televisão|2|Bruno|Velucci|7/3/2018|São Paulo|2500|NaN|5000|
|2192|9861|HL2714|Tablet|5|Ananda|Dias|5/10/2018|São Paulo|1600|NaN|8000|
|2193|9868|HL1918|iPhone|5|Nathan|Morelli|8/2/2018|São Paulo|5300|NaN|26500|
|2194|9869|HL2714|Tablet|3|Rodrigo|Mendes|5/26/2018|São Paulo|1600|NaN|4800|
|2195|9871|HL9962|Android|2|José|Fonseca|3/9/2018|São Paulo|3400|NaN|6800|
|2196|9872|HL4379|Televisão|1|Daniela|Rosa|10/2/2018|São Paulo|2500|NaN|2500|
|2197|9873|HL8851|Notebook|5|Pedro|Jorge|10/29/2018|São Paulo|3500|NaN|17500|
|2198|9881|HL1918|iPhone|1|Mariana|Freire|4/16/2018|São Paulo|5300|NaN|5300|
|2199|9884|HL2714|Tablet|3|Julia|Penteado|9/8/2018|São Paulo|1600|NaN|4800|
|2200|9887|HL1918|iPhone|1|Ravena|Bhering|4/1/2018|São Paulo|5300|NaN|5300|
|2201|9894|HL7348|SmartWatch|5|Rodrigo|Ramos|12/3/2018|São Paulo|1400|NaN|7000|
|2202|9896|HL7348|SmartWatch|1|Yasser|Calbucci|4/19/2018|São Paulo|1400|NaN|1400|
|2203|9900|HL1148|Câmera|3|Lucas|Monte|6/4/2018|São Paulo|2100|NaN|6300|
|2204|9905|HL4379|Televisão|5|Felipe|Mello|3/4/2018|São Paulo|2500|NaN|12500|
|2205|9909|HL9962|Android|1|Gabriel|Thoni|4/7/2018|São Paulo|3400|NaN|3400|
|2206|9915|HL4379|Televisão|1|Kimberly|Sad|1/26/2018|São Paulo|2500|NaN|2500|
|2207|9917|HL1918|iPhone|5|Thais|Rodrigues|6/19/2018|São Paulo|5300|NaN|26500|
|2208|9922|HL2714|Tablet|2|Luiz|Almeida|2/1/2018|São Paulo|1600|NaN|3200|
|2209|9928|HL7348|SmartWatch|5|Fernanda|Coutinho|11/17/2018|São Paulo|1400|NaN|7000|
|2210|9929|HL8851|Notebook|3|Anderson|Martins|12/25/2018|São Paulo|3500|NaN|10500|
|2211|9931|HL1918|iPhone|3|Eduardo|Pacheco|7/31/2018|São Paulo|5300|NaN|15900|
|2212|9940|HL4379|Televisão|3|Lucas|Wanderley|6/3/2018|São Paulo|2500|NaN|7500|
|2213|9949|HL1918|iPhone|2|Beatriz|Rodrigues|8/19/2018|São Paulo|5300|NaN|10600|
|2214|9953|HL1918|iPhone|4|Rubens|Valente|11/28/2018|São Paulo|5300|NaN|21200|
|2215|9957|HL4379|Televisão|2|Beatriz|Nogueira|9/23/2018|São Paulo|2500|NaN|5000|
|2216|9958|HL1918|iPhone|4|Mariane|Ferreira|6/10/2018|São Paulo|5300|NaN|21200|
|2217|9963|HL1918|iPhone|3|Bianca|Allevato|5/18/2018|São Paulo|5300|NaN|15900|
|2218|9967|HL2714|Tablet|3|Roberta|Pimenta|9/11/2018|São Paulo|1600|NaN|4800|
|2219|9973|HL1148|Câmera|2|Bruno|Oliveira|4/14/2018|São Paulo|2100|NaN|4200|
|2220|9977|HL4379|Televisão|5|Rafael|Rocha|9/27/2018|São Paulo|2500|NaN|12500|
|2221|9981|HL7348|SmartWatch|4|João|Junior|4/14/2018|São Paulo|1400|NaN|5600|
|2222|9984|HL1918|iPhone|4|Itai|Puntel|5/2/2018|São Paulo|5300|NaN|21200|
|2223|9985|HL1918|iPhone|1|Guilherme|Vianna|3/18/2018|São Paulo|5300|NaN|5300|
|2224|9991|HL7348|SmartWatch|5|Antônio|Soares|11/21/2018|São Paulo|1400|NaN|7000|
|2225|9996|HL4379|Televisão|5|Caio|Moraes|1/22/2018|São Paulo|2500|NaN|12500|
|0|17|HL4379|Televisão|2|Carolina|Alfradique|2/25/2018|Belo Horizonte|2500|NaN|5000|
|1|25|HL4379|Televisão|1|Danilo|Rubim|2/20/2018|Belo Horizonte|2500|NaN|2500|
|2|27|HL1918|iPhone|5|Bernard|Pedrosa|7/7/2018|Belo Horizonte|5300|NaN|26500|
|3|54|HL1918|iPhone|5|Lucas|Lemos|12/26/2018|Belo Horizonte|5300|NaN|26500|
|4|67|HL8851|Notebook|5|Bernardo|Botelho|6/8/2018|Belo Horizonte|3500|NaN|17500|
|5|107|HL4379|Televisão|2|Raíza|Lopes|4/24/2018|Belo Horizonte|2500|NaN|5000|
|6|117|HL8851|Notebook|1|Paola|Abreu|8/2/2018|Belo Horizonte|3500|NaN|3500|
|7|155|HL8851|Notebook|4|Marina|Delgado|5/10/2018|Belo Horizonte|3500|NaN|14000|
|8|189|HL8851|Notebook|5|Giovana|Vilela|7/10/2018|Belo Horizonte|3500|NaN|17500|
|9|217|HL1918|iPhone|5|Gabriel|Brito|7/15/2018|Belo Horizonte|5300|NaN|26500|
|10|218|HL7348|SmartWatch|1|Amanda|Delgado|10/22/2018|Belo Horizonte|1400|NaN|1400|
|11|220|HL1918|iPhone|5|Isabella|Scalabrin|6/13/2018|Belo Horizonte|5300|NaN|26500|
|12|231|HL1918|iPhone|5|Guilherme|Monteiro|7/7/2018|Belo Horizonte|5300|NaN|26500|
|13|262|HL4379|Televisão|3|Isabel|Lacerda|1/10/2018|Belo Horizonte|2500|NaN|7500|
|14|316|HL2714|Tablet|4|Aline|Morais|1/23/2018|Belo Horizonte|1600|NaN|6400|
|15|319|HL2714|Tablet|2|Isabela|Rodrigues|7/24/2018|Belo Horizonte|1600|NaN|3200|
|16|329|HL4379|Televisão|3|Aline|Andrade|10/7/2018|Belo Horizonte|2500|NaN|7500|
|17|388|HL1918|iPhone|2|Raul|Junqueira|9/24/2018|Belo Horizonte|5300|NaN|10600|
|18|397|HL2714|Tablet|1|Lucas|Lemos|11/15/2018|Belo Horizonte|1600|NaN|1600|
|19|420|HL2714|Tablet|3|Leandro|Melo|2/28/2018|Belo Horizonte|1600|NaN|4800|
|20|428|HL1148|Câmera|2|Rogério|Gentile|10/13/2018|Belo Horizonte|2100|NaN|4200|
|21|430|HL7348|SmartWatch|3|Julia|Aliani|11/28/2018|Belo Horizonte|1400|NaN|4200|
|22|434|HL1148|Câmera|4|Victor|Gomes|5/8/2018|Belo Horizonte|2100|NaN|8400|
|23|452|HL2714|Tablet|5|Luã|Sá|4/16/2018|Belo Horizonte|1600|NaN|8000|
|24|492|HL1148|Câmera|3|Pedro|Santos|12/24/2018|Belo Horizonte|2100|NaN|6300|
|25|520|HL9962|Android|2|Thiago|Nóbrega|11/11/2018|Belo Horizonte|3400|NaN|6800|
|26|530|HL4379|Televisão|4|Rafael|Portela|2/27/2018|Belo Horizonte|2500|NaN|10000|
|27|540|HL9962|Android|4|Ana|Silva|10/13/2018|Belo Horizonte|3400|NaN|13600|
|28|566|HL8851|Notebook|4|João|Costa|9/18/2018|Belo Horizonte|3500|NaN|14000|
|29|604|HL1918|iPhone|4|Thomáz|Vannier|3/5/2018|Belo Horizonte|5300|NaN|21200|
|30|609|HL9962|Android|2|Paula|Carneiro|5/26/2018|Belo Horizonte|3400|NaN|6800|
|31|610|HL1918|iPhone|5|Ana|Carvalho|6/19/2018|Belo Horizonte|5300|NaN|26500|
|32|660|HL1918|iPhone|4|Felipe|Jorge|8/2/2018|Belo Horizonte|5300|NaN|21200|
|33|690|HL4379|Televisão|2|Daniel|Ortiz|8/24/2018|Belo Horizonte|2500|NaN|5000|
|34|691|HL9962|Android|5|Mônica|Rotolo|2/2/2018|Belo Horizonte|3400|NaN|17000|
|35|701|HL1918|iPhone|5|Raphael|Rezende|2/9/2018|Belo Horizonte|5300|NaN|26500|
|36|719|HL7348|SmartWatch|3|Anderson|Cavalcanti|6/14/2018|Belo Horizonte|1400|NaN|4200|
|37|729|HL1918|iPhone|2|Gustavo|Erthal|8/9/2018|Belo Horizonte|5300|NaN|10600|
|38|730|HL9962|Android|4|Ana|Fioretti|10/23/2018|Belo Horizonte|3400|NaN|13600|
|39|738|HL2714|Tablet|3|Amanda|Procaci|3/12/2018|Belo Horizonte|1600|NaN|4800|
|40|752|HL1918|iPhone|3|Carolina|Costa|9/17/2018|Belo Horizonte|5300|NaN|15900|
|41|761|HL4379|Televisão|4|Carolina|Siqueira|8/1/2018|Belo Horizonte|2500|NaN|10000|
|42|763|HL1918|iPhone|2|Igor|Azevedo|6/8/2018|Belo Horizonte|5300|NaN|10600|
|43|782|HL1918|iPhone|4|Karine|Barros|3/22/2018|Belo Horizonte|5300|NaN|21200|
|44|802|HL4379|Televisão|1|Pedro|Costa|3/27/2018|Belo Horizonte|2500|NaN|2500|
|45|807|HL8851|Notebook|4|Arthur|Rocha|11/25/2018|Belo Horizonte|3500|NaN|14000|
|46|817|HL7348|SmartWatch|2|Natalia|Accioly|8/7/2018|Belo Horizonte|1400|NaN|2800|
|47|825|HL4379|Televisão|5|Raíssa|Oros|2/17/2018|Belo Horizonte|2500|NaN|12500|
|48|840|HL4379|Televisão|1|Katharina|Barros|2/16/2018|Belo Horizonte|2500|NaN|2500|
|49|845|HL4379|Televisão|1|Lara|Moreira|10/25/2018|Belo Horizonte|2500|NaN|2500|
|50|850|HL1148|Câmera|2|Carlos|Mesquita|1/11/2018|Belo Horizonte|2100|NaN|4200|
|51|855|HL1918|iPhone|1|Carolina|Bernardes|3/25/2018|Belo Horizonte|5300|NaN|5300|
|52|856|HL1918|iPhone|3|Marcela|Gasperi|12/31/2018|Belo Horizonte|5300|NaN|15900|
|53|872|HL8851|Notebook|1|Gustavo|Junior|4/12/2018|Belo Horizonte|3500|NaN|3500|
|54|891|HL1918|iPhone|4|Matheus|Silva|7/3/2018|Belo Horizonte|5300|NaN|21200|
|55|927|HL1148|Câmera|1|Danilo|Mendonça|4/19/2018|Belo Horizonte|2100|NaN|2100|
|56|938|HL1918|iPhone|4|Wen|Braga|5/1/2018|Belo Horizonte|5300|NaN|21200|
|57|946|HL1918|iPhone|3|Gabriel|Brito|4/28/2018|Belo Horizonte|5300|NaN|15900|
|58|953|HL7348|SmartWatch|4|Jonatas|Passos|8/14/2018|Belo Horizonte|1400|NaN|5600|
|59|955|HL1918|iPhone|1|Gabriel|Rocha|6/11/2018|Belo Horizonte|5300|NaN|5300|
|60|968|HL9962|Android|4|Beatriz|Rocha|1/11/2018|Belo Horizonte|3400|NaN|13600|
|61|977|HL4379|Televisão|1|Adrielle|Gabriel|4/8/2018|Belo Horizonte|2500|NaN|2500|
|62|983|HL8851|Notebook|1|Caroll|Johnson|12/11/2018|Belo Horizonte|3500|NaN|3500|
|63|1041|HL4379|Televisão|4|Bruna|Franco|10/26/2018|Belo Horizonte|2500|NaN|10000|
|64|1046|HL2714|Tablet|4|Maria|Motta|5/8/2018|Belo Horizonte|1600|NaN|6400|
|65|1060|HL1918|iPhone|3|Priscila|Garcia|10/24/2018|Belo Horizonte|5300|NaN|15900|
|66|1079|HL1918|iPhone|5|Andressa|Nóbrega|9/18/2018|Belo Horizonte|5300|NaN|26500|
|67|1114|HL4379|Televisão|2|Ana|Miura|7/24/2018|Belo Horizonte|2500|NaN|5000|
|68|1128|HL8851|Notebook|2|Giulia|Pessanha|11/13/2018|Belo Horizonte|3500|NaN|7000|
|69|1129|HL7348|SmartWatch|3|Samara|Pinto|1/10/2018|Belo Horizonte|1400|NaN|4200|
|70|1143|HL4379|Televisão|4|Caio|Silva|11/21/2018|Belo Horizonte|2500|NaN|10000|
|71|1147|HL7348|SmartWatch|1|Myllena|Carneiro|1/22/2018|Belo Horizonte|1400|NaN|1400|
|72|1154|HL9962|Android|3|Juan|Fernandes|1/9/2018|Belo Horizonte|3400|NaN|10200|
|73|1161|HL1148|Câmera|4|Raphael|Mattos|6/22/2018|Belo Horizonte|2100|NaN|8400|
|74|1179|HL9962|Android|3|Gustavo|Junior|2/23/2018|Belo Horizonte|3400|NaN|10200|
|75|1203|HL1148|Câmera|2|Célio|Xavier|6/6/2018|Belo Horizonte|2100|NaN|4200|
|76|1233|HL2714|Tablet|4|Diego|Rodrigues|10/13/2018|Belo Horizonte|1600|NaN|6400|
|77|1235|HL1148|Câmera|5|Guilherme|Monteiro|5/18/2018|Belo Horizonte|2100|NaN|10500|
|78|1267|HL1148|Câmera|1|Anderson|Martins|4/22/2018|Belo Horizonte|2100|NaN|2100|
|79|1283|HL9962|Android|1|Júlia|Almeida|12/6/2018|Belo Horizonte|3400|NaN|3400|
|80|1314|HL2714|Tablet|2|Carolina|Motta|8/6/2018|Belo Horizonte|1600|NaN|3200|
|81|1339|HL9962|Android|5|Bernardo|Nauenberg|2/21/2018|Belo Horizonte|3400|NaN|17000|
|82|1350|HL4379|Televisão|4|Giuseppe|Bhering|5/13/2018|Belo Horizonte|2500|NaN|10000|
|83|1394|HL2714|Tablet|3|Chan|Santos|6/20/2018|Belo Horizonte|1600|NaN|4800|
|84|1486|HL1918|iPhone|2|Rafaela|Ferreira|9/14/2018|Belo Horizonte|5300|NaN|10600|
|85|1497|HL8851|Notebook|5|Erick|Soares|12/8/2018|Belo Horizonte|3500|NaN|17500|
|86|1503|HL8851|Notebook|5|Jéssica|Resinente|5/8/2018|Belo Horizonte|3500|NaN|17500|
|87|1507|HL9962|Android|2|Hanna|Fonseca|11/16/2018|Belo Horizonte|3400|NaN|6800|
|88|1520|HL8851|Notebook|3|Carolina|Carneiro|3/19/2018|Belo Horizonte|3500|NaN|10500|
|89|1529|HL1918|iPhone|2|Mariane|Racy|6/8/2018|Belo Horizonte|5300|NaN|10600|
|90|1536|HL2714|Tablet|3|Deysiane|Bach|5/15/2018|Belo Horizonte|1600|NaN|4800|
|91|1542|HL1148|Câmera|5|Thales|Portillo|1/29/2018|Belo Horizonte|2100|NaN|10500|
|92|1547|HL7348|SmartWatch|5|Rafael|Ramos|1/30/2018|Belo Horizonte|1400|NaN|7000|
|93|1562|HL4379|Televisão|3|Gabriella|Sagrillo|1/13/2018|Belo Horizonte|2500|NaN|7500|
|94|1563|HL1148|Câmera|1|João|Tabet|11/2/2018|Belo Horizonte|2100|NaN|2100|
|95|1590|HL1148|Câmera|5|Juliana|Huon|10/18/2018|Belo Horizonte|2100|NaN|10500|
|96|1614|HL7348|SmartWatch|5|Mariana|Barrozo|6/15/2018|Belo Horizonte|1400|NaN|7000|
|97|1620|HL1148|Câmera|2|Gabriel|Pereira|1/30/2018|Belo Horizonte|2100|NaN|4200|
|98|1662|HL1148|Câmera|2|Carlos|Souza|5/26/2018|Belo Horizonte|2100|NaN|4200|
|99|1697|HL4379|Televisão|2|Thomáz|Bôas|6/30/2018|Belo Horizonte|2500|NaN|5000|
|100|1708|HL1918|iPhone|4|Pedro|Rodrigues|2/17/2018|Belo Horizonte|5300|NaN|21200|
|101|1726|HL9962|Android|2|Rafael|Carneiro|10/6/2018|Belo Horizonte|3400|NaN|6800|
|102|1728|HL2714|Tablet|2|Marina|Delgado|8/11/2018|Belo Horizonte|1600|NaN|3200|
|103|1761|HL4379|Televisão|2|Rachel|Restum|9/3/2018|Belo Horizonte|2500|NaN|5000|
|104|1762|HL1918|iPhone|3|Luiza|Cabral|2/18/2018|Belo Horizonte|5300|NaN|15900|
|105|1785|HL4379|Televisão|5|Caio|Fernandes|8/13/2018|Belo Horizonte|2500|NaN|12500|
|106|1793|HL9962|Android|2|Mariana|Barrozo|4/17/2018|Belo Horizonte|3400|NaN|6800|
|107|1799|HL1918|iPhone|1|Gabriel|Almeida|6/26/2018|Belo Horizonte|5300|NaN|5300|
|108|1806|HL7348|SmartWatch|2|Marcelo|Borges|9/10/2018|Belo Horizonte|1400|NaN|2800|
|109|1807|HL1918|iPhone|3|Maria|Costa|8/15/2018|Belo Horizonte|5300|NaN|15900|
|110|1838|HL9962|Android|1|Marcos|Nucci|7/17/2018|Belo Horizonte|3400|NaN|3400|
|111|1874|HL4379|Televisão|4|Juliana|Guimarães|10/6/2018|Belo Horizonte|2500|NaN|10000|
|112|1880|HL1918|iPhone|4|Jessica|Ferreira|7/13/2018|Belo Horizonte|5300|NaN|21200|
|113|1883|HL1918|iPhone|1|Iuri|Neto|7/4/2018|Belo Horizonte|5300|NaN|5300|
|114|1886|HL8851|Notebook|1|Breno|Britto|9/14/2018|Belo Horizonte|3500|NaN|3500|
|115|1912|HL1148|Câmera|1|Maria|Motta|9/20/2018|Belo Horizonte|2100|NaN|2100|
|116|1923|HL1148|Câmera|1|Larissa|Jesus|6/13/2018|Belo Horizonte|2100|NaN|2100|
|117|1924|HL2714|Tablet|2|Gabriel|Azevedo|5/28/2018|Belo Horizonte|1600|NaN|3200|
|118|1935|HL1148|Câmera|3|Pedro|Cardoso|11/23/2018|Belo Horizonte|2100|NaN|6300|
|119|1938|HL7348|SmartWatch|2|Raul|Silveira|1/6/2018|Belo Horizonte|1400|NaN|2800|
|120|1948|HL1148|Câmera|5|Eduardo|Silva|12/10/2018|Belo Horizonte|2100|NaN|10500|
|121|1967|HL1918|iPhone|2|Henrique|Oliveira|5/21/2018|Belo Horizonte|5300|NaN|10600|
|122|2026|HL1918|iPhone|1|João|Tabet|6/30/2018|Belo Horizonte|5300|NaN|5300|
|123|2051|HL1918|iPhone|1|Luana|Santos|10/24/2018|Belo Horizonte|5300|NaN|5300|
|124|2090|HL9962|Android|2|Michelle|Miura|5/2/2018|Belo Horizonte|3400|NaN|6800|
|125|2095|HL9962|Android|4|Manuela|Ferreira|4/13/2018|Belo Horizonte|3400|NaN|13600|
|126|2098|HL4379|Televisão|2|Roger|Rosa|10/12/2018|Belo Horizonte|2500|NaN|5000|
|127|2125|HL1918|iPhone|4|Caroline|Cavalcanti|5/14/2018|Belo Horizonte|5300|NaN|21200|
|128|2143|HL7348|SmartWatch|5|Mariane|Ferreira|8/22/2018|Belo Horizonte|1400|NaN|7000|
|129|2146|HL4379|Televisão|5|Thales|Fanara|9/18/2018|Belo Horizonte|2500|NaN|12500|
|130|2152|HL9962|Android|3|Jessica|Ferreira|11/12/2018|Belo Horizonte|3400|NaN|10200|
|131|2160|HL7348|SmartWatch|2|Allan|Candido|5/20/2018|Belo Horizonte|1400|NaN|2800|
|132|2200|HL9962|Android|5|Rodrigo|Bruno|12/4/2018|Belo Horizonte|3400|NaN|17000|
|133|2203|HL4379|Televisão|4|Maria|Junior|1/21/2018|Belo Horizonte|2500|NaN|10000|
|134|2208|HL1918|iPhone|1|Pedro|Dalforne|8/7/2018|Belo Horizonte|5300|NaN|5300|
|135|2223|HL1918|iPhone|1|Gabriel|Rocha|5/29/2018|Belo Horizonte|5300|NaN|5300|
|136|2247|HL8851|Notebook|1|Cícero|Lima|4/13/2018|Belo Horizonte|3500|NaN|3500|
|137|2264|HL1148|Câmera|2|Victoria|Tavares|9/27/2018|Belo Horizonte|2100|NaN|4200|
|138|2268|HL4379|Televisão|1|Matheus|Moraes|2/7/2018|Belo Horizonte|2500|NaN|2500|
|139|2310|HL9962|Android|2|Eric|Neves|3/9/2018|Belo Horizonte|3400|NaN|6800|
|140|2333|HL4379|Televisão|5|João|Araujo|3/17/2018|Belo Horizonte|2500|NaN|12500|
|141|2339|HL1918|iPhone|1|Debora|Silva|12/9/2018|Belo Horizonte|5300|NaN|5300|
|142|2367|HL7348|SmartWatch|4|Lucas|Wanderley|12/12/2018|Belo Horizonte|1400|NaN|5600|
|143|2368|HL9962|Android|2|Raul|Junqueira|11/10/2018|Belo Horizonte|3400|NaN|6800|
|144|2372|HL4379|Televisão|3|Victoria|Mazza|12/27/2018|Belo Horizonte|2500|NaN|7500|
|145|2379|HL8851|Notebook|4|Livia|Cozendey|7/8/2018|Belo Horizonte|3500|NaN|14000|
|146|2393|HL1918|iPhone|5|Larissa|Vasconcellos|12/22/2018|Belo Horizonte|5300|NaN|26500|
|147|2398|HL4379|Televisão|1|Caio|Moraes|6/27/2018|Belo Horizonte|2500|NaN|2500|
|148|2413|HL8851|Notebook|5|Bárbara|Lima|8/2/2018|Belo Horizonte|3500|NaN|17500|
|149|2424|HL1918|iPhone|5|Caio|Vianna|9/7/2018|Belo Horizonte|5300|NaN|26500|
|150|2431|HL7348|SmartWatch|1|Daniel|Monteiro|5/23/2018|Belo Horizonte|1400|NaN|1400|
|151|2436|HL9962|Android|1|José|Vieira|10/30/2018|Belo Horizonte|3400|NaN|3400|
|152|2449|HL2714|Tablet|2|Caroline|Delgado|10/5/2018|Belo Horizonte|1600|NaN|3200|
|153|2476|HL4379|Televisão|1|Bernardo|Ribeiro|12/3/2018|Belo Horizonte|2500|NaN|2500|
|154|2478|HL1918|iPhone|1|Guilherme|Rachide|4/25/2018|Belo Horizonte|5300|NaN|5300|
|155|2526|HL9962|Android|1|Vitor|Arruda|10/22/2018|Belo Horizonte|3400|NaN|3400|
|156|2555|HL1918|iPhone|4|Daniela|Rosa|4/5/2018|Belo Horizonte|5300|NaN|21200|
|157|2635|HL9962|Android|2|Gustavo|Accardo|8/15/2018|Belo Horizonte|3400|NaN|6800|
|158|2669|HL7348|SmartWatch|4|Breno|Caputo|6/13/2018|Belo Horizonte|1400|NaN|5600|
|159|2687|HL7348|SmartWatch|1|Norman|Jimbo|4/7/2018|Belo Horizonte|1400|NaN|1400|
|160|2694|HL8851|Notebook|3|Yasmim|Bittencourt|10/21/2018|Belo Horizonte|3500|NaN|10500|
|161|2745|HL8851|Notebook|5|Andreza|Ramos|6/15/2018|Belo Horizonte|3500|NaN|17500|
|162|2749|HL7348|SmartWatch|3|Luiza|Cabral|7/30/2018|Belo Horizonte|1400|NaN|4200|
|163|2768|HL1918|iPhone|5|Marina|Miranda|8/10/2018|Belo Horizonte|5300|NaN|26500|
|164|2774|HL9962|Android|5|Douglas|Rodrigues|8/17/2018|Belo Horizonte|3400|NaN|17000|
|165|2778|HL1918|iPhone|5|Pedro|Oliveira|11/28/2018|Belo Horizonte|5300|NaN|26500|
|166|2799|HL2714|Tablet|2|Caio|Ferreira|6/30/2018|Belo Horizonte|1600|NaN|3200|
|167|2820|HL8851|Notebook|4|Raul|Silveira|1/27/2018|Belo Horizonte|3500|NaN|14000|
|168|2821|HL2714|Tablet|4|Luiza|Ribeiro|2/12/2018|Belo Horizonte|1600|NaN|6400|
|169|2829|HL1918|iPhone|4|Jônatas|Castro|2/2/2018|Belo Horizonte|5300|NaN|21200|
|170|2843|HL8851|Notebook|1|Camila|Sobral|8/6/2018|Belo Horizonte|3500|NaN|3500|
|171|2853|HL4379|Televisão|2|Isabela|Chagas|7/28/2018|Belo Horizonte|2500|NaN|5000|
|172|2873|HL1918|iPhone|1|Arthur|Pereira|7/22/2018|Belo Horizonte|5300|NaN|5300|
|173|2875|HL9962|Android|3|Jéssica|Stefanelli|2/3/2018|Belo Horizonte|3400|NaN|10200|
|174|2890|HL2714|Tablet|2|Carolina|Bernardes|7/15/2018|Belo Horizonte|1600|NaN|3200|
|175|2904|HL4379|Televisão|1|Mateus|Duque|9/9/2018|Belo Horizonte|2500|NaN|2500|
|176|2937|HL4379|Televisão|4|Marcelo|Magalhães|12/2/2018|Belo Horizonte|2500|NaN|10000|
|177|2956|HL1148|Câmera|1|Vitor|Arruda|12/16/2018|Belo Horizonte|2100|NaN|2100|
|178|2963|HL1918|iPhone|4|Henrique|Oliveira|6/28/2018|Belo Horizonte|5300|NaN|21200|
|179|2987|HL4379|Televisão|2|Eduardo|Ferreira|11/10/2018|Belo Horizonte|2500|NaN|5000|
|180|2996|HL1918|iPhone|3|Luã|Sá|2/18/2018|Belo Horizonte|5300|NaN|15900|
|181|3018|HL1918|iPhone|5|Raphael|Coelho|8/11/2018|Belo Horizonte|5300|NaN|26500|
|182|3025|HL2714|Tablet|2|Raíssa|Nimer|3/11/2018|Belo Horizonte|1600|NaN|3200|
|183|3040|HL1918|iPhone|2|Philipe|Morete|1/30/2018|Belo Horizonte|5300|NaN|10600|
|184|3041|HL2714|Tablet|1|Thaís|Pereira|9/9/2018|Belo Horizonte|1600|NaN|1600|
|185|3075|HL1918|iPhone|4|Anna|Maia|4/5/2018|Belo Horizonte|5300|NaN|21200|
|186|3098|HL9962|Android|3|Juliana|Guimarães|4/3/2018|Belo Horizonte|3400|NaN|10200|
|187|3132|HL7348|SmartWatch|5|Roberta|Teixeira|10/14/2018|Belo Horizonte|1400|NaN|7000|
|188|3163|HL8851|Notebook|5|Gabrielle|Costa|8/9/2018|Belo Horizonte|3500|NaN|17500|
|189|3180|HL1918|iPhone|4|Fabio|Sepúlveda|3/25/2018|Belo Horizonte|5300|NaN|21200|
|190|3218|HL2714|Tablet|2|Arthur|Fernandes|4/6/2018|Belo Horizonte|1600|NaN|3200|
|191|3219|HL4379|Televisão|2|Livia|Codeceira|4/18/2018|Belo Horizonte|2500|NaN|5000|
|192|3226|HL4379|Televisão|3|Isabella|Santos|9/4/2018|Belo Horizonte|2500|NaN|7500|
|193|3236|HL4379|Televisão|1|Gabriel|Ribeiro|7/29/2018|Belo Horizonte|2500|NaN|2500|
|194|3281|HL8851|Notebook|1|Gustavo|Aragão|10/22/2018|Belo Horizonte|3500|NaN|3500|
|195|3317|HL1918|iPhone|3|Carolina|Silva|11/24/2018|Belo Horizonte|5300|NaN|15900|
|196|3324|HL4379|Televisão|3|Livia|Corrêa|4/11/2018|Belo Horizonte|2500|NaN|7500|
|197|3331|HL2714|Tablet|2|Rebeca|Manhães|9/13/2018|Belo Horizonte|1600|NaN|3200|
|198|3362|HL7348|SmartWatch|3|Patrícia|Fernandes|2/22/2018|Belo Horizonte|1400|NaN|4200|
|199|3370|HL1918|iPhone|4|Giuseppe|Bhering|9/6/2018|Belo Horizonte|5300|NaN|21200|
|200|3399|HL1918|iPhone|4|Paulo|Campos|4/21/2018|Belo Horizonte|5300|NaN|21200|
|201|3418|HL1918|iPhone|3|Lucas|Junior|6/12/2018|Belo Horizonte|5300|NaN|15900|
|202|3426|HL2714|Tablet|4|Gustavo|Thome|8/8/2018|Belo Horizonte|1600|NaN|6400|
|203|3435|HL4379|Televisão|5|Deysiane|Bach|9/28/2018|Belo Horizonte|2500|NaN|12500|
|204|3437|HL9962|Android|2|Bruna|Londero|1/6/2018|Belo Horizonte|3400|NaN|6800|
|205|3442|HL4379|Televisão|2|Juliana|Guimarães|5/31/2018|Belo Horizonte|2500|NaN|5000|
|206|3487|HL1918|iPhone|4|Mateus|Maia|3/30/2018|Belo Horizonte|5300|NaN|21200|
|207|3489|HL9962|Android|2|Adrielle|Vieira|10/1/2018|Belo Horizonte|3400|NaN|6800|
|208|3497|HL1918|iPhone|4|Fernanda|Junior|4/24/2018|Belo Horizonte|5300|NaN|21200|
|209|3563|HL1918|iPhone|1|José|Seixas|10/18/2018|Belo Horizonte|5300|NaN|5300|
|210|3577|HL1918|iPhone|4|Rafael|Wajnsztok|9/6/2018|Belo Horizonte|5300|NaN|21200|
|211|3603|HL4379|Televisão|5|Cícero|Ramos|6/24/2018|Belo Horizonte|2500|NaN|12500|
|212|3609|HL1918|iPhone|5|Luiz|Campista|2/11/2018|Belo Horizonte|5300|NaN|26500|
|213|3621|HL4379|Televisão|4|Carolina|Rocha|6/5/2018|Belo Horizonte|2500|NaN|10000|
|214|3622|HL1918|iPhone|4|Natalia|Accioly|2/20/2018|Belo Horizonte|5300|NaN|21200|
|215|3623|HL7348|SmartWatch|3|Philipe|Morete|2/2/2018|Belo Horizonte|1400|NaN|4200|
|216|3642|HL4379|Televisão|1|Breno|Costa|8/29/2018|Belo Horizonte|2500|NaN|2500|
|217|3647|HL9962|Android|1|Bruno|Temporal|2/2/2018|Belo Horizonte|3400|NaN|3400|
|218|3659|HL9962|Android|5|Breno|Farias|11/11/2018|Belo Horizonte|3400|NaN|17000|
|219|3664|HL9962|Android|3|Lívia|Tanaka|5/11/2018|Belo Horizonte|3400|NaN|10200|
|220|3665|HL8851|Notebook|1|Gustavo|Accardo|9/16/2018|Belo Horizonte|3500|NaN|3500|
|221|3706|HL9962|Android|5|Thales|Santos|6/28/2018|Belo Horizonte|3400|NaN|17000|
|222|3734|HL4379|Televisão|3|Mônica|Rotolo|9/6/2018|Belo Horizonte|2500|NaN|7500|
|223|3739|HL1148|Câmera|5|Alex|Fernandes|9/25/2018|Belo Horizonte|2100|NaN|10500|
|224|3743|HL1918|iPhone|4|Khaio|Mesquita|11/28/2018|Belo Horizonte|5300|NaN|21200|
|225|3761|HL9962|Android|1|Pedro|Macckione|8/31/2018|Belo Horizonte|3400|NaN|3400|
|226|3766|HL1148|Câmera|1|Arthur|Pereira|11/4/2018|Belo Horizonte|2100|NaN|2100|
|227|3772|HL1918|iPhone|4|Thiago|Veloso|1/9/2018|Belo Horizonte|5300|NaN|21200|
|228|3782|HL9962|Android|4|Paloma|Sperandei|4/3/2018|Belo Horizonte|3400|NaN|13600|
|229|3800|HL1918|iPhone|1|Carolina|Silva|8/22/2018|Belo Horizonte|5300|NaN|5300|
|230|3801|HL8851|Notebook|5|Thainá|Binello|9/18/2018|Belo Horizonte|3500|NaN|17500|
|231|3852|HL7348|SmartWatch|5|Raphael|Ferman|9/3/2018|Belo Horizonte|1400|NaN|7000|
|232|3868|HL1148|Câmera|3|Maike|Pereira|2/7/2018|Belo Horizonte|2100|NaN|6300|
|233|3873|HL8851|Notebook|1|Matheus|Figueiredo|3/13/2018|Belo Horizonte|3500|NaN|3500|
|234|3891|HL2714|Tablet|4|Ives|Barbosa|1/21/2018|Belo Horizonte|1600|NaN|6400|
|235|3901|HL7348|SmartWatch|3|Larissa|Jesus|6/22/2018|Belo Horizonte|1400|NaN|4200|
|236|3907|HL8851|Notebook|3|Eric|Júnior|3/15/2018|Belo Horizonte|3500|NaN|10500|
|237|3927|HL1918|iPhone|1|Aline|Andrade|2/27/2018|Belo Horizonte|5300|NaN|5300|
|238|3934|HL1918|iPhone|5|Andressa|Rotsztejn|8/21/2018|Belo Horizonte|5300|NaN|26500|
|239|3948|HL1918|iPhone|5|Bruno|Mota|4/20/2018|Belo Horizonte|5300|NaN|26500|
|240|3978|HL7348|SmartWatch|5|Victoria|Mazza|2/23/2018|Belo Horizonte|1400|NaN|7000|
|241|3999|HL1918|iPhone|3|Bernardo|Soares|12/16/2018|Belo Horizonte|5300|NaN|15900|
|242|4000|HL1148|Câmera|4|Pedro|Martins|7/20/2018|Belo Horizonte|2100|NaN|8400|
|243|4005|HL7348|SmartWatch|1|Alon|Pestana|1/7/2018|Belo Horizonte|1400|NaN|1400|
|244|4017|HL4379|Televisão|2|Raphael|Filho|7/11/2018|Belo Horizonte|2500|NaN|5000|
|245|4019|HL8851|Notebook|5|Thomáz|Rodriguez|5/19/2018|Belo Horizonte|3500|NaN|17500|
|246|4031|HL1918|iPhone|2|Bernardo|Nauenberg|10/6/2018|Belo Horizonte|5300|NaN|10600|
|247|4060|HL4379|Televisão|4|Luiza|Marques|7/1/2018|Belo Horizonte|2500|NaN|10000|
|248|4067|HL7348|SmartWatch|2|William|Mendonça|11/12/2018|Belo Horizonte|1400|NaN|2800|
|249|4081|HL8851|Notebook|5|Anízio|Carvalho|1/9/2018|Belo Horizonte|3500|NaN|17500|
|250|4100|HL7348|SmartWatch|2|Jônatas|Castro|7/4/2018|Belo Horizonte|1400|NaN|2800|
|251|4114|HL1918|iPhone|1|Pedro|Costa|9/20/2018|Belo Horizonte|5300|NaN|5300|
|252|4117|HL1918|iPhone|4|Luiz|Mendonça|7/28/2018|Belo Horizonte|5300|NaN|21200|
|253|4118|HL1918|iPhone|5|Henrique|Oliveira|1/21/2018|Belo Horizonte|5300|NaN|26500|
|254|4120|HL1918|iPhone|2|Cassio|Faria|12/23/2018|Belo Horizonte|5300|NaN|10600|
|255|4124|HL1918|iPhone|1|Mateus|Polastri|10/24/2018|Belo Horizonte|5300|NaN|5300|
|256|4142|HL1918|iPhone|1|Paula|Cavalcanti|6/18/2018|Belo Horizonte|5300|NaN|5300|
|257|4156|HL7348|SmartWatch|2|David|Vasconcelos|11/4/2018|Belo Horizonte|1400|NaN|2800|
|258|4160|HL1918|iPhone|2|Fabio|Ramos|4/26/2018|Belo Horizonte|5300|NaN|10600|
|259|4167|HL1148|Câmera|3|Natali|Rangel|11/23/2018|Belo Horizonte|2100|NaN|6300|
|260|4182|HL1918|iPhone|2|Marina|Cormack|7/15/2018|Belo Horizonte|5300|NaN|10600|
|261|4187|HL1918|iPhone|1|Eric|Carvalho|9/20/2018|Belo Horizonte|5300|NaN|5300|
|262|4242|HL1148|Câmera|4|Bruna|Rangel|6/25/2018|Belo Horizonte|2100|NaN|8400|
|263|4254|HL2714|Tablet|2|Lucas|Reis|10/29/2018|Belo Horizonte|1600|NaN|3200|
|264|4255|HL1918|iPhone|3|Luiza|Marques|4/17/2018|Belo Horizonte|5300|NaN|15900|
|265|4268|HL1918|iPhone|3|Thales|Portillo|10/28/2018|Belo Horizonte|5300|NaN|15900|
|266|4295|HL1918|iPhone|3|Roger|Rosa|12/24/2018|Belo Horizonte|5300|NaN|15900|
|267|4300|HL8851|Notebook|1|Stefan|Santos|8/21/2018|Belo Horizonte|3500|NaN|3500|
|268|4317|HL4379|Televisão|2|Pedro|Costa|4/18/2018|Belo Horizonte|2500|NaN|5000|
|269|4354|HL1918|iPhone|2|Marina|Perdomo|1/1/2018|Belo Horizonte|5300|NaN|10600|
|270|4365|HL1918|iPhone|2|Bárbara|Lima|10/8/2018|Belo Horizonte|5300|NaN|10600|
|271|4368|HL1148|Câmera|3|Luiza|Farias|4/28/2018|Belo Horizonte|2100|NaN|6300|
|272|4376|HL4379|Televisão|2|Felipe|Paulo|1/10/2018|Belo Horizonte|2500|NaN|5000|
|273|4379|HL1918|iPhone|5|Luiz|Marinho|2/6/2018|Belo Horizonte|5300|NaN|26500|
|274|4388|HL9962|Android|3|Pedro|Rodrigues|11/18/2018|Belo Horizonte|3400|NaN|10200|
|275|4401|HL4379|Televisão|1|Luiz|Xavier|3/6/2018|Belo Horizonte|2500|NaN|2500|
|276|4421|HL4379|Televisão|2|Leonardo|Faria|12/19/2018|Belo Horizonte|2500|NaN|5000|
|277|4428|HL8851|Notebook|3|Vivianne|Rodrigues|2/19/2018|Belo Horizonte|3500|NaN|10500|
|278|4445|HL2714|Tablet|4|Priscila|Vogel|2/27/2018|Belo Horizonte|1600|NaN|6400|
|279|4448|HL8851|Notebook|1|Laura|Araujo|7/3/2018|Belo Horizonte|3500|NaN|3500|
|280|4449|HL8851|Notebook|5|Michelle|Pereira|9/2/2018|Belo Horizonte|3500|NaN|17500|
|281|4469|HL1148|Câmera|5|Leandro|Rodrigues|6/18/2018|Belo Horizonte|2100|NaN|10500|
|282|4474|HL4379|Televisão|2|Julia|Aliani|5/19/2018|Belo Horizonte|2500|NaN|5000|
|283|4477|HL8851|Notebook|1|Felipe|Cavalcanti|11/13/2018|Belo Horizonte|3500|NaN|3500|
|284|4490|HL7348|SmartWatch|2|Livia|Cozendey|8/15/2018|Belo Horizonte|1400|NaN|2800|
|285|4491|HL1918|iPhone|3|Natália|Appel|9/1/2018|Belo Horizonte|5300|NaN|15900|
|286|4516|HL1918|iPhone|5|Andressa|Nóbrega|8/9/2018|Belo Horizonte|5300|NaN|26500|
|287|4531|HL1918|iPhone|4|Joao|Silva|11/24/2018|Belo Horizonte|5300|NaN|21200|
|288|4553|HL9962|Android|1|José|Carvalho|4/12/2018|Belo Horizonte|3400|NaN|3400|
|289|4562|HL4379|Televisão|3|Henrique|Lencastre|2/21/2018|Belo Horizonte|2500|NaN|7500|
|290|4568|HL4379|Televisão|1|Julie|Ferreira|2/25/2018|Belo Horizonte|2500|NaN|2500|
|291|4571|HL4379|Televisão|3|Lara|Moreira|11/20/2018|Belo Horizonte|2500|NaN|7500|
|292|4573|HL1918|iPhone|5|Gustavo|Thome|7/6/2018|Belo Horizonte|5300|NaN|26500|
|293|4605|HL1918|iPhone|2|Luis|Silva|12/4/2018|Belo Horizonte|5300|NaN|10600|
|294|4627|HL9962|Android|3|Miguel|Carneiro|2/12/2018|Belo Horizonte|3400|NaN|10200|
|295|4645|HL4379|Televisão|4|Laura|Araujo|1/3/2018|Belo Horizonte|2500|NaN|10000|
|296|4650|HL1148|Câmera|4|Bárbara|Lima|7/1/2018|Belo Horizonte|2100|NaN|8400|
|297|4686|HL4379|Televisão|2|Rafael|Carneiro|8/30/2018|Belo Horizonte|2500|NaN|5000|
|298|4696|HL1918|iPhone|1|Paula|Calbucci|7/7/2018|Belo Horizonte|5300|NaN|5300|
|299|4717|HL1918|iPhone|2|Pedro|Macckione|7/30/2018|Belo Horizonte|5300|NaN|10600|
|300|4723|HL8851|Notebook|5|Brenno|Miranda|5/23/2018|Belo Horizonte|3500|NaN|17500|
|301|4735|HL4379|Televisão|3|Pedro|Macckione|9/30/2018|Belo Horizonte|2500|NaN|7500|
|302|4748|HL8851|Notebook|4|Wendela|Mariz|7/16/2018|Belo Horizonte|3500|NaN|14000|
|303|4755|HL8851|Notebook|3|Pedro|Sena|10/5/2018|Belo Horizonte|3500|NaN|10500|
|304|4756|HL7348|SmartWatch|4|João|Abraçado|6/25/2018|Belo Horizonte|1400|NaN|5600|
|305|4766|HL1918|iPhone|1|Marcela|Johnson|8/26/2018|Belo Horizonte|5300|NaN|5300|
|306|4788|HL2714|Tablet|3|Beatriz|Rocha|2/17/2018|Belo Horizonte|1600|NaN|4800|
|307|4811|HL1918|iPhone|2|Daniel|Nauenberg|1/19/2018|Belo Horizonte|5300|NaN|10600|
|308|4880|HL4379|Televisão|5|Juliana|Souza|3/31/2018|Belo Horizonte|2500|NaN|12500|
|309|4910|HL1918|iPhone|4|Thales|Gouvêa|6/4/2018|Belo Horizonte|5300|NaN|21200|
|310|4917|HL7348|SmartWatch|5|Pedro|Oliveira|11/21/2018|Belo Horizonte|1400|NaN|7000|
|311|4920|HL7348|SmartWatch|5|Guilherme|Assis|7/21/2018|Belo Horizonte|1400|NaN|7000|
|312|4953|HL1918|iPhone|4|Eduardo|Nunes|7/10/2018|Belo Horizonte|5300|NaN|21200|
|313|4960|HL8851|Notebook|1|Gabrielle|Silva|5/20/2018|Belo Horizonte|3500|NaN|3500|
|314|4963|HL9962|Android|5|Guilherme|Marchesi|5/3/2018|Belo Horizonte|3400|NaN|17000|
|315|4994|HL9962|Android|4|Adriana|Passos|7/5/2018|Belo Horizonte|3400|NaN|13600|
|316|5015|HL2714|Tablet|5|Thales|Santos|5/10/2018|Belo Horizonte|1600|NaN|8000|
|317|5054|HL4379|Televisão|4|Ylana|Teraoka|6/19/2018|Belo Horizonte|2500|NaN|10000|
|318|5078|HL1918|iPhone|2|Caio|Silva|8/10/2018|Belo Horizonte|5300|NaN|10600|
|319|5099|HL9962|Android|5|Milena|Almeida|4/19/2018|Belo Horizonte|3400|NaN|17000|
|320|5100|HL1148|Câmera|5|Sarah|Souza|2/11/2018|Belo Horizonte|2100|NaN|10500|
|321|5115|HL7348|SmartWatch|2|Karine|Barros|11/16/2018|Belo Horizonte|1400|NaN|2800|
|322|5139|HL4379|Televisão|4|Alon|Palmeira|2/22/2018|Belo Horizonte|2500|NaN|10000|
|323|5149|HL8851|Notebook|1|Natalia|Andrade|3/13/2018|Belo Horizonte|3500|NaN|3500|
|324|5153|HL4379|Televisão|4|João|Junior|8/14/2018|Belo Horizonte|2500|NaN|10000|
|325|5168|HL1918|iPhone|4|Carla|Zakhm|10/12/2018|Belo Horizonte|5300|NaN|21200|
|326|5190|HL9962|Android|4|Andre|Sampaio|11/2/2018|Belo Horizonte|3400|NaN|13600|
|327|5198|HL8851|Notebook|2|Guilherme|Merotto|2/27/2018|Belo Horizonte|3500|NaN|7000|
|328|5200|HL9962|Android|5|Livia|Cozendey|5/19/2018|Belo Horizonte|3400|NaN|17000|
|329|5240|HL2714|Tablet|3|Joao|Pereira|10/28/2018|Belo Horizonte|1600|NaN|4800|
|330|5244|HL4379|Televisão|1|Juan|Barbosa|12/21/2018|Belo Horizonte|2500|NaN|2500|
|331|5261|HL4379|Televisão|2|Gabriel|Puntel|3/20/2018|Belo Horizonte|2500|NaN|5000|
|332|5266|HL2714|Tablet|5|Wilson|Vianna|2/10/2018|Belo Horizonte|1600|NaN|8000|
|333|5269|HL1148|Câmera|2|Beatriz|Nogueira|11/7/2018|Belo Horizonte|2100|NaN|4200|
|334|5275|HL4379|Televisão|3|Victor|Gomes|6/11/2018|Belo Horizonte|2500|NaN|7500|
|335|5280|HL8851|Notebook|1|Eduardo|Pacheco|11/25/2018|Belo Horizonte|3500|NaN|3500|
|336|5307|HL4379|Televisão|5|José|Jesus|8/12/2018|Belo Horizonte|2500|NaN|12500|
|337|5314|HL1918|iPhone|3|Anízio|Carvalho|9/25/2018|Belo Horizonte|5300|NaN|15900|
|338|5330|HL1918|iPhone|5|Eric|Carvalho|12/26/2018|Belo Horizonte|5300|NaN|26500|
|339|5338|HL1918|iPhone|5|Amanda|Procaci|8/28/2018|Belo Horizonte|5300|NaN|26500|
|340|5341|HL8851|Notebook|2|Amanda|Machado|8/16/2018|Belo Horizonte|3500|NaN|7000|
|341|5358|HL9962|Android|1|Bruna|Franco|9/30/2018|Belo Horizonte|3400|NaN|3400|
|342|5363|HL1148|Câmera|2|Luíza|Melo|10/4/2018|Belo Horizonte|2100|NaN|4200|
|343|5379|HL4379|Televisão|2|Luiza|Farias|4/2/2018|Belo Horizonte|2500|NaN|5000|
|344|5424|HL1918|iPhone|1|Gabriel|Pereira|2/23/2018|Belo Horizonte|5300|NaN|5300|
|345|5449|HL1148|Câmera|2|Glenda|Santos|4/3/2018|Belo Horizonte|2100|NaN|4200|
|346|5468|HL1918|iPhone|3|Raphael|Mattos|9/21/2018|Belo Horizonte|5300|NaN|15900|
|347|5479|HL1148|Câmera|4|Helena|Chafin|11/18/2018|Belo Horizonte|2100|NaN|8400|
|348|5499|HL9962|Android|5|Wendela|Mariz|12/12/2018|Belo Horizonte|3400|NaN|17000|
|349|5517|HL1918|iPhone|5|Morgana|Correa|11/3/2018|Belo Horizonte|5300|NaN|26500|
|350|5541|HL8851|Notebook|4|Gabrielle|Porto|12/29/2018|Belo Horizonte|3500|NaN|14000|
|351|5557|HL1918|iPhone|4|Audir|Franco|11/16/2018|Belo Horizonte|5300|NaN|21200|
|352|5570|HL2714|Tablet|1|Patrícia|Ferreira|5/24/2018|Belo Horizonte|1600|NaN|1600|
|353|5577|HL7348|SmartWatch|3|Gabriella|Lopes|10/30/2018|Belo Horizonte|1400|NaN|4200|
|354|5581|HL4379|Televisão|2|Silvio|Fahrnholz|5/6/2018|Belo Horizonte|2500|NaN|5000|
|355|5584|HL4379|Televisão|5|Breno|Caputo|6/26/2018|Belo Horizonte|2500|NaN|12500|
|356|5587|HL2714|Tablet|5|Beatriz|Cavalcanti|5/21/2018|Belo Horizonte|1600|NaN|8000|
|357|5597|HL4379|Televisão|5|Bruna|Ramos|2/10/2018|Belo Horizonte|2500|NaN|12500|
|358|5601|HL7348|SmartWatch|3|João|Alves|9/11/2018|Belo Horizonte|1400|NaN|4200|
|359|5621|HL1918|iPhone|4|Bruna|Soares|5/4/2018|Belo Horizonte|5300|NaN|21200|
|360|5643|HL9962|Android|5|Diego|Rodrigues|5/9/2018|Belo Horizonte|3400|NaN|17000|
|361|5648|HL8851|Notebook|1|Mayara|Soares|11/12/2018|Belo Horizonte|3500|NaN|3500|
|362|5650|HL8851|Notebook|3|Andre|Sampaio|7/18/2018|Belo Horizonte|3500|NaN|10500|
|363|5673|HL9962|Android|2|Isabella|Santos|11/28/2018|Belo Horizonte|3400|NaN|6800|
|364|5687|HL1918|iPhone|1|Lucas|Machado|9/6/2018|Belo Horizonte|5300|NaN|5300|
|365|5708|HL7348|SmartWatch|1|Carolina|Bernardes|11/4/2018|Belo Horizonte|1400|NaN|1400|
|366|5750|HL9962|Android|3|Allan|Candido|3/4/2018|Belo Horizonte|3400|NaN|10200|
|367|5751|HL9962|Android|1|Lucas|Reis|10/31/2018|Belo Horizonte|3400|NaN|3400|
|368|5756|HL7348|SmartWatch|3|Mariana|Sousa|1/6/2018|Belo Horizonte|1400|NaN|4200|
|369|5775|HL1148|Câmera|2|Lucas|Aragão|3/17/2018|Belo Horizonte|2100|NaN|4200|
|370|5788|HL7348|SmartWatch|1|Isaac|Santos|8/13/2018|Belo Horizonte|1400|NaN|1400|
|371|5833|HL1148|Câmera|5|Daniel|Valente|5/26/2018|Belo Horizonte|2100|NaN|10500|
|372|5872|HL8851|Notebook|3|Beatriz|Perdomo|6/2/2018|Belo Horizonte|3500|NaN|10500|
|373|5884|HL2714|Tablet|5|Elena|Barreto|3/8/2018|Belo Horizonte|1600|NaN|8000|
|374|5903|HL2714|Tablet|3|Guilherme|Jordao|5/25/2018|Belo Horizonte|1600|NaN|4800|
|375|5904|HL8851|Notebook|2|Morgana|Correa|9/22/2018|Belo Horizonte|3500|NaN|7000|
|376|5908|HL1918|iPhone|5|Glenda|Santos|6/16/2018|Belo Horizonte|5300|NaN|26500|
|377|5968|HL1918|iPhone|1|Carlos|Assis|6/8/2018|Belo Horizonte|5300|NaN|5300|
|378|5983|HL1918|iPhone|3|Rafael|Guimarães|9/2/2018|Belo Horizonte|5300|NaN|15900|
|379|5996|HL9962|Android|1|Carlos|Cardoso|7/9/2018|Belo Horizonte|3400|NaN|3400|
|380|6001|HL4379|Televisão|2|Marianna|Pestana|6/30/2018|Belo Horizonte|2500|NaN|5000|
|381|6012|HL8851|Notebook|4|Lucas|Coelho|10/1/2018|Belo Horizonte|3500|NaN|14000|
|382|6015|HL1918|iPhone|1|João|Fonseca|3/23/2018|Belo Horizonte|5300|NaN|5300|
|383|6028|HL8851|Notebook|4|Jeferson|Costa|6/14/2018|Belo Horizonte|3500|NaN|14000|
|384|6042|HL4379|Televisão|1|Milena|Almeida|10/21/2018|Belo Horizonte|2500|NaN|2500|
|385|6050|HL1918|iPhone|1|Cézar|Santos|12/26/2018|Belo Horizonte|5300|NaN|5300|
|386|6059|HL4379|Televisão|5|Beatriz|Santos|1/6/2018|Belo Horizonte|2500|NaN|12500|
|387|6103|HL4379|Televisão|1|Marcelo|Pereira|1/13/2018|Belo Horizonte|2500|NaN|2500|
|388|6108|HL1918|iPhone|2|Pedro|Macckione|6/6/2018|Belo Horizonte|5300|NaN|10600|
|389|6125|HL9962|Android|4|Pedro|Pereira|6/8/2018|Belo Horizonte|3400|NaN|13600|
|390|6168|HL9962|Android|3|Laura|Araujo|11/8/2018|Belo Horizonte|3400|NaN|10200|
|391|6203|HL4379|Televisão|1|Paula|Carneiro|6/16/2018|Belo Horizonte|2500|NaN|2500|
|392|6211|HL2714|Tablet|5|Ulisses|Arruda|1/14/2018|Belo Horizonte|1600|NaN|8000|
|393|6226|HL9962|Android|5|Sthefeson|Pereira|9/15/2018|Belo Horizonte|3400|NaN|17000|
|394|6238|HL9962|Android|2|Rafael|Ramos|7/24/2018|Belo Horizonte|3400|NaN|6800|
|395|6240|HL9962|Android|3|Adrielle|Forte|1/31/2018|Belo Horizonte|3400|NaN|10200|
|396|6249|HL4379|Televisão|1|Mateus|Franco|10/14/2018|Belo Horizonte|2500|NaN|2500|
|397|6257|HL2714|Tablet|3|Julie|Ferreira|6/7/2018|Belo Horizonte|1600|NaN|4800|
|398|6294|HL1148|Câmera|4|Julia|Silva|1/1/2018|Belo Horizonte|2100|NaN|8400|
|399|6303|HL1918|iPhone|2|Julie|Ferreira|6/26/2018|Belo Horizonte|5300|NaN|10600|
|400|6311|HL4379|Televisão|5|Natália|Appel|10/19/2018|Belo Horizonte|2500|NaN|12500|
|401|6316|HL1918|iPhone|4|Raissa|Sales|3/3/2018|Belo Horizonte|5300|NaN|21200|
|402|6317|HL1918|iPhone|1|Guilherme|Merotto|5/14/2018|Belo Horizonte|5300|NaN|5300|
|403|6324|HL1918|iPhone|2|Paulo|Campos|10/11/2018|Belo Horizonte|5300|NaN|10600|
|404|6346|HL4379|Televisão|1|Bruna|Ramos|11/12/2018|Belo Horizonte|2500|NaN|2500|
|405|6377|HL9962|Android|2|Rodrigo|Feijo|12/1/2018|Belo Horizonte|3400|NaN|6800|
|406|6380|HL1148|Câmera|3|Carlos|Araujo|6/24/2018|Belo Horizonte|2100|NaN|6300|
|407|6409|HL4379|Televisão|2|Joao|Silva|7/2/2018|Belo Horizonte|2500|NaN|5000|
|408|6418|HL4379|Televisão|4|Paula|Cavalcanti|2/18/2018|Belo Horizonte|2500|NaN|10000|
|409|6428|HL1918|iPhone|5|Glenda|Santos|12/8/2018|Belo Horizonte|5300|NaN|26500|
|410|6439|HL1918|iPhone|2|Daniel|Ortiz|9/27/2018|Belo Horizonte|5300|NaN|10600|
|411|6444|HL2714|Tablet|1|Sthefeson|Kohn|6/13/2018|Belo Horizonte|1600|NaN|1600|
|412|6500|HL4379|Televisão|2|Camilla|Cardeman|10/3/2018|Belo Horizonte|2500|NaN|5000|
|413|6508|HL1148|Câmera|4|Daniel|Terra|7/30/2018|Belo Horizonte|2100|NaN|8400|
|414|6513|HL1918|iPhone|5|Giuseppe|Borges|9/1/2018|Belo Horizonte|5300|NaN|26500|
|415|6540|HL4379|Televisão|1|Lucas|Destri|7/17/2018|Belo Horizonte|2500|NaN|2500|
|416|6547|HL1918|iPhone|4|Marcelo|Guadagnino|1/11/2018|Belo Horizonte|5300|NaN|21200|
|417|6570|HL1918|iPhone|1|Priscila|Suzano|5/26/2018|Belo Horizonte|5300|NaN|5300|
|418|6584|HL1918|iPhone|5|Carlos|Souza|3/9/2018|Belo Horizonte|5300|NaN|26500|
|419|6587|HL8851|Notebook|3|Ives|Barbosa|11/20/2018|Belo Horizonte|3500|NaN|10500|
|420|6590|HL2714|Tablet|2|Caroll|Johnson|6/22/2018|Belo Horizonte|1600|NaN|3200|
|421|6594|HL1148|Câmera|4|Juliana|Correa|2/17/2018|Belo Horizonte|2100|NaN|8400|
|422|6604|HL4379|Televisão|4|Andressa|Nóbrega|2/27/2018|Belo Horizonte|2500|NaN|10000|
|423|6639|HL4379|Televisão|3|Isabella|Montanholi|7/29/2018|Belo Horizonte|2500|NaN|7500|
|424|6648|HL2714|Tablet|5|Samara|Pinto|3/4/2018|Belo Horizonte|1600|NaN|8000|
|425|6667|HL1918|iPhone|4|Bianca|Ferezin|2/9/2018|Belo Horizonte|5300|NaN|21200|
|426|6681|HL2714|Tablet|4|Danilo|Rubim|8/2/2018|Belo Horizonte|1600|NaN|6400|
|427|6705|HL1918|iPhone|5|Julia|Leig|7/2/2018|Belo Horizonte|5300|NaN|26500|
|428|6707|HL4379|Televisão|2|Caroline|Cavalcanti|5/9/2018|Belo Horizonte|2500|NaN|5000|
|429|6718|HL1918|iPhone|2|Caio|Cardoso|5/29/2018|Belo Horizonte|5300|NaN|10600|
|430|6761|HL1918|iPhone|3|Raíza|Lopes|3/30/2018|Belo Horizonte|5300|NaN|15900|
|431|6765|HL1918|iPhone|2|Stephanie|Oliveira|3/12/2018|Belo Horizonte|5300|NaN|10600|
|432|6766|HL4379|Televisão|2|Alessandra|Martins|12/24/2018|Belo Horizonte|2500|NaN|5000|
|433|6781|HL1918|iPhone|1|Débora|Lopes|6/10/2018|Belo Horizonte|5300|NaN|5300|
|434|6804|HL1918|iPhone|1|Jéssica|Stefanelli|1/22/2018|Belo Horizonte|5300|NaN|5300|
|435|6805|HL1918|iPhone|2|Laura|Araujo|4/7/2018|Belo Horizonte|5300|NaN|10600|
|436|6807|HL7348|SmartWatch|3|Antonio|Manhães|11/29/2018|Belo Horizonte|1400|NaN|4200|
|437|6817|HL1918|iPhone|1|Renan|Melo|10/2/2018|Belo Horizonte|5300|NaN|5300|
|438|6828|HL4379|Televisão|1|Ives|Teixeira|9/26/2018|Belo Horizonte|2500|NaN|2500|
|439|6830|HL7348|SmartWatch|5|Maria|Junior|7/27/2018|Belo Horizonte|1400|NaN|7000|
|440|6867|HL1918|iPhone|5|Marina|Aragão|4/4/2018|Belo Horizonte|5300|NaN|26500|
|441|6880|HL1918|iPhone|3|Paula|Carneiro|2/16/2018|Belo Horizonte|5300|NaN|15900|
|442|6896|HL4379|Televisão|5|João|Monteiro|4/20/2018|Belo Horizonte|2500|NaN|12500|
|443|6897|HL4379|Televisão|5|Caroll|Johnson|12/5/2018|Belo Horizonte|2500|NaN|12500|
|444|6903|HL1148|Câmera|4|Guilherme|Seixas|10/18/2018|Belo Horizonte|2100|NaN|8400|
|445|6910|HL1918|iPhone|3|Pedro|Costa|12/28/2018|Belo Horizonte|5300|NaN|15900|
|446|6939|HL4379|Televisão|4|Michelle|Pereira|6/12/2018|Belo Horizonte|2500|NaN|10000|
|447|6948|HL1918|iPhone|3|Gustavo|Erthal|7/19/2018|Belo Horizonte|5300|NaN|15900|
|448|6961|HL1148|Câmera|4|João|Silva|8/6/2018|Belo Horizonte|2100|NaN|8400|
|449|6997|HL2714|Tablet|1|João|Capitulo|8/21/2018|Belo Horizonte|1600|NaN|1600|
|450|7009|HL4379|Televisão|1|Ana|Gomes|2/23/2018|Belo Horizonte|2500|NaN|2500|
|451|7031|HL1148|Câmera|5|Felipe|Freitas|4/12/2018|Belo Horizonte|2100|NaN|10500|
|452|7034|HL1918|iPhone|4|Luiz|Marinho|3/20/2018|Belo Horizonte|5300|NaN|21200|
|453|7079|HL1918|iPhone|4|Carlos|Silva|9/3/2018|Belo Horizonte|5300|NaN|21200|
|454|7081|HL1918|iPhone|2|Priscila|Carvalho|7/24/2018|Belo Horizonte|5300|NaN|10600|
|455|7090|HL2714|Tablet|3|Jéssica|Resinente|2/19/2018|Belo Horizonte|1600|NaN|4800|
|456|7109|HL1918|iPhone|4|Juan|Fernandes|12/21/2018|Belo Horizonte|5300|NaN|21200|
|457|7112|HL1148|Câmera|5|Michelle|Miura|8/5/2018|Belo Horizonte|2100|NaN|10500|
|458|7118|HL1918|iPhone|4|Raísa|Rodrigues|3/20/2018|Belo Horizonte|5300|NaN|21200|
|459|7123|HL1918|iPhone|3|Vanessa|Bach|12/18/2018|Belo Horizonte|5300|NaN|15900|
|460|7132|HL4379|Televisão|4|Leandro|Ferreira|1/14/2018|Belo Horizonte|2500|NaN|10000|
|461|7136|HL4379|Televisão|4|Matheus|Gomes|11/6/2018|Belo Horizonte|2500|NaN|10000|
|462|7144|HL1918|iPhone|4|Caroline|Cavalcanti|10/6/2018|Belo Horizonte|5300|NaN|21200|
|463|7145|HL1918|iPhone|5|Andressa|Rotsztejn|6/15/2018|Belo Horizonte|5300|NaN|26500|
|464|7148|HL4379|Televisão|2|Lucas|Lacerda|4/21/2018|Belo Horizonte|2500|NaN|5000|
|465|7170|HL1148|Câmera|1|Wilson|Vianna|3/15/2018|Belo Horizonte|2100|NaN|2100|
|466|7208|HL1918|iPhone|2|Maria|Mello|5/1/2018|Belo Horizonte|5300|NaN|10600|
|467|7225|HL8851|Notebook|3|Alberto|Silveira|5/17/2018|Belo Horizonte|3500|NaN|10500|
|468|7241|HL8851|Notebook|5|Wilson|Meirelles|5/23/2018|Belo Horizonte|3500|NaN|17500|
|469|7257|HL1918|iPhone|4|Paula|Cavalcanti|7/17/2018|Belo Horizonte|5300|NaN|21200|
|470|7269|HL1918|iPhone|1|Thainá|Binello|9/5/2018|Belo Horizonte|5300|NaN|5300|
|471|7274|HL2714|Tablet|5|Matheus|Delgado|2/26/2018|Belo Horizonte|1600|NaN|8000|
|472|7283|HL4379|Televisão|2|Rubens|Netto|10/31/2018|Belo Horizonte|2500|NaN|5000|
|473|7287|HL4379|Televisão|3|Beatriz|Silva|2/16/2018|Belo Horizonte|2500|NaN|7500|
|474|7299|HL1918|iPhone|5|Arthur|Pereira|11/6/2018|Belo Horizonte|5300|NaN|26500|
|475|7313|HL1918|iPhone|5|Caio|Caldas|4/20/2018|Belo Horizonte|5300|NaN|26500|
|476|7335|HL4379|Televisão|3|Juliana|Correa|3/24/2018|Belo Horizonte|2500|NaN|7500|
|477|7341|HL2714|Tablet|1|Anderson|Cavalcanti|10/28/2018|Belo Horizonte|1600|NaN|1600|
|478|7374|HL1918|iPhone|2|Maria|Correa|7/26/2018|Belo Horizonte|5300|NaN|10600|
|479|7376|HL8851|Notebook|2|Diego|Mello|6/18/2018|Belo Horizonte|3500|NaN|7000|
|480|7400|HL1918|iPhone|5|Iuri|Barbosa|7/3/2018|Belo Horizonte|5300|NaN|26500|
|481|7424|HL8851|Notebook|3|Alexandre|Rodriguez|3/28/2018|Belo Horizonte|3500|NaN|10500|
|482|7465|HL9962|Android|2|Sandy|Ribeiro|10/2/2018|Belo Horizonte|3400|NaN|6800|
|483|7491|HL1148|Câmera|3|Arthur|Pereira|9/22/2018|Belo Horizonte|2100|NaN|6300|
|484|7495|HL9962|Android|4|Roberto|Mattos|1/29/2018|Belo Horizonte|3400|NaN|13600|
|485|7512|HL7348|SmartWatch|4|Clara|Bruno|11/20/2018|Belo Horizonte|1400|NaN|5600|
|486|7516|HL2714|Tablet|5|Gabrielle|Costa|1/25/2018|Belo Horizonte|1600|NaN|8000|
|487|7523|HL8851|Notebook|4|Adrielle|Vieira|4/1/2018|Belo Horizonte|3500|NaN|14000|
|488|7563|HL1918|iPhone|5|Raphael|Kurtz|2/16/2018|Belo Horizonte|5300|NaN|26500|
|489|7607|HL2714|Tablet|3|Luana|Santana|2/16/2018|Belo Horizonte|1600|NaN|4800|
|490|7608|HL2714|Tablet|4|Maria|Costa|3/7/2018|Belo Horizonte|1600|NaN|6400|
|491|7620|HL8851|Notebook|5|Thaís|Moura|11/30/2018|Belo Horizonte|3500|NaN|17500|
|492|7637|HL1918|iPhone|2|Maria|Cardoso|3/27/2018|Belo Horizonte|5300|NaN|10600|
|493|7645|HL4379|Televisão|1|Luis|Silva|8/1/2018|Belo Horizonte|2500|NaN|2500|
|494|7659|HL1148|Câmera|1|Maria|Gasperi|7/25/2018|Belo Horizonte|2100|NaN|2100|
|495|7662|HL4379|Televisão|1|Amanda|Procaci|9/23/2018|Belo Horizonte|2500|NaN|2500|
|496|7696|HL1918|iPhone|5|Alexandre|Rodriguez|10/31/2018|Belo Horizonte|5300|NaN|26500|
|497|7701|HL9962|Android|2|Fernanda|Figueiredo|11/25/2018|Belo Horizonte|3400|NaN|6800|
|498|7704|HL1918|iPhone|5|Clara|Silveira|8/26/2018|Belo Horizonte|5300|NaN|26500|
|499|7721|HL4379|Televisão|2|Gabriela|Mello|5/7/2018|Belo Horizonte|2500|NaN|5000|
|500|7730|HL2714|Tablet|1|Izabel|Lopes|5/11/2018|Belo Horizonte|1600|NaN|1600|
|501|7736|HL7348|SmartWatch|3|Amanda|Gontijo|1/1/2018|Belo Horizonte|1400|NaN|4200|
|502|7790|HL9962|Android|3|Amanda|Felippe|9/13/2018|Belo Horizonte|3400|NaN|10200|
|503|7799|HL4379|Televisão|2|Júlia|Almeida|2/4/2018|Belo Horizonte|2500|NaN|5000|
|504|7854|HL7348|SmartWatch|3|Matheus|Delgado|8/5/2018|Belo Horizonte|1400|NaN|4200|
|505|7862|HL2714|Tablet|4|Breno|Godoy|3/29/2018|Belo Horizonte|1600|NaN|6400|
|506|7888|HL4379|Televisão|2|Raíssa|Oliveira|10/4/2018|Belo Horizonte|2500|NaN|5000|
|507|7895|HL7348|SmartWatch|3|Rodrigo|Silva|11/6/2018|Belo Horizonte|1400|NaN|4200|
|508|7905|HL1148|Câmera|2|Maike|Pereira|5/11/2018|Belo Horizonte|2100|NaN|4200|
|509|7908|HL9962|Android|1|Miguel|Carneiro|1/8/2018|Belo Horizonte|3400|NaN|3400|
|510|7916|HL8851|Notebook|4|Victor|Firmino|9/1/2018|Belo Horizonte|3500|NaN|14000|
|511|7924|HL1918|iPhone|5|Eduardo|Veiga|3/1/2018|Belo Horizonte|5300|NaN|26500|
|512|7942|HL2714|Tablet|2|Kim|Ferreira|10/5/2018|Belo Horizonte|1600|NaN|3200|
|513|7957|HL1918|iPhone|3|Carolina|Rachide|7/20/2018|Belo Horizonte|5300|NaN|15900|
|514|7964|HL9962|Android|4|Willian|Albino|3/1/2018|Belo Horizonte|3400|NaN|13600|
|515|7983|HL9962|Android|3|Lucas|Machado|12/24/2018|Belo Horizonte|3400|NaN|10200|
|516|8008|HL1148|Câmera|1|Amanda|Braga|7/6/2018|Belo Horizonte|2100|NaN|2100|
|517|8009|HL8851|Notebook|1|Lucas|Costa|10/8/2018|Belo Horizonte|3500|NaN|3500|
|518|8011|HL1918|iPhone|2|Felipe|Mendonça|9/2/2018|Belo Horizonte|5300|NaN|10600|
|519|8014|HL4379|Televisão|2|João|Menezes|5/23/2018|Belo Horizonte|2500|NaN|5000|
|520|8039|HL7348|SmartWatch|2|Maria|Cardoso|1/21/2018|Belo Horizonte|1400|NaN|2800|
|521|8051|HL4379|Televisão|4|Rojane|Lima|6/24/2018|Belo Horizonte|2500|NaN|10000|
|522|8062|HL1918|iPhone|3|Breno|Caputo|7/18/2018|Belo Horizonte|5300|NaN|15900|
|523|8069|HL9962|Android|2|Victor|Oliveira|7/20/2018|Belo Horizonte|3400|NaN|6800|
|524|8070|HL1918|iPhone|2|Mariana|Sousa|2/8/2018|Belo Horizonte|5300|NaN|10600|
|525|8079|HL9962|Android|5|Ulisses|Filho|7/25/2018|Belo Horizonte|3400|NaN|17000|
|526|8081|HL1148|Câmera|3|Gabriel|Rocha|4/22/2018|Belo Horizonte|2100|NaN|6300|
|527|8082|HL7348|SmartWatch|3|Helvio|Pedrosa|3/3/2018|Belo Horizonte|1400|NaN|4200|
|528|8086|HL9962|Android|2|Maria|Moita|1/2/2018|Belo Horizonte|3400|NaN|6800|
|529|8094|HL1918|iPhone|4|Rafaela|Gonçalves|4/15/2018|Belo Horizonte|5300|NaN|21200|
|530|8100|HL4379|Televisão|1|Camilla|Vieira|7/23/2018|Belo Horizonte|2500|NaN|2500|
|531|8104|HL2714|Tablet|5|Antônio|Oliveira|11/11/2018|Belo Horizonte|1600|NaN|8000|
|532|8128|HL1918|iPhone|3|Izabel|Lopes|9/19/2018|Belo Horizonte|5300|NaN|15900|
|533|8152|HL9962|Android|2|Guido|Monteiro|12/24/2018|Belo Horizonte|3400|NaN|6800|
|534|8168|HL7348|SmartWatch|2|Morgana|Correa|7/2/2018|Belo Horizonte|1400|NaN|2800|
|535|8178|HL8851|Notebook|4|Ana|Júnior|11/23/2018|Belo Horizonte|3500|NaN|14000|
|536|8205|HL4379|Televisão|1|Isabela|Resende|9/6/2018|Belo Horizonte|2500|NaN|2500|
|537|8254|HL1918|iPhone|3|Bruno|Velucci|4/14/2018|Belo Horizonte|5300|NaN|15900|
|538|8256|HL1148|Câmera|3|Jeferson|Sone|10/31/2018|Belo Horizonte|2100|NaN|6300|
|539|8257|HL1918|iPhone|3|Eduardo|Veiga|1/30/2018|Belo Horizonte|5300|NaN|15900|
|540|8272|HL7348|SmartWatch|4|Breno|Varella|9/7/2018|Belo Horizonte|1400|NaN|5600|
|541|8283|HL9962|Android|4|Maria|Junior|3/20/2018|Belo Horizonte|3400|NaN|13600|
|542|8284|HL4379|Televisão|5|Matheus|Sapir|11/23/2018|Belo Horizonte|2500|NaN|12500|
|543|8292|HL4379|Televisão|4|Julia|Figueiredo|11/20/2018|Belo Horizonte|2500|NaN|10000|
|544|8299|HL4379|Televisão|5|Juan|Barbosa|12/1/2018|Belo Horizonte|2500|NaN|12500|
|545|8304|HL1918|iPhone|3|Pedro|Rodrigues|4/23/2018|Belo Horizonte|5300|NaN|15900|
|546|8396|HL4379|Televisão|4|Raul|Junqueira|6/14/2018|Belo Horizonte|2500|NaN|10000|
|547|8401|HL4379|Televisão|3|Lucas|Rodrigues|7/5/2018|Belo Horizonte|2500|NaN|7500|
|548|8438|HL2714|Tablet|5|Luíza|Melo|9/25/2018|Belo Horizonte|1600|NaN|8000|
|549|8447|HL1918|iPhone|2|Júlio|Fraga|9/7/2018|Belo Horizonte|5300|NaN|10600|
|550|8459|HL1918|iPhone|4|Lívia|Marques|1/5/2018|Belo Horizonte|5300|NaN|21200|
|551|8467|HL4379|Televisão|4|Wilson|Meirelles|12/16/2018|Belo Horizonte|2500|NaN|10000|
|552|8499|HL2714|Tablet|2|Amanda|Amaral|10/25/2018|Belo Horizonte|1600|NaN|3200|
|553|8500|HL1918|iPhone|5|Julia|Leite|1/1/2018|Belo Horizonte|5300|NaN|26500|
|554|8502|HL2714|Tablet|3|Giselia|Thiele|6/25/2018|Belo Horizonte|1600|NaN|4800|
|555|8508|HL7348|SmartWatch|1|Wilson|Brandão|5/19/2018|Belo Horizonte|1400|NaN|1400|
|556|8538|HL9962|Android|5|Juliana|Goes|9/29/2018|Belo Horizonte|3400|NaN|17000|
|557|8569|HL9962|Android|3|Gabriel|Silva|6/3/2018|Belo Horizonte|3400|NaN|10200|
|558|8595|HL2714|Tablet|2|Jéssica|Netto|2/19/2018|Belo Horizonte|1600|NaN|3200|
|559|8609|HL1918|iPhone|4|Rilson|Dias|4/16/2018|Belo Horizonte|5300|NaN|21200|
|560|8633|HL1918|iPhone|2|Rodrigo|Bruno|2/14/2018|Belo Horizonte|5300|NaN|10600|
|561|8684|HL9962|Android|4|João|Pedrazza|7/9/2018|Belo Horizonte|3400|NaN|13600|
|562|8698|HL7348|SmartWatch|2|Gabrielle|Costa|8/29/2018|Belo Horizonte|1400|NaN|2800|
|563|8719|HL1918|iPhone|4|Daniela|Rosa|11/14/2018|Belo Horizonte|5300|NaN|21200|
|564|8739|HL1918|iPhone|5|Maria|Cardoso|3/21/2018|Belo Horizonte|5300|NaN|26500|
|565|8749|HL4379|Televisão|1|Gustavo|Erthal|5/3/2018|Belo Horizonte|2500|NaN|2500|
|566|8791|HL2714|Tablet|2|Bruno|Ursulino|1/28/2018|Belo Horizonte|1600|NaN|3200|
|567|8808|HL1918|iPhone|3|Eduardo|Soares|10/16/2018|Belo Horizonte|5300|NaN|15900|
|568|8826|HL4379|Televisão|2|Lucas|Valim|12/25/2018|Belo Horizonte|2500|NaN|5000|
|569|8840|HL8851|Notebook|1|Marcela|Gasperi|7/11/2018|Belo Horizonte|3500|NaN|3500|
|570|8843|HL1148|Câmera|1|Amanda|Procaci|12/28/2018|Belo Horizonte|2100|NaN|2100|
|571|8858|HL8851|Notebook|5|Roberto|Mattos|6/13/2018|Belo Horizonte|3500|NaN|17500|
|572|8862|HL9962|Android|1|Renan|Melo|12/13/2018|Belo Horizonte|3400|NaN|3400|
|573|8871|HL8851|Notebook|3|Camille|Silva|1/8/2018|Belo Horizonte|3500|NaN|10500|
|574|8899|HL8851|Notebook|4|Caio|Ferreira|1/18/2018|Belo Horizonte|3500|NaN|14000|
|575|8915|HL1918|iPhone|4|Maria|Costa|4/17/2018|Belo Horizonte|5300|NaN|21200|
|576|8942|HL8851|Notebook|1|Marcos|Nucci|8/3/2018|Belo Horizonte|3500|NaN|3500|
|577|8954|HL4379|Televisão|2|Willian|Albino|3/31/2018|Belo Horizonte|2500|NaN|5000|
|578|8957|HL1918|iPhone|4|João|Matheus|10/23/2018|Belo Horizonte|5300|NaN|21200|
|579|8968|HL1918|iPhone|4|Pedro|Rodrigues|7/16/2018|Belo Horizonte|5300|NaN|21200|
|580|8978|HL1918|iPhone|1|Luana|Santana|8/25/2018|Belo Horizonte|5300|NaN|5300|
|581|9009|HL8851|Notebook|4|Jackson|Derossi|3/7/2018|Belo Horizonte|3500|NaN|14000|
|582|9022|HL2714|Tablet|2|Iuri|Barbosa|11/25/2018|Belo Horizonte|1600|NaN|3200|
|583|9050|HL4379|Televisão|4|Carolina|Santos|11/24/2018|Belo Horizonte|2500|NaN|10000|
|584|9055|HL7348|SmartWatch|2|Rubens|Valente|12/2/2018|Belo Horizonte|1400|NaN|2800|
|585|9065|HL1918|iPhone|3|Lucas|Almeida|6/29/2018|Belo Horizonte|5300|NaN|15900|
|586|9067|HL4379|Televisão|1|Isabela|Resende|12/20/2018|Belo Horizonte|2500|NaN|2500|
|587|9068|HL8851|Notebook|5|João|Araujo|3/20/2018|Belo Horizonte|3500|NaN|17500|
|588|9124|HL7348|SmartWatch|1|João|Costa|3/15/2018|Belo Horizonte|1400|NaN|1400|
|589|9142|HL8851|Notebook|3|Anderson|Cavalcanti|6/27/2018|Belo Horizonte|3500|NaN|10500|
|590|9148|HL9962|Android|2|Carolina|Abrahão|9/26/2018|Belo Horizonte|3400|NaN|6800|
|591|9178|HL4379|Televisão|1|Rubens|Valente|6/9/2018|Belo Horizonte|2500|NaN|2500|
|592|9191|HL4379|Televisão|3|Beatriz|Silva|8/10/2018|Belo Horizonte|2500|NaN|7500|
|593|9205|HL4379|Televisão|5|Manuela|Ferreira|3/29/2018|Belo Horizonte|2500|NaN|12500|
|594|9243|HL7348|SmartWatch|5|Carlos|Barbosa|7/5/2018|Belo Horizonte|1400|NaN|7000|
|595|9281|HL1918|iPhone|3|João|Luz|9/30/2018|Belo Horizonte|5300|NaN|15900|
|596|9287|HL1918|iPhone|5|Patrícia|Fernandes|10/8/2018|Belo Horizonte|5300|NaN|26500|
|597|9292|HL1148|Câmera|3|Henrique|Oliveira|2/7/2018|Belo Horizonte|2100|NaN|6300|
|598|9297|HL8851|Notebook|1|Luiza|Cavalcanti|1/18/2018|Belo Horizonte|3500|NaN|3500|
|599|9301|HL9962|Android|5|Anna|Silva|7/16/2018|Belo Horizonte|3400|NaN|17000|
|600|9331|HL1918|iPhone|5|Caio|Caldas|5/13/2018|Belo Horizonte|5300|NaN|26500|
|601|9339|HL7348|SmartWatch|4|Ana|Soledade|6/23/2018|Belo Horizonte|1400|NaN|5600|
|602|9341|HL4379|Televisão|1|David|Vasconcelos|9/18/2018|Belo Horizonte|2500|NaN|2500|
|603|9351|HL2714|Tablet|5|João|Fonseca|7/10/2018|Belo Horizonte|1600|NaN|8000|
|604|9380|HL9962|Android|2|Fabio|Sepúlveda|9/28/2018|Belo Horizonte|3400|NaN|6800|
|605|9402|HL4379|Televisão|4|Wen|Braga|5/14/2018|Belo Horizonte|2500|NaN|10000|
|606|9410|HL1918|iPhone|4|Bernardo|Nauenberg|9/18/2018|Belo Horizonte|5300|NaN|21200|
|607|9422|HL4379|Televisão|2|João|Abraçado|9/21/2018|Belo Horizonte|2500|NaN|5000|
|608|9441|HL1148|Câmera|2|Jônatas|Tanaka|1/12/2018|Belo Horizonte|2100|NaN|4200|
|609|9456|HL7348|SmartWatch|1|Fernanda|Coutinho|11/28/2018|Belo Horizonte|1400|NaN|1400|
|610|9463|HL9962|Android|1|Maria|Costa|11/24/2018|Belo Horizonte|3400|NaN|3400|
|611|9487|HL4379|Televisão|3|Beatriz|Perdomo|6/4/2018|Belo Horizonte|2500|NaN|7500|
|612|9492|HL1918|iPhone|1|Gabriel|Puntel|2/6/2018|Belo Horizonte|5300|NaN|5300|
|613|9501|HL7348|SmartWatch|2|Lucas|Rodrigues|10/28/2018|Belo Horizonte|1400|NaN|2800|
|614|9514|HL4379|Televisão|2|Raphael|Guedes|2/11/2018|Belo Horizonte|2500|NaN|5000|
|615|9528|HL1918|iPhone|4|Larissa|Jesus|12/21/2018|Belo Horizonte|5300|NaN|21200|
|616|9553|HL8851|Notebook|5|Eduardo|Nunes|10/30/2018|Belo Horizonte|3500|NaN|17500|
|617|9579|HL9962|Android|1|Caio|Silva|10/25/2018|Belo Horizonte|3400|NaN|3400|
|618|9596|HL2714|Tablet|1|Bernardo|Soares|11/29/2018|Belo Horizonte|1600|NaN|1600|
|619|9632|HL4379|Televisão|1|Julia|Silva|5/14/2018|Belo Horizonte|2500|NaN|2500|
|620|9634|HL2714|Tablet|3|Mariana|Freire|3/4/2018|Belo Horizonte|1600|NaN|4800|
|621|9639|HL2714|Tablet|5|Bernard|Pedrosa|10/13/2018|Belo Horizonte|1600|NaN|8000|
|622|9643|HL4379|Televisão|5|Breno|Godoy|2/11/2018|Belo Horizonte|2500|NaN|12500|
|623|9645|HL1918|iPhone|5|Bianca|Paz|10/11/2018|Belo Horizonte|5300|NaN|26500|
|624|9667|HL8851|Notebook|2|Lucas|Almeida|11/21/2018|Belo Horizonte|3500|NaN|7000|
|625|9671|HL1918|iPhone|3|Carla|Zakhm|10/26/2018|Belo Horizonte|5300|NaN|15900|
|626|9679|HL4379|Televisão|2|Henrique|Villanova|12/23/2018|Belo Horizonte|2500|NaN|5000|
|627|9699|HL7348|SmartWatch|2|Carolina|Rachide|1/17/2018|Belo Horizonte|1400|NaN|2800|
|628|9709|HL7348|SmartWatch|3|João|Peçanha|5/30/2018|Belo Horizonte|1400|NaN|4200|
|629|9729|HL1148|Câmera|2|Rodrigo|Mendes|2/4/2018|Belo Horizonte|2100|NaN|4200|
|630|9734|HL2714|Tablet|2|Thomaz|Ferreira|4/24/2018|Belo Horizonte|1600|NaN|3200|
|631|9755|HL1918|iPhone|2|Milena|Pereira|1/24/2018|Belo Horizonte|5300|NaN|10600|
|632|9757|HL4379|Televisão|3|Paula|Cavalcanti|12/20/2018|Belo Horizonte|2500|NaN|7500|
|633|9758|HL1918|iPhone|3|Anna|Silva|7/30/2018|Belo Horizonte|5300|NaN|15900|
|634|9769|HL2714|Tablet|3|Bruno|Ferreira|8/14/2018|Belo Horizonte|1600|NaN|4800|
|635|9772|HL8851|Notebook|2|Carlos|Azevedo|11/18/2018|Belo Horizonte|3500|NaN|7000|
|636|9779|HL1918|iPhone|3|Viviane|Souza|7/9/2018|Belo Horizonte|5300|NaN|15900|
|637|9789|HL4379|Televisão|2|Gustavo|Accardo|3/14/2018|Belo Horizonte|2500|NaN|5000|
|638|9818|HL4379|Televisão|4|Kim|Ferreira|7/13/2018|Belo Horizonte|2500|NaN|10000|
|639|9840|HL1918|iPhone|4|Fernanda|Bhering|1/12/2018|Belo Horizonte|5300|NaN|21200|
|640|9845|HL2714|Tablet|4|João|Pedrazza|12/1/2018|Belo Horizonte|1600|NaN|6400|
|641|9850|HL1148|Câmera|5|Bruno|Salomão|7/28/2018|Belo Horizonte|2100|NaN|10500|
|642|9864|HL1148|Câmera|4|Patrick|Silva|3/1/2018|Belo Horizonte|2100|NaN|8400|
|643|9883|HL9962|Android|3|Breno|Britto|3/26/2018|Belo Horizonte|3400|NaN|10200|
|644|9910|HL1148|Câmera|4|Norman|Jimbo|2/17/2018|Belo Horizonte|2100|NaN|8400|
|645|9927|HL2714|Tablet|2|Marina|Marins|1/29/2018|Belo Horizonte|1600|NaN|3200|
|646|9932|HL1918|iPhone|1|José|Vieira|5/11/2018|Belo Horizonte|5300|NaN|5300|
|647|9942|HL4379|Televisão|1|Fernanda|Junior|2/9/2018|Belo Horizonte|2500|NaN|2500|
|648|9978|HL8851|Notebook|2|Mariane|Racy|12/28/2018|Belo Horizonte|3500|NaN|7000|

