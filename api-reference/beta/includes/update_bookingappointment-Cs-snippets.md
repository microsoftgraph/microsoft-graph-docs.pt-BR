---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f89a916c3ade122cd0de532f2aa4b407155b2fa2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = new BookingAppointment
{
    End = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    InvoiceDate = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:00:00+03:00",
        TimeZone = "UTC"
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .UpdateAsync(bookingAppointment);

```