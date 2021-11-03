---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 167740105d8c05022afcee9bed7df7511123c996fc5f2df3292551e4c97461df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Joni Sherman",
    EmailAddress = "jonis@relecloud.com"
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers
    .Request()
    .AddAsync(bookingCustomer);

```