---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 817b9f0b330e6f269beffaa94c4492309f637614
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="]
    .Request()
    .GetAsync();

```