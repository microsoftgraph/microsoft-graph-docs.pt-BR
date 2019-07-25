---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f9dd8fd7656738c63b2c2c2afef4fec3ac43960
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","microsoft.graph.mailSearchFolder"}
    },
    DisplayName = "Weekly digests",
    IncludeNestedFolders = true,
    SourceFolderIds = new List<String>()
    {
        "AQMkADYAAAIBDAAAAA=="
    },
    FilterQuery = "contains(subject, 'weekly digest')"
};

await graphClient.Me.MailFolders["AQMkADYAAAIBDAAAAA=="].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```