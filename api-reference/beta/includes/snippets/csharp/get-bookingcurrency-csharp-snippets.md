---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ff81773c48e482cad55460d791009d09ac34e3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796612"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrency = await graphClient.BookingCurrencies["{bookingCurrency-id}"]
    .Request()
    .GetAsync();

```