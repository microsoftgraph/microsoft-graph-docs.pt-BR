---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37e6ba6d3336868c1ed32d640b199116b68b1c00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .EntireRow()
    .Request()
    .GetAsync();

```