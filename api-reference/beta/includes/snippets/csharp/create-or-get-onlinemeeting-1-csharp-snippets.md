---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c5d61682b5096753cc17d9a6657031f91af0da471bca369a121cb7e327bee74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var startDateTime = DateTimeOffset.Parse("2020-02-06T01:49:21.3524945+00:00");

var endDateTime = DateTimeOffset.Parse("2020-02-06T02:19:21.3524945+00:00");

var subject = "Create a meeting with customId provided";

var externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";

var participants = new MeetingParticipants
{
    Attendees = new List<MeetingParticipantInfo>()
    {
        new MeetingParticipantInfo
        {
            Identity = new IdentitySet
            {
                User = new Identity
                {
                    Id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                }
            },
            Role = OnlineMeetingRole.Presenter,
            Upn = "test1@contoso.com"
        }
    }
};

await graphClient.Me.OnlineMeetings
    .CreateOrGet(externalId,null,endDateTime,participants,startDateTime,subject)
    .Request()
    .PostAsync();

```