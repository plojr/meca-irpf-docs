# MeCa-IRPF

## Resumo
Este projeto é para aqueles que compram ações no mercado à vista na B3 e precisam de dados para declarar no software da Receita Federal. Ele é um dos módulos de um projeto pessoal chamado MeCa.

## Disclaimer
Não usem esta aplicação como verdade absoluta. Eu estudei como calcular cada dado, porém erros podem acontecer. Interpretações diferentes também podem acontecer. Por isso, sugiro que usem esta aplicação só para comparar com os seus próprios cálculos. Não me responsabilizo por informações erradas que esta aplicação possa apresentar, já que ela estará em constante evolução. Caso encontre alguma diferença discrepante com seus próprios cálculos, e se estiver disposto/disposta a encontrar qual parte do código está com problema, sinta-se à vontade para corrigi-lo.

Eu nunca fiz um cálculo manual para lançar os dados no programa da Receita Federal e utilizo o algoritmo desta aplicação há mais de 5 anos. Nunca tive problemas com os dados declarados para a Receita Federal. Espero continuar assim. :-)

Por fim, gostaria de deixar claro que este módulo, MeCa-IRPF, só serve para lançar os dados relativos a ações no mercado à vista. Isso significa que derivativos, commodities etc não devem ser lançados aqui.

## Objetivo
O intuito destes módulos é fornecer os dados que você precisa lançar no programa da Receita Federal, em "Bens e Direitos", "Rendimentos isentos" e também na parte de "Renda Variável". Em "Bens e Direitos", serão lançados seus ativos, o CNPJ da empresa e a situação no dia 31/12. Em "Renda Variável", será possível lançar o lucro acumulado para as vendas em até 20.000,00, os prejuízos de cada mês, o lucro mensal - e também o imposto de renda que deverá pagar em cima dele - para vendas que ultrapassarem os 20.000,00 e também os lucros e prejuízos que obtiver nos day trade.

## Como devo lançar as notas de corretagem?
A minha sugestão é que você lance, preferencialmente, todas as suas notas de corretagem. Existe um tipo de caso onde isso não é preciso. É quando você está com sua posição de ações totalmente zerada, isto é, sem ter nenhuma ação em sua carteira. Neste caso, você pode começar a lançar as ações que comprar a partir de então, desde que você não queira saber dos dados de anos anteriores. Porém, se esse não for o seu caso, o custo das compras feitas de uma determinada ação no passado pode influenciar, ou não, no custo atual. Não influenciaria no custo atual dadas algumas condições bem específicas.
Com isso em mente, eu sugiro lançar todas as notas. Eu sei que é trabalhoso, mas é o cenário ideal para evitar cálculos errados.

## Módulos - Resumo

O módulo mais básico é o de cadastro, onde você pode lançar as ordens, notas de corretagem, eventos corporativos etc.

O segundo módulo é o de day trade, que calcula os valores que você precisa usar para pagar o DARF, relativo aos day trade. Além disso, é mantido um eventual prejuízo acumulado para que o investidor possa usar no futuro.

Um terceiro módulo é o que calcula a carteira do investidor.

O quarto módulo é o de swing trade. Este leva em consideração os eventos corporativos do módulo de cadastro.

Um ponto a ficar claro é que alguns módulos são interdependentes e outros não. Antes de usar os módulos day trade, carteira e swing trade, cadastre todas as notas de corretagem e eventos corporativos pelo módulo de cadastro, pois todos dependem dele.

Nas pastas relativas a cada módulo, você pode encontrar mais detalhes de cada projeto.