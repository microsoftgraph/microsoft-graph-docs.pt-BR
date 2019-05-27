---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcb3eb3e251157ab20d2caf5e16cbe0006be6868
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```