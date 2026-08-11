**A diferença entre dado e informação:**

Elmasri e Navathe (2019), dados representam fatos brutos, valores isolados que, por si só, não detém significado contextual específico. São elementos básicos, como números, textos, datas ou símbolos, que existem independentemente de qualquer interpretação. 

A informação, por sua vez, emerge quando os dados são processados, organizados e contextualizados de forma a adquirir significado e relevância para quem os utiliza (Date, 2004).

**Um banco de dados bem projetado deve ser capaz de armazenar dados de forma eficiente e permitir que eles sejam transformados em informações valiosas a partir de consultas, relatórios e análises.**

**Características dos Dados:**

Os dados possuem características específicas que devem ser consideradas durante o processo de modelagem.

**Os dados são atômicos:** Representam a menor unidade de informação que pode ser armazenada sem perder seu significado intrínseco. 

**Os dados são persistentes:** uma vez armazenados adequadamente, devem permanecer disponíveis até que sejam explicitamente removidos ou modificados.

**Os dados possuem granularidade:** Podem ser coletados e armazenados em diferentes níveis de detalhamento.

Exemplo:

Em um sistema de vendas, armazenamos dados agregados (referentes às vendas mensais) ou dados detalhados (correspondentes a cada transação individual). 

A escolha do nível de granularidade impacta diretamente a flexibilidade das consultas futuras e o desempenho do sistema.

**Hierarquia Data-Information-Knowledge-Wisdom (DIKW):**

*A Hierarquia DIKW mostra como evoluímos de dados brutos até a sabedoria.*

**Dados:** Fatos brutos sem contexto.

**Informação:** Dados organizados.

**Conhecimento:** Informação aplicada na prática.

**Sabedoria:** Conhecimento usado com bom senso e julgamento.

**É a base do Business Intelligence para transformar dados simples em decisões estratégicas.**

**Transformação de Dados em Informação:**

Dividimos em 5 etapas, cada etapa define a forma de modelar tabelas, criar índices, gatilhos (triggers) e proceimentos armazenados (stored procedures):

**1. Coleta (captura):** Capta os dados brutos de diferentes fontes.

**2. Validação (qualidade):** Garante que os dados estejam corretos e dentro do padrão.

**3. Processamento (organização):** Organiza, cruza e calcula os dados.

Exemplo:

*Soma vendas diárias para gerar o total do mês.*

**4. Contextualização (significado):** Aplica regras de negócio para dar sentido aos dados processados.

**5. Apresentação (visualização):** Exibe tudo em relatórios, dashboards ou telas como informação útil.

