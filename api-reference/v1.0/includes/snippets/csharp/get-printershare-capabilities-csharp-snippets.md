---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 982a35bc034b791f07999e2b0fd3c785747fc691
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771642"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .Select("id,displayName,capabilities")
    .GetAsync();

```