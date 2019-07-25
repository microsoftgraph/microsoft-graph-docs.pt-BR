---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0457003c8b827c5bf342672c3f2d058d45da70c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .DeleteAsync();

```