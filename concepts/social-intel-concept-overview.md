---
title: Visão geral da inteligência social e do local de trabalho no Microsoft Graph
description: As centenas de milhões de usuários que utilizam os serviços de nuvem do Microsoft 365 fazem parte do núcleo do Microsoft Graph. Os dados dos usuários são cuidadosamente gerenciados, protegidos e, com a autorização adequada, disponibilizados pelos serviços do Microsoft Graph para promover a criatividade e a produtividade em empresas. Mesmo os dados do usuário sendo onipresentes no Microsoft Graph, os dados derivados das interações do usuário são especialmente interessantes.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: bf50bcd6d55b9c31ebb6ecca4d176ef230bb2bc8
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450491"
---
# <a name="overview-of-social-and-workplace-intelligence-in-microsoft-graph"></a>Visão geral da inteligência social e do local de trabalho no Microsoft Graph

As centenas de milhões de usuários que utilizam os serviços de nuvem do Microsoft 365 fazem parte do núcleo do Microsoft Graph. Os dados dos usuários são cuidadosamente gerenciados, protegidos e, com a autorização adequada, disponibilizados pelos serviços do Microsoft Graph para promover a criatividade e a produtividade em empresas. Mesmo os dados do usuário sendo onipresentes no Microsoft Graph, os dados derivados das interações do usuário são especialmente interessantes. Eles fornece informações inteligentes que podem responder a perguntas como:

- "Quem esse usuário deve contatar para obter informações sobre esse tópico?"
- "Quais documentos são interessantes para essa pessoa?"

Você pode usar a API de Pessoas e a API do Insights no Microsoft Graph para criar aplicativos mais inteligentes que podem, respectivamente, acessar as pessoas e os documentos relevantes para um usuário.

A API de Pessoas retorna as pessoas por ordem de relevância para um usuário com base nos contatos do usuário, em suas redes sociais, seu diretório organizacional e suas comunicações recentes por email e Skype. Isso é particularmente útil para cenários de seleção de pessoas.

A API do Insights usa análises e avançadas e o aprendizado de máquina para fornecer os arquivos mais relevantes de que os usuários precisam ao longo de seu dia de trabalho. Essa API capacita experiências familiares do Office 365, incluindo o Office Delve, a página inicial do SharePoint, o modo de exibição Descoberta do OneDrive for Business e o Outlook na Web.

![As APIs de Pessoas e do Insights retornam pessoas e documentos relevantes para um usuário](images/social-intel-concept-overview-data.png)

## <a name="why-integrate-with-people-data"></a>Por que se integrar com dados de pessoas?

A API de Pessoas retorna dados de uma única entidade, [person](/graph/api/resources/person?view=graph-rest-1.0), que inclui dados típicos de um indivíduo no mundo de negócios de hoje. O que torna esses dados de **pessoa** especialmente úteis é sua _relevância_ em relação a um usuário do Microsoft Graph. A relevância é identificada por meio de uma pontuação para cada pessoa, que é calculada com base nos padrões de colaboração e comunicação e nas relações de negócios do usuário. Há 3 tipos principais de aplicações para esses dados de _relevância_.

### <a name="browse-people-by-relevance"></a>Procurar pessoas pela relevância

Você pode procurar pessoas que estão relacionadas ao usuário conectado ou a outro usuário na organização do usuário conectado, desde que você tenha a [autorização](people-example.md#authorization) apropriada. Você obtém um conjunto de objetos **person** ordenados pela relevância. Você pode [personalizar](people-example.md#browse-people) mais a coleção de objetos **person** retornados na resposta ao especificar os parâmetros de consulta `top`, `skip`, `orderby`, `select` e `filter`.

### <a name="fuzzy-searches-based-on-people-criteria"></a>Pesquisas difusas baseadas em critérios de pessoas

A API de Pessoas permite pesquisar por pessoas relevantes para o usuário conectado, desde que o aplicativo tenha permissões desse usuário. (Leia mais em [permissões de pessoas](permissions-reference.md#people-permissions).)

Essas pesquisas retornam resultados com base em uma correspondência exata e também em inferências sobre a intenção da pesquisa. Para ilustrar isso, o exemplo a seguir retorna objetos **person** relevantes para o usuário conectado cujo nome _ou endereço de email_ contém uma palavra que começa com "j".

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

### <a name="fuzzy-searches-based-on-topic-criteria"></a>Pesquisas baseadas em critérios de tópico

A API de Pessoas também permite que você realize pesquisas por pessoas relevantes para o usuário conectado e que tenham manifestado interesse em se comunicar com esse usuário sobre determinados tópicos. Os tópicos são apenas palavras que os usuários usaram com mais frequência nas conversas de email. A Microsoft extrai essas palavras, sem qualquer contexto, e cria um índice para esses dados para facilitar pesquisas difusas.

O exemplo a seguir ilustra inferências sobre a finalidade de uma pesquisa sobre o tópico "beetle":

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search="topic:beetle" 
```

Uma pesquisa difusa no índice de dados de tópico retorna instâncias que significam o nome em inglês do inseto besouro, o icônico carro Beetle da Volkswagen, a banda Beatles e outras definições.


## <a name="why-integrate-with-document-based-insights-preview"></a>Por que se integrar com informações baseadas em documentos (visualização)?

### <a name="use-intelligence-to-improve-collaboration"></a>Use inteligência para melhorar a colaboração

Durante um dia de trabalho típico, usuários frequentemente interagem com grandes quantidades de informações armazenadas em muitos documentos e colaboram com outros usuários de muitas maneiras diferentes. É importante que eles sempre possam encontrar o precisam no momento certo.

Você pode usar a API do Insights, que inclui as APIs [trending](/graph/api/resources/insights-trending?view=graph-rest-beta), [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) e [used](/graph/api/resources/insights-used?view=graph-rest-beta) para localizar arquivos no Office 365 com base no contexto e nas necessidades atuais dos seus usuários, tornando os usuários mais produtivos e melhorando a colaboração em sua organização.

É fácil renderizar os resultados da API do Insights em seu aplicativo. Cada resultado acompanha um conjunto de propriedades de visualização comuns, como uma URL de imagem de visualização ou um texto de visualização.

### <a name="make-relevant-content-visible"></a>Tornar o conteúdo relevante visível

No Office 365, o Delve usa informações de _tendências_ para ajudar os usuários a descobrir os documentos que são mais interessantes para eles no momento. Veja a Figura 1.

É possível usar a entidade [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) de forma programática na API do Insights para proporcionar uma experiência semelhante aos clientes do seu aplicativo. Use a entidade **trending** para se conectar aos documentos que mais relevantes para o usuário e mais populares ao seu redor. A opção [Listar documentos mais populares](/graph/api/insights-list-trending?view=graph-rest-beta) retornará arquivos armazenados em sites de equipe do SharePoint ou no OneDrive, classificados por relevância, com os mais importantes primeiro. 

**Figura 1. Delve no Office 365 mostrando documentos populares para um usuário**

![Captura de tela do Delve no Office 365 mostrando documentos populares para um usuário](images/delve-concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a>Permitir que os usuários colaborem e voltem ao trabalho

Os novos cartões de pessoas do Office 365 utilizam as informações _used_ e _shared_ para conectar os dados entre pessoas e informações. O cartão de pessoas identifica e exibe documentos relevantes sobre uma pessoa. Os usuários podem ver cartões de pessoas em todo o pacote Office, por exemplo, no Outlook na Web. Veja a Figura 2.

A API do Insights fornece uma com uma funcionalidade semelhante às entidades [used](/graph/api/resources/insights-used?view=graph-rest-beta) e [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) entidades. Elas retornam o que um usuário tem visualizado e trabalhado mais recentemente, ou o que colegas compartilharam com o usuário mais recentemente no Office 365.

**Figura 2. Outlook na Web, mostrando um cartão de pessoas para um usuário**

![Captura de tela de um cartão de pessoas para um usuário no Outlook na Web, mostrando os arquivos recentes](images/peoplecard-concept.png)

## <a name="why-integrate-with-myanalytics-preview"></a>Por que integrar o MyAnalytics (visualização)?


  [O myAnalytics](https://docs.microsoft.com/pt-BR/workplace-analytics/myanalytics/index) fornece uma visão geral de como e com quem as pessoas passam o tempo. Esses dados podem ajudar as pessoas a planejar o dia, obter informações sobre seus diferentes padrões de trabalho e ajudar a equilibrar o trabalho e a vida.

A API de análises permite a sincronização ou a integração de dados de análise do usuário com um aplicativo de terceiros personalizado para oferecer suporte a uma ampla variedade de cenários que podem ajudar a melhorar a produtividade e a colaboração do usuário. Por exemplo, você poderia integrar dados do myAnalytics com atividades de dispositivos móveis para ajudar os usuários a acompanhar todas as atividades de trabalho e social e planejar o seu dia dentro de um aplicativo.

## <a name="api-reference"></a>Referência da API

Procurando a referência de API para estes serviços?

- [API de Pessoas no Microsoft Graph v1.0](/graph/api/resources/social-overview?view=graph-rest-1.0)
- [Use a API do Microsoft Graph para integrar inteligência social e de local de trabalho em um aplicativo](/graph/api/resources/social-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

* Use o [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para experimentar as APIs de pessoas, Insights e análises com seus próprios arquivos. Entre e escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para habilitar **Pessoas**, **Insights (beta)** e **Análises**.
* Saiba mais sobre a [API de Pessoas](people-example.md) e a entidade [person](/graph/api/resources/person?view=graph-rest-1.0).
* Para começar a usar a API do Insights, consulte [Usar a API do Insights](/graph/api/resources/insights?view=graph-rest-beta).
* Saiba mais sobre a [API de análise](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-balance-work-and-life).
