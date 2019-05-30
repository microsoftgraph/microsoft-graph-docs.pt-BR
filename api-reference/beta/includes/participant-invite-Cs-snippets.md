---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1aec6d469d0ab2d16317ade124d9c9bb20b8cbe
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        EndpointType = EndpointType.Default,
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "550fae72-d251-43ec-868c-373732c2704f",
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47",
                DisplayName = "Heidi Steen"
            }
        },
        LanguageId = "languageId-value",
        Region = "region-value",
        ReplacesCallId = "replacesCallId-value"
    }
};

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"].Participants
    .Invite(participants,clientContext)
    .Request()
    .PostAsync();

```