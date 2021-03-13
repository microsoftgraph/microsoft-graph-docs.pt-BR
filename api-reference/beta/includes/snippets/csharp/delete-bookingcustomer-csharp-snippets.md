---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1988edadb2b328b47f80ae4d9d3ce830eceffe2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers["{bookingCustomer-id}"]
    .Request()
    .DeleteAsync();

```