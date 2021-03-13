---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d386ecd96daad06f754cb08f139865268b2027d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .DeleteAsync();

```