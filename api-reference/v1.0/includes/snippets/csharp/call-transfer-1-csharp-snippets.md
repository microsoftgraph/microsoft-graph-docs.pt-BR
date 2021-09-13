---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6f1af9c5f6c542c7cff2b7c2041783a3dd6f0993d912841cb77b1acb61380e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215303"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "550fae72-d251-43ec-868c-373732c2704f",
            DisplayName = "Heidi Steen"
        }
    },
    ReplacesCallId = "replacesCallId-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"endpointType", "default"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget)
    .Request()
    .PostAsync();

```