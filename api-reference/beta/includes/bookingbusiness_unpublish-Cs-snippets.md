---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4f29f103d61257b85331925e8799d80c44f70a3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"]
    .Unpublish(bookingBusiness)
    .Request()
    .PostAsync();

```