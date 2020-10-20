---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92b10428b2e42c1cd6c992ae9d13c5c05a3777e2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Charity work"
};

await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAhrbPWAAA="]
    .Request()
    .UpdateAsync(outlookTaskFolder);

```