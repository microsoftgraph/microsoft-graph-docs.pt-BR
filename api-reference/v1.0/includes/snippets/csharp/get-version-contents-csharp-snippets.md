---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfce8c8b8faf76c140cfcd3fb9550de5e4769429686f87a8d4d79b458ec8d921
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions["{driveItemVersion-id}"].Content
    .Request()
    .GetAsync();

```