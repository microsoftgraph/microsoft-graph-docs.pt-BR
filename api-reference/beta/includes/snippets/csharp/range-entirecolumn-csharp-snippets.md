---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63790024a45aebb9246bcd2d525f26137a16cfd2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .EntireColumn()
    .Request()
    .GetAsync();

```