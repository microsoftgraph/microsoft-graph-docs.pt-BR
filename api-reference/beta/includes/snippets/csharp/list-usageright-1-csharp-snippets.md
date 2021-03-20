---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 603c65d33027ed803912d034d87257cdd0aeca02
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Devices["{device-id}"].UsageRights
    .Request()
    .GetAsync();

```