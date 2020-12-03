---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff660dac5b40357d0ba8dab30befd5b9ed71137a
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    CallbackUri = "https://bot.contoso.com/callback",
    Source = new ParticipantInfo
    {
        Identity = new IdentitySet
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"applicationInstance", "{\"@odata.type\":\"#microsoft.graph.identity\",\"displayName\":\"Calling Bot\",\"id\":\"3d913abb-aec0-4964-8fa6-3c6850c4f278\"}"}
            }
        },
        CountryCode = null,
        EndpointType = null,
        Region = null,
        LanguageId = null
    },
    Targets = new List<InvitationParticipantInfo>()
    {
        new InvitationParticipantInfo
        {
            Identity = new IdentitySet
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"phone", "{\"@odata.type\":\"#microsoft.graph.identity\",\"id\":\"+12345678901\"}"}
                }
            }
        }
    },
    RequestedModalities = new List<Modality>()
    {
        Modality.Audio
    },
    MediaConfig = new AppHostedMediaConfig
    {
        Blob = "<Media Session Configuration>"
    }
};

await graphClient.Communications.Calls
    .Request()
    .AddAsync(call);

```