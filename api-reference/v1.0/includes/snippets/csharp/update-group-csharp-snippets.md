---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28b520823156e20101ca2714a37078014760f34f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Library Assist",
    DisplayName = "Library Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "library-help"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```