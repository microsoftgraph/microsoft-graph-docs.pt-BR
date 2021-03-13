---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edda8db92d30cf8a4c68f453abba8859f4ce5364
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHold = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"]
    .Request()
    .GetAsync();

```