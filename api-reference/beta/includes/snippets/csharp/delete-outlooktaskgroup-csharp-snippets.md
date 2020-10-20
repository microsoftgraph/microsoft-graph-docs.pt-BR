---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc285be1e93b144b5752f7bd56b32d63e1a271d7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="]
    .Request()
    .DeleteAsync();

```