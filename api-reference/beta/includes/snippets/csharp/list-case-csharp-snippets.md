---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90fda57b2ca3bf40b2eb31104e61d01bb1e38263
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cases = await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .GetAsync();

```