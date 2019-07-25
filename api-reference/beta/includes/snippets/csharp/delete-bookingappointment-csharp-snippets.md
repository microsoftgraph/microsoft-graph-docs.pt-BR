---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12983dc99f7cb5cf592291fead02d5f853824f96
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKqAAA="]
    .Request()
    .DeleteAsync();

```