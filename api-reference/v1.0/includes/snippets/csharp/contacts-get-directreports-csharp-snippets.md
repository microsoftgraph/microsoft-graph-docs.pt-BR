---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 958ab1606c2a1766aee6f314e3ac22d8a2dad19c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Contacts["{id}"].DirectReports
    .Request()
    .GetAsync();

```