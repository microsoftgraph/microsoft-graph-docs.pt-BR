---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a12d58a26bbbabaa9a3d2470068efb37569eb75
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CreateSession(this,persistChanges)
    .Request()
    .PostAsync();

```