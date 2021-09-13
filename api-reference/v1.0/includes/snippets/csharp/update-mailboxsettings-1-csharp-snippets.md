---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a372d0daa4f372d4a2dca4e8900717f00d923af468aef09c0792996eb3c3174d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    AutomaticRepliesSetting = new AutomaticRepliesSetting
    {
        Status = AutomaticRepliesStatus.Scheduled,
        ScheduledStartDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-20T18:00:00",
            TimeZone = "UTC"
        },
        ScheduledEndDateTime = new DateTimeTimeZone
        {
            DateTime = "2016-03-28T18:00:00",
            TimeZone = "UTC"
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.context", "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings"}
    }
};

var me = new User();
me.MailboxSettings = mailboxSettings;

await graphClient.Me
    .Request()
    .UpdateAsync(me);

```