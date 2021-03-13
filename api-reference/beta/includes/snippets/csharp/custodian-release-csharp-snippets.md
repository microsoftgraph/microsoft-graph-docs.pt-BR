---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7ed818892ef89b83b7e323e4c06f5585813b2ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"]
    .Release()
    .Request()
    .PostAsync();

```