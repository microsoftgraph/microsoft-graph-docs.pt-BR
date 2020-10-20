---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a47e3912a9654cf08a5a6f0e3f39e228183f1b9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrency = await graphClient.BookingCurrencies["USD"]
    .Request()
    .GetAsync();

```