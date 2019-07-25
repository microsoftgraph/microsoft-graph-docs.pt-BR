---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5669fc602f905dda8d5fda80a7efe4a5f3872aa6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
    .Publish(bookingBusiness)
    .Request()
    .PostAsync();

```