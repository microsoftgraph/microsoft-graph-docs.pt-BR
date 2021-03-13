---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 693bb6ecdc4477a86b91980154821d940a8330af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services["{bookingService-id}"]
    .Request()
    .DeleteAsync();

```