---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 973ae496dbd05a8b64e42e4b11fceedc0ecc261d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Subject = "Let's go for lunch",
    Body = new ItemBody
    {
        ContentType = BodyType.Html,
        Content = "Does late morning work for you?"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2019-06-16T12:00:00",
        TimeZone = "Pacific Standard Time"
    },
    End = new DateTimeTimeZone
    {
        DateTime = "2019-06-16T14:00:00",
        TimeZone = "Pacific Standard Time"
    },
    Location = new Location
    {
        DisplayName = "Harry's Bar"
    },
    Attendees = new List<Attendee>()
    {
        new Attendee
        {
            EmailAddress = new EmailAddress
            {
                Address = "adelev@contoso.onmicrosoft.com",
                Name = "Adele Vance"
            },
            Type = AttendeeType.Required
        }
    }
};

await graphClient.Groups["01d4ee64-15ce-491e-bad1-b91aa3223df4"].Events
    .Request()
    .AddAsync(@event);

```