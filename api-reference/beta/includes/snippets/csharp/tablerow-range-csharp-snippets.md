---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2e59acf6fbdb2a97d76df1b2e8a5a3ab05ff8df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Range()
    .Request()
    .GetAsync();

```