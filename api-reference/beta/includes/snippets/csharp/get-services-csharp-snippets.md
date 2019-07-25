---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eddd7a382e153d49959b887fc8bb99fb49cf3363
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Services
    .Request()
    .GetAsync();

```