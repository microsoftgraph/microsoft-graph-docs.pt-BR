---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0457003c8b827c5bf342672c3f2d058d45da70c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .DeleteAsync();

```