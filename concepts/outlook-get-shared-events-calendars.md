---
title: Obtenha os eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permita que eles exibir ou modificar os eventos nesse calendário. Os clientes também podem conceder a um representante para agir em nome deles, para receber ou responder às solicitações de reunião, ou criar ou alterar itens do calendário.
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091617"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>Obtenha os eventos do Outlook em um calendário compartilhado ou delegado

No Outlook, os clientes podem compartilhar um calendário com outros usuários e permita que eles exibir ou modificar os eventos nesse calendário. Os clientes também podem conceder a um representante para agir em nome deles, para receber ou responder às solicitações de reunião, ou criar ou alterar itens do calendário.

Programaticamente, oferece suporte ao Microsoft Graph obtendo eventos no calendários que foram compartilhados por outros usuários, bem como obtendo o compartilhado calendários sozinhos. O suporte também se aplica a calendários que foram delegados.

Por exemplo, Garth tem compartilhadas com John seu calendário padrão e oferecido acesso de leitura de John. Se John tiver entrado no seu aplicativo e oferecido permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o seu aplicativo será capaz de acessar o calendário padrão e os eventos do Garth nesse calendário conforme descrito abaixo.

## <a name="get-an-event-in-the-shared-calendar"></a>Obtenha um evento no calendário compartilhado

Você pode obter um evento específico no calendário do Garth padrão compartilhada:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificado pela `{id}` de calendário do Garth padrão.

## <a name="get-all-the-events-in-the-shared-calendar"></a>Obtenha todos os eventos no calendário compartilhado

Obtenha todos os eventos no calendário padrão que Garth compartilhada com John:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e um conjunto de instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) no calendário de padrão do Garth.

## <a name="get-the-shared-calendar"></a>Obtenha o calendário compartilhado

Obtenha o calendário padrão que Garth compartilhada com John.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa a pasta de padrão do Garth.

Os mesmos recursos GET aplicam se Garth tinha John mais acesso delegado a calendário de padrão do Garth ou se Garth tinha delegada John sua caixa de correio inteira.

Se Garth não compartilhou seu calendário padrão com John, nem ele tem delegado sua caixa de correio de John, a especificação user ID do Garth ou o nome principal do usuário nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que a integração com o calendário do Outlook](outlook-calendar-concept-overview.md)
- A [API do calendário](/graph/api/resources/calendar?view=graph-rest-1.0) na versão 1.0 do Microsoft Graph.