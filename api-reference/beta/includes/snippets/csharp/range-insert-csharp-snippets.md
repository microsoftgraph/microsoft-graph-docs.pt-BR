---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d81afd04004d677d34ce55eda01b3f13d9925eb4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Insert(shift)
    .Request()
    .PostAsync();

```