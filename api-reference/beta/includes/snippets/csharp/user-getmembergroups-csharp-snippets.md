---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcb3eb3e251157ab20d2caf5e16cbe0006be6868
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```