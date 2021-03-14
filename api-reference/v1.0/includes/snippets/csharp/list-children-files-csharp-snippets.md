---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de09ba4912210a14a8ade96a1158f20eb9ef67d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Children
    .Request()
    .GetAsync();

```