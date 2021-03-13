---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 103f7b044ca486ad10072be9d4d25d76128064d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customers = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers
    .Request()
    .GetAsync();

```