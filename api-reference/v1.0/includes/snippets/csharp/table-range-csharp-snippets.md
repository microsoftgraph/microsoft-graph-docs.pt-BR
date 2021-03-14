---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53180cb0156420822fa185eb0da1ac558dd05ce5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Range()
    .Request()
    .GetAsync();

```