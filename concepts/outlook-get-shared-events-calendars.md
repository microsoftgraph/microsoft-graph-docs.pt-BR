---
title: Obter eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 773d996e8343c69028a7cbbe8a1a4283f5470108
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981382"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>Obter eventos do Outlook em um calendário compartilhado ou delegado

No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.

O Microsoft Graph oferece suporte de forma programática para colocar eventos em calendários que foram compartilhadas por outros usuários, além de receber os calendários compartilhadas propriamente ditos. O suporte também se aplica a calendários que foram delegados.

Por exemplo, Henrique compartilhou com Diogo seu calendário padrão e deu a ele acesso de leitura. Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o aplicativo poderá acessar o calendário padrão de Henrique e os eventos nesse calendário, conforme descrito abaixo.

> **Observação** permissões de compartilhamento (Calendars.Read.Shared ou Calendars.ReadWrite.Shared) permitem a você ler ou escrever eventos em um calendário compartilhado ou representante. Eles não têm suporte [subscrever para alterar notificações](webhooks.md) em itens como pastas. Para configurar as assinaturas de notificação de alteração em eventos em um usuário compartilhado, representante ou qualquer outro usuário ou calendário de recursos no locatário, use a permissão de aplicativo Calendars.Read.

## <a name="get-an-event-in-the-shared-calendar"></a>Obter um evento no calendário compartilhado

Você pode obter um evento específico no calendário padrão compartilhado de Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificada por `{id}` do calendário padrão de Henrique.

## <a name="get-all-the-events-in-the-shared-calendar"></a>Obter todos os eventos no calendário compartilhado

Obtenha todos os eventos no calendário padrão que Henrique compartilhou com Diogo:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) no calendário padrão de Henrique.

## <a name="get-the-shared-calendar"></a>Obter o calendário compartilhado

Obtenha o calendário padrão que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa a pasta padrão de Henrique.

Os mesmos recursos de GET se aplicarão se Henrique delegar a Diogo mais acesso ao seu calendário padrão ou se Henrique delegar toda a sua caixa de correio a Diogo.

Se Henrique não tiver compartilhado seu calendário padrão com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que se integrar com o calendário do Outlook](outlook-calendar-concept-overview.md)
- A [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.
