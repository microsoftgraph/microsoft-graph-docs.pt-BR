---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1e15fbafdd9333a90e6a87ade138a129b984ea3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Cell(5,6)
    .Request()
    .GetAsync();

```