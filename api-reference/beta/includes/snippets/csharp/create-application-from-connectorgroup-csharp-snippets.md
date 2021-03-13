---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74d469a3dd8b844e7d335f5fd99a84f98a8fe608
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ConnectorGroup.Reference
    .Request()
    .PutAsync("{id}");

```