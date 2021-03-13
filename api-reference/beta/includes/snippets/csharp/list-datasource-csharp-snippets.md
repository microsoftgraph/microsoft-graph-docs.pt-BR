---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8daab269a0dde592549f74eee69b215a2369345e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769606"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodianSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"].CustodianSources
    .Request()
    .GetAsync();

```