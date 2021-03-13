---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00101da8272bd5f3adb960ec86690f39b910f980
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails["{thumbnailSet-id}"]["{thumbnailSet-id}"]
    .Request()
    .GetAsync();

```