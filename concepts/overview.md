---
title: Visão geral do Microsoft Graph
description: O Microsoft Graph é o gateway para dados e inteligência no Microsoft 365. O Microsoft Graph fornece um modelo de programabilidade unificada que você pode usar para aproveitar a enorme quantidade de dados disponíveis no Office 365, no Enterprise Mobility + Security e no Windows 10.
author: jthake-msft
ms.openlocfilehash: 754580e0f5a6af628a2bf18c11a0a20d3c2d1329
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349039"
---
# <a name="overview-of-microsoft-graph"></a>Visão geral do Microsoft Graph

O Microsoft Graph é o gateway para dados e inteligência no Microsoft 365. O Microsoft Graph fornece um modelo de programabilidade unificada que você pode usar para aproveitar a enorme quantidade de dados disponíveis no Office 365, no Enterprise Mobility + Security e no Windows 10. 

Você pode usar a API do Microsoft Graph para criar aplicativos para organizações e clientes que interagem com os dados de milhões de usuários. Com o Microsoft Graph, você pode se conectar a uma ampla variedade de recursos, relações e inteligência, tudo por um único ponto de extremidade: `https://graph.microsoft.com`.

## <a name="whats-in-the-graph"></a>O que há no gráfico?
O Microsoft Graph expõe as APIs REST e bibliotecas do cliente para acessar dados no seguinte:

- Azure Active Directory
- Serviços do Office 365: SharePoint, OneDrive, Outlook/Exchange, Microsoft Teams, OneNote, Planner e Excel
- Serviços do Enterprise Mobility + Security: Identity Manager, Intune, Advanced Threat Analytics e Advanced Threat Protection.
- Serviços do Windows 10: atividades e dispositivos
- Educação

Para saber mais, veja os [principais serviços e recursos do Microsoft Graph](overview-major-services.md).

O Microsoft Graph conecta todos os recursos entre esses serviços usando relações. Por exemplo, um usuário pode estar conectado a um grupo por meio de uma relação [memberOf](/graph/api/user-list-memberof?view=graph-rest-1.0)e com outro usuário por uma relação [manager](/graph/api/user-list-manager?view=graph-rest-1.0). O aplicativo pode desviar dessas relações para acessar esses recursos conectados e executar ações neles pela API.

Você também pode obter informações valiosas e inteligência sobre os dados pelo Microsoft Graph. Por exemplo, você pode obter os arquivos [mais populares](/graph/api/resources/insights-trending?view=graph-rest-beta) para um determinado usuário ou [obter as pessoas mais relevantes](/graph/api/user-list-people?view=graph-rest-beta) para um usuário.

Descubra as possibilidades nas relações dentro do Microsoft Graph.

![Uma imagem mostrando os recursos principais e as relações que fazem parte do gráfico](images/microsoft-graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>O que você pode fazer com o Microsoft Graph? 

Você pode usar o Microsoft Graph para criar experiências de acordo com o contexto exclusivo do usuário para ajudá-lo a ser mais produtivo. Imagine um aplicativo que...

- Analisa sua próxima reunião e o ajuda a se preparar para ela ao fornecer informações de perfil dos participantes, incluindo os cargos e com quem eles trabalham, bem como informações sobre os documentos e projetos mais recentes nos quais eles estão trabalhando.
- Verifica seu calendário e sugere os horários recomendados para a próxima reunião de equipe.
- Busca o gráfico de projeção mais recente das vendas de um arquivo do Excel em seu OneDrive e permite atualizar a previsão em tempo real, tudo em seu telefone.
- Assina alterações em seu calendário, envia um alerta quando você está gastando muito tempo em reuniões e oferece recomendações sobre as que você pode perder ou delegar com base na relevância dos participantes para você.
- Ajuda você a classificar informações pessoais e profissionais em seu telefone, por exemplo, categorizando imagens que devem seguir para seu OneDrive pessoal e recibos comerciais que devem seguir para seu OneDrive for Business.

Você pode fazer tudo isso e muito mais com a API do Microsoft Graph.

>
  **Observação:** ao usar a API do Microsoft Graph, você concorda com os [Termos de Uso do Microsoft Graph](https://developer.microsoft.com/graph/docs/misc/terms-of-use) e com a [Política de Privacidade da Microsoft](https://go.microsoft.com/fwlink/?LinkId=521839).

### <a name="popular-requests"></a>Solicitações mais usadas

Veja alguns desses cenários mais comuns para trabalhar com a API do Microsoft Graph. Os links levam você ao [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

| **Operação** | **URL** |
|:--------------------------|:----------------------------------------|
|   GET meu perfil |    [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   GET meus arquivos | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   GET minha foto | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   GET meu email |   [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   GET meu email de alta prioridade | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   OBTER eventos do meu calendário |    [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   GET meu gerente  | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   GET o último usuário que modificou o arquivo foo.txt |  [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   OBTER grupos do Office365 dos quais eu sou membro| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   GET os usuários em minha organização     | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   OBTER grupos em minha organização | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   GET as pessoas relacionadas a mim    | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   Itens GET mais populares à minha volta |  [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   GET my notes |  [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="access-microsoft-graph-at-scale"></a>Acessar o Microsoft Graph em escala


O Microsoft Graph Data Connect habilita acesso em massa (em vez do tradicional acesso transacional) aos dados do Office 365. Com os dados em massa do Office 365, você pode usar as ferramentas do Azure para criar aplicativos inteligentes que:

- Encontram para você o especialista em um determinado tópico mais próximo em sua organização 
- Automatizam a criação de base de dados de conhecimento
- Analisam solicitações de reunião para fornecer insights sobre o uso de sala de conferência
- Detectam fraudes envolvendo dados de comunicação e de produtividade

## <a name="when-should-i-use-microsoft-graph-data-connect"></a>Por que devo usar o Microsoft Graph Data Connect?

O Microsoft Graph Data Connect fornece uma nova maneira de interagir com os dados que estão disponíveis por meio de APIs do Microsoft Graph. Além de fornecer acesso escalonável aos dados do Office 365, o Microsoft Graph Data Connect também fornece um conjunto exclusivo de recursos que facilitam o desenvolvimento de aplicativos inteligentes, tudo isso na nuvem da Microsoft.

|**Recurso**| **API do Microsoft Graph** | **Microsoft Graph Data Connect** |
|:----------|:------------------------|:--------------------------------------|
| **Escopo de acesso** | Usuário único ou locatário inteiro | Muitos usuários ou grupos |
| **Padrão de acesso** | Tempo real | Cronograma recorrente |
| **Operações de dados** | Funciona em mestre de dados | Funciona em um cache dos dados |
| **Proteção de dados** | Os dados são protegidos enquanto estão no Microsoft 365 | A proteção de dados é estendida ao cache dos dados em sua assinatura do Azure |
| **Consentimento do usuário** | Self<br>Tipos de recursos | Nenhum |
| **Consentimento do administrador** | Toda a organização<br>Tipos de recursos | Selecione grupos de usuários<br>Propriedades e tipos de recursos<br>Exclui usuários |
| **Ferramentas de acesso** | Consultas da Web RESTful | Azure Data Factory |

Para obter mais informações sobre o Microsoft Graph Data Connect, veja [Microsoft Graph Data Connect](data-connect-overview.md). Para começar, veja [Visão geral do Microsoft Graph Data Connect](data-connect-concept-overview.md). 

## <a name="next-steps"></a>Próximas etapas

- Confira alguns [cenários em destaque](https://developer.microsoft.com/graph/examples).
- Experimente um exemplo de solicitação no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Use o [início rápido](https://developer.microsoft.com/graph/quick-start) para configurar um aplicativo de exemplo pronto para funcionar.
- Consulte o item **Saiba mais** no índice para ler sobre os serviços e recursos que você pode usar em seus cenários. 
- Descubra como [obter um token de autenticação](auth-overview.md) em seu aplicativo.
- Comece a [usar a API](use-the-api.md).

## <a name="feedback"></a>Comentários?

Seus comentários são importantes para nós. Junte-se a nós na página [Stack Overflow](https://stackoverflow.com/questions/tagged/office365+or+microsoftgraph). Marque suas perguntas com {MicrosoftGraph}.

