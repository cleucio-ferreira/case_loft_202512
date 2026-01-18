---
aliases: 
tags: 
autor: Cleucio Diogo Bastos Ferreira
criado em:
atualizado em: 
atualizado por: 
classificações:
  - Em desenvolvimento
---
Este projeto foi desenvolvido por: Cleucio Diogo Bastos Ferreira
# Agradecimento

Primeiramente gostaria de agradecer pelo tempo e pela dedicação durante este processo seletivo, fiquei muito feliz e empolgado de participar dele.
Achei todas as etapas muito construtivas e coerentes com o desafio proposto, parabéns pelo ótimo trabalho.

A seguir, fiz um resumo de tudo que foi feito, para facilitar e guiar a sua exploração, espero que gostem. 
Obrigado.
# Estrutura do projeto
## Tratamento e analise de dados

Esta etapa implementa um pipeline de dados em python responsável por preparar, explorar, tratar e adicionar dados/informações relevantes ao modelo.
O código contém várias analises, algumas não geei artefatos, pois não vi uma aplicação pratica para o time. No caso das mais relevantes gerei os seguintes artefatos: 

- **df_consolidado.xlsx**: arquivo que unifica e simplifica os a base de dados contemplando todos os tratamento e adições aplicadas ao modelo. O objetivo deste arquivo é prover uma fonte segura, controlada e tratada para os gestores poderem fazer suas análises pontuais.

- **outliers_acionamentos.xlsx**: arquivo contendo uma lista de contratos, que não honraram com seus compromissos, e  sem reversão de status. O objetivo deste fornecer recomendações e priorização para os contratos não acionados ou acionados com bastante intensidade.

- imagens: todas as imagens geradas pelo código como mapas de calor e histogramas ficam armazenadas para analise separadamente. O objetivo deste recursos é facilitar o compartilhamento das informações, sem a necessidade de compartilhar o código.

- starr_squema: pasta contendo as bases tratadas e enriquecidas para serem consumidas pelo PBI. O objetivo desse passo é gerar automaticamente as bases de forma controlada a partir dos dados da origem garantindo a padronização e a governança dos dados. 

>[!important]
Devido a baixa complexidade da entrada dos dados, escolhi o google colab para criar o pipeline, pela facilidade de desenvolvimento e compartilhamento. O código esta disponível em: `./case_loft_202512/case_loft_20251209.ipynb`

>[!warning]
>Todos os arquivos de entrada de dados estão armazenados em: `./case_loft_202512/input`
>Todos os artefatos gerados pelo código são exportados automaticamente para: `./case_loft_202512/output`
>
>*Exceto o `star_schema` que é armazenado na pasta de input, pois será consumido na próxima etapa.*
## Visualização de dados

Para visualização dos dados escolhi o PBI, pela sua flexibilidade, pela familiaridade com a ferramenta e pela ampla disponibilidade de documentação, isso apesar de estar  enferrujado, por estar trabalhando apenas com a parte de código, nos últimos 6 meses. O backgroud do dashboard foi construído no `Figma` e esta disponível em [Projeto case Lofte 202512](https://www.figma.com/design/nWfsXRCGVuMc83ImT4OFa7/loft?node-id=1-25&p=f&t=MnWfzTFp5qujtnz6-0)

O design do dashboard é simples e baseado no site oficial da empresa. Como não foi fornecido a paleta de cores, foram utilizadas cores obtidas na página oficial aproximadas. O objetivo do dashboard foi demonstrar as habilidades de visualização de dados, sem sobrepor ou tentar entregar as mesmas analises e ou informações das demais ferramentas utilizadas.

A paleta de cores foi escolhida utilizando a ferramenta [coolors](https://coolors.co/2e4756-16262e-248232-9883e5-2ba84a), que gera cores complementares a partir de cores pré-definidas.

![600x300](capa_dash.png)

![600x300](volume.png)
Na imagem acima foi selecionado os meses do ano de 2023, para aplicar o comparativo.

>[!important]
>O dashboad pode ser encontrado em: ``./case_loft_202512/output/dashboard/case_202512.pbip*
>
>*Escolho salvar com essa extensão por já ter o modelo semântico e scrips TDML separados para facilitar na documentação.*
## Documentação

Além da documentação funciona do código disponível no próprio arquivo do google colab, a documentação do projeto é composta por:

Orientações gerais:  `./case_loft_202512/Leia me.pdf` ( arquivo atual )
Aprendizado e recomendações:  `./case_loft_202512/output/documentacao/Case Loft 202512 - Aprendizados e recomendações.pdf`
Pontos de atenção e sugestões: `./case_loft_202512/output/documentacao/Case Loft 202512 - Pontos de atenção e sugestões.pdf`

>[!Nota]
>A documentação foi gerada integralmente utilizando a linguagem `markdown` e  os recursos disponibilizados pelo o software Obsidian, que é um ótimo gestor de arquivos do tipo markdown.

Desenvolvido por: Cleucio Diogo Bastos Ferreira