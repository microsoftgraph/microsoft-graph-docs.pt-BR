---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db5c34a56da98ef9f77cd6cd3c72f1b356c0682e
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    EndpointType = EndpointType.Default,
    Identity = new IdentitySet
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"phone", "{\"@odata.type\":\"#microsoft.graph.identity\",\"id\":\"+12345678901\"}"}
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"languageId", "languageId-value"},
        {"region", "region-value"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,null)
    .Request()
    .PostAsync();

```