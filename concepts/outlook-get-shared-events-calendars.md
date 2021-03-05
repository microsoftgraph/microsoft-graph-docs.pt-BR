---
title: Obter calendário do Outlook compartilhado ou delegado e seus eventos
description: No Outlook, um proprietário de calendário pode compartilhar um calendário com outros usuários e deixá-los exibir ou modificar eventos nesse calendário. o calendário pode ser um calendário personalizado ou o calendário principal. O proprietário também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário da conta de email.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 06e11f11b9c25e3392075e027278558d1330d51e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470071"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a>Obter calendário do Outlook compartilhado ou delegado e seus eventos

No Outlook, um proprietário de calendário pode compartilhar um calendário com outros usuários e deixá-los exibir ou modificar eventos nesse calendário. o calendário compartilhado pode ser um calendário personalizado ou o calendário principal do proprietário, criado por ele.. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.

Programaticamente, o Microsoft Graph oferece suporte à leitura e à criação de eventos em calendários que foram compartilhadas por outros usuários, além de leitura de calendários compartilhados e atualização do nome do calendário para compartilhamento. O suporte também se aplica a calendários que foram delegados. O restante deste artigo descreve a leitura de eventos em um calendário compartilhado ou delegado. Para obter eventos, consulte[Obter eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md).

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a>Compartilhamento: Obtenha um calendário compartilhado ou seus eventos diretamente da caixa de correio do proprietário do calendário

Os três exemplos a seguir usam esse cenário: no Outlook, Alex compartilhou seu calendário principal com Sara e recebeu de Sara permissões de leitura. Se Sara entrar no aplicativo e oferecer _permissões delegadas_ (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), em nome de Sara, seu aplicativo poderá acessar o calendário principal e seus eventos diretamente da caixa de correio.

Os três exemplos especificam a identidade do proprietário (Alex ' ID de usuário ou nome de usuário do usuário) e o atalho `calendar`. Eles acessam o calendário e as IDs de eventos que correspondem somente à caixa de correio do proprietário. Especificar esses IDs de eventos e calendários na caixa de correio do compartilhamento (ID de usuário de Sara ou nome de usuário principal) retornaria um erro. Para usar o calendário e as IDs de eventos que correspondem à caixa de correio do compartilhamento, confira [compartilhar: Obtenha calendário personalizado, compartilhado ou seus eventos na caixa de correio do compartilhamento](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox). 

> **Observação** permissões de compartilhamento (Calendars.Read.Shared ou Calendars.ReadWrite.Shared) permitem a você ler ou escrever eventos em um calendário compartilhado ou representante. Eles não têm suporte [subscrever para alterar notificações](webhooks.md) em itens como pastas. Para configurar as assinaturas de notificação de alteração em eventos em um usuário compartilhado, representante ou qualquer outro usuário ou calendário de recursos no locatário, use a permissão de aplicativo Calendars.Read.

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Sara: Obtenha o calendário principal compartilhado diretamente da caixa de correio de Alex

Conectado como Sara, obtenha o calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa calendário compartilhado, principal, na caixa de correio de Alex.

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Sara: Obtenha o calendário principal compartilhado diretamente a partir da caixa de correio de Alex

Conectado como Sara, seu aplicativo pode obter um evento específico no calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificada por `{id}` do calendário principal de Alex, diretamente da caixa de correio de Alex.

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a>Sara: Obtenha todos os eventos no calendário principal compartilhado da caixa de correio de Alex

Conectado como Sara, obtenha todos os eventos no calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção das instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) do calendário principal de Alex, diretamente da caixa de correio de Alex.

Os mesmos recursos GET se aplicam se a Alex tiver delegado o acesso a Sara ao calendário principal de Alex, ou se Alex tiver delegado a Sara a sua caixa de correio inteira.

Se Alex não tiver compartilhado nem delegado o seu calendário principal com Sara, especificar a ID de usuário ou o nome de usuário da Alex nas operações de obter retornará um erro. 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a>Compartilhamento: Obtenha calendário personalizado, compartilhado ou seus eventos da caixa de correio do compartilhamento

Se Alex compartilhou um _calendário_ personalizado (por exemplo, um calendário chamado "festas de crianças") com Adele e Adele tiver fornecido permissões delegadas (Calendars.Read ou Calendars.ReadWrite), seu aplicativo poderá obter os eventos ou o calendário do calendário da cópia local do Alex ", na caixa de email de Adele, conforme descrito abaixo.

1. Conectado como Adele, use uma das seguintes solicitações para obter todos os calendários aos quais Adele tem acesso, incluindo o calendário personalizado compartilhado.

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    Uma resposta bem-sucedida inclui o código de resposta HTTP 200 e o conjunto de calendários que Adele tem acesso, incluindo o calendário ("festas das crianças") com o nome do proprietário como "Alex Rodrigues" como o segundo calendário na resposta. Para um compartilhamento, Adele, a propriedade **canShare** do calendário compartilhado é sempre falsa.

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
      "truncated": true,
      "@odata.type": "microsoft.graph.calendar",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json

    {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
        "value": [
            {
                "id": "AQMkADU5NAAAJMjAAAAA==",
                "name": "Calendar",
                "color": "auto",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
                "canShare": true,
                "canViewPrivateItems": true,
                "canEdit": true,
                "owner": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            {
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. Conectado como Adele, obtenha o calendário compartilhado ou obtenha um ou mais eventos no calendário compartilhado usando a segunda ID de calendário na resposta da etapa 1. As IDs do calendário compartilhado e seu evento correspondem à cópia local do calendário de Alex na caixa de correio de Adele.

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e o evento, os eventos ou o calendário solicitado que Alex compartilhou com Adele.


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Criar eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md)
- [Compartilhar ou delegar um calendário no Outlook (visualização)](outlook-share-or-delegate-calendar.md)
- [Por que se integrar com o calendário do Outlook](outlook-calendar-concept-overview.md)
- A [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.
