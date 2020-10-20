---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4fd29caed863a2f9fff82ac0c5d9038d21da1a40
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Services["57da6774-a087-4d69-b0e6-6fb82c339976"]
    .Request()
    .GetAsync();

```