# Sistema de Recomendação de Imóveis

## **Introdução**

Encontrar o imóvel ideal pode ser uma tarefa desafiadora e muitas vezes frustrante. A dificuldade em encontrar uma propriedade que atenda ao gosto pessoal, orçamento e necessidades individuais, aliada à subjetividade na correspondência das expectativas com o corretor, pode tornar esse processo ainda mais complexo. Neste artigo, exploraremos uma solução inovadora baseada em Inteligência Artificial (IA) que visa superar esses obstáculos e proporcionar uma experiência eficiente e satisfatória na busca por imóveis.

## **O Desafio da Busca por Imóveis**

### **Dificuldades Enfrentadas**

1. **Personalização do Gosto**: Cada pessoa possui preferências únicas quando se trata de um imóvel. Encontrar uma propriedade que se alinhe perfeitamente com essas preferências é um desafio, já que as opções disponíveis muitas vezes não correspondem ao gosto individual.
2. **Restrições Orçamentárias**: O orçamento desempenha um papel crucial na decisão de compra ou aluguel de um imóvel. Encontrar opções que atendam às restrições financeiras do comprador muitas vezes é uma tarefa árdua.
3. **Subjetividade na Correspondência**: A comunicação entre o cliente e o corretor pode ser complexa. A subjetividade na compreensão das expectativas do cliente pode levar a mal-entendidos e frustrações ao longo do processo.

Para superar esses desafios, propomos a utilização de um sistema de recomendação alimentado por Inteligência Artificial. Este sistema é projetado para entender e aprender com as preferências do usuário, bem como para fornecer sugestões de imóveis que atendam tanto ao gosto quanto ao orçamento.

### **Metodologia e Dados Utilizados**

Para desenvolver e treinar o modelo, utilizamos uma abordagem de coleta de dados diversificada:

1. **Web Scraping**: Coletamos informações de 50 páginas da web relacionadas a imóveis (OLX) no Centro de São Paulo. Esses dados incluíam detalhes dos anúncios e links para as páginas individuais de cada imóvel.
2. **Dados de Endereço**: Os endereços foram obtidos através de duas fontes: uma base de CEPs e a API dos Correios. Esses endereços são cruciais para fornecer informações precisas sobre a localização dos imóveis.
3. **Tratamento de Dados**: Realizamos uma série de tratamentos nos dados coletados, eliminando imóveis com informações insuficientes e tratando valores atípicos, como áreas e valores de condomínio irreais.

### **Funcionamento do Modelo**

O modelo se baseia em um algoritmo de aprendizado de máquina (ensemble) que leva em consideração tanto os aspectos subjetivos quanto objetivos na busca por imóveis. Vejamos como ele funciona:

1. **Entrada de Dados**: O usuário fornece informações detalhadas por meio do aplicativo, incluindo uma descrição livre e filtros relacionados às suas preferências.
2. **Pré-processamento**: O modelo utiliza técnicas avançadas de processamento de linguagem natural para analisar a descrição do usuário e os filtros selecionados.
3. **Agrupamento de Dados**: Com base em técnicas como Latent Semantic Indexing (LSI) e Latent Dirichlet Allocation (LDA), o sistema agrupa os imóveis em clusters ou tópicos relevantes.
4. **Recomendações Personalizadas**: O modelo sugere inicialmente os imóveis mais próximos às preferências do usuário. Ele também utiliza a técnica LSI para comparar a descrição dos imóveis curtidos com outros imóveis, buscando semelhanças e afinidades ocultas.
5. **Feedback Contínuo**: Com base nas interações do usuário, o modelo (ensemble) aprende e refina suas recomendações ao longo do tempo. O usuário pode até mesmo fornecer sugestões, permitindo um aprimoramento constante do sistema.

## **Benefícios para Diferentes Envolvidos**

### **Vantagens para o Mercado Imobiliário**

Essa abordagem traz uma alternativa moderna ao mercado imobiliário, alinhando-se à revolução digital em que vivemos. Ao incorporar tais tecnologias, o setor imobiliário pode oferecer uma experiência mais eficiente e satisfatória aos clientes.

### **Experiência Aprimorada para Clientes**

Os compradores e inquilinos se beneficiam significativamente com essa solução. Eles não precisam mais gastar tempo navegando por várias páginas e imóveis que não se adequam às suas preferências. O sistema de recomendação direciona-os diretamente às opções mais relevantes, economizando tempo e energia.

### **Facilitação do Trabalho dos Corretores**

Os corretores de imóveis também encontram vantagens nesse modelo. Ele age como um auxílio valioso, ajudando a compreender as preferências subjetivas dos clientes. Isso permite que os corretores otimizem suas interações e aumentem a precisão das correspondências.

## **Resultados e Conclusões**

A economia significativa de tempo em comparação com métodos tradicionais é notável. Os usuários não precisam mais navegar por inúmeras páginas para encontrar uma opção adequada.

No entanto, reconhecemos que ajustes e testes adicionais são necessários para aprimorar o modelo. Testes mais abrangentes e dados mais diversificados permitirão uma validação mais sólida e uma otimização contínua.

Em última análise, a aplicação bem-sucedida desse sistema de recomendação pode transformar a experiência de busca por imóveis, tornando-a mais personalizada, eficiente e satisfatória para todos os envolvidos.
