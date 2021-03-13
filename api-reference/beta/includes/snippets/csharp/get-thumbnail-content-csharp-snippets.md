---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a645f709ee82a038d0307bd25f0d82cebc60f7dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails["{thumbnailSet-id}"]["{thumbnailSet-id}"].Content
    .Request()
    .GetAsync();

```