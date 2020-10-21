---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da0ac949daf734cac5f1a82d85e5b77bd736f0a8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{id}"]
    .Request()
    .UpdateAsync(mailFolder);

```