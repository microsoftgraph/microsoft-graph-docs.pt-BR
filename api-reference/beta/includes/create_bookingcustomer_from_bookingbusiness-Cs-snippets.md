---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45e75108b950ad2fb5c6763fe17fef8e84e2fe8f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Joni Sherman",
    EmailAddress = "jonis@relecloud.com"
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers
    .Request()
    .AddAsync(bookingCustomer);

```