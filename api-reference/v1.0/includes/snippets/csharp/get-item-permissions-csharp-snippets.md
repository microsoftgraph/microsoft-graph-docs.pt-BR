---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73b500bda59a884fcfd23f4712310c4faf2c3dca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions
    .Request()
    .GetAsync();

```