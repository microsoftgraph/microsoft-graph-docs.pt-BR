---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18e996ebb80dc597af8390fb056ba9c0e44ece9adff25d7b6f8ba3f0529c2943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group assignable to a role",
    DisplayName = "Role assignable group",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    IsAssignableToRole = true,
    MailEnabled = true,
    SecurityEnabled = true,
    MailNickname = "contosohelpdeskadministrators",
    Visibility = "Private"
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```