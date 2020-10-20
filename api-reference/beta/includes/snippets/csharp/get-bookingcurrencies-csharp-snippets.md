---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f87676202a9f30865c6ceb413cf0e23c445e8f4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrencies = await graphClient.BookingCurrencies
    .Request()
    .GetAsync();

```