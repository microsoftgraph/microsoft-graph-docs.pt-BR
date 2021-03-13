---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28e84cc2bad4317f6e562a94ae724d31c2fe67d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook
    .CreateSession(persistChanges)
    .Request()
    .PostAsync();

```