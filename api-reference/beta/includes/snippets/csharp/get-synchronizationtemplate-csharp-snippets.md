---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 957b0e8db1a6c2094b3b51b04bd043cee6f15d56
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var templates = await graphClient.ServicePrincipals["{id}"].Synchronization.Templates
    .Request()
    .GetAsync();

```