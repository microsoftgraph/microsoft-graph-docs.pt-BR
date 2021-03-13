---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bad233821abd0317c5451927ad75365b1d6b68cf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```