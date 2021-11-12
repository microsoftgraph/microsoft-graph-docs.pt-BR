---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76dd641aaaeb1d2657eb0405cab70a964bf3d83efad7d57286a3cca5df53c0c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214170"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Groups["{group-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```