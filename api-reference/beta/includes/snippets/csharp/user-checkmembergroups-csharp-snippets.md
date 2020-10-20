---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1a9ac5158187a4cd717d17ee85123a0702e29bb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Me
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```