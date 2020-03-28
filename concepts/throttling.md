---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 3889f23353b46c852547501c59d8a94653c67b75
ms.sourcegitcommit: 2ac179fb774a15c9e9c01502e59c76efb57803a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2020
ms.locfileid: "42986145"
---
# <a name="microsoft-graph-throttling-guidance"></a>Diretrizes de limitação do Microsoft Graph

Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.

Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>O que acontece quando a limitação ocorre?
<!-- markdownlint-enable MD026 -->

Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.

## <a name="common-throttling-scenarios"></a>Cenários comuns de limitação

As causas mais comuns de limitação dos clientes incluem:

- Um grande número de solicitações em todos os aplicativos em um locatário.
- Um grande número de solicitações de um aplicativo específico entre todos os locatários.

## <a name="best-practices-to-handle-throttling"></a>Práticas recomendadas para lidar com a limitação

Estas são as práticas recomendadas para lidar com a limitação:

- Reduza o número de operações por solicitação.
- Reduza a frequência de chamadas.
- Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.

Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.

1. Aguarde o número de segundos especificado no cabeçalho `Retry-After`.
2. Repita a solicitação.
3. Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.

Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:

- [Usuário](/graph/api/resources/user?view=graph-rest-1.0)
- [Foto](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [Email](/graph/api/resources/message?view=graph-rest-1.0)
- [Calendário (usuários e grupos)](/graph/api/resources/event?view=graph-rest-1.0)
- [Contato](/graph/api/resources/contact?view=graph-rest-1.0)
- [Anexo](/graph/api/resources/attachment?view=graph-rest-1.0)
- [Conversas em grupo](/graph/api/resources/conversation?view=graph-rest-1.0)
- [Pessoas e social](/graph/api/resources/social-overview?view=graph-rest-beta)
- [Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)
- [Item externo (Pesquisa da Microsoft)](/graph/api/resources/externalitem?view=graph-rest-beta)

Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).

> [!NOTE]
> Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada. Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.
>
> Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.

## <a name="service-specific-limits"></a>Limites específicos do serviço

O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory. Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.

> [!NOTE]
> Os limites específicos descritos aqui estão sujeitos a alterações.

### <a name="outlook-service-limits"></a>Limites de serviço do Outlook

Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio. Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo). Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio.

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | Ponto de extremidade Beta   |
| carregamento de 15 megabits (PATCH, POST, PUT) em um período de 30 segundos | Ponto de extremidade Beta   |

#### <a name="outlook-service-resources"></a>Recursos de serviço do Outlook

Os recursos a seguir são fornecidos pelo serviço do Outlook.

##### <a name="calendar-api-resources"></a>Recursos da API do calendário

- [event](/graph/api/resources/event)
- [eventMessage](/graph/api/resources/eventmessage)
- [calendar](/graph/api/resources/calendar)
- [calendarGroup](/graph/api/resources/calendargroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)
- [place (preview)](/graph/api/resources/place)

##### <a name="mail-api-resources"></a>Recursos da API do email

- [message](/graph/api/resources/message)
- [mailFolder](/graph/api/resources/mailfolder)
- [mailSearchFolder](/graph/api/resources/mailsearchfolder)
- [messageRule](/graph/api/resources/messagerule)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a>Recursos da API de contatos pessoais

- [contato](/graph/api/resources/contact)
- [contactFolder](/graph/api/resources/contactfolder)
- [outlookCategory](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a>Recursos da inteligência social e do local de trabalho 

- [person](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a>Recursos da API de tarefas pendentes (visualização)

- [outlookTask](/graph/api/resources/outlooktask)
- [outlookTaskFolder](/graph/api/resources/outlooktaskfolder)
- [outlookTaskGroup](/graph/api/resources/outlooktaskgroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a>Limites do serviço do Microsoft Teams

Os limites são expressos como solicitações por segundo (rps).

| Tipo de solicitação do Teams                                   | Limitar por aplicativo por locatário        | Limitar por aplicativo em todos os locatários      |
|------------------------------------------------------|---------------------------------|------------|
| Todas as chamadas de API do Graph para o Microsoft Teams              | 15000 solicitações a cada 10 segundos | n/d |
| OBTER equipe, canal, guia, installedApps, appCatalogs   | 60 rps                          | 600 rps |
| Canal POST/PUT, guia, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH da equipe, canal, guia, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| EXCLUIR canal, Tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| OBTER /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone | 6 rps | 150 rps  | 
| OBTER mensagem do canal  | 5 rps | 100 rps |
| OBTER 1:1/mensagem de chat do grupo  | 3 rps | 30 rps |
| POSTAR mensagem do canal | 2 rps | 20 rps |
| POSTAR 1:1/mensagem de chat do grupo | 2 rps | 20 rps |

É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.

Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).
