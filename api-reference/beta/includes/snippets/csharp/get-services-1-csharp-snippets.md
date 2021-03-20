---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db815b14d5f8bb7b0979aeda7d39ae9f1954506e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services
    .Request()
    .GetAsync();

```