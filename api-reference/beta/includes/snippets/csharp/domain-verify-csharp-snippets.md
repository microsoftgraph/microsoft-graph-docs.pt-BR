---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1894850b69cc416e50f0c66afaae6de56989a71
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["contoso.com"]
    .Verify()
    .Request()
    .PostAsync();

```