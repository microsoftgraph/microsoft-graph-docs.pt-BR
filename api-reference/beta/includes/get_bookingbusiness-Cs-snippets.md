---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 697cb5463720e7d604110d9d9ce3f357f17b8b29
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473803"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = await graphClient.BookingBusinesses["Fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .GetAsync();

```