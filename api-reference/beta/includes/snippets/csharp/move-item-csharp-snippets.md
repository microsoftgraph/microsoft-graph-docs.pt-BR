---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0eba89a2362976ae52c64736432e8da219e3c977
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    ParentReference = new ItemReference
    {
        Id = "new-parent-folder-id"
    },
    Name = "new-item-name.txt"
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```