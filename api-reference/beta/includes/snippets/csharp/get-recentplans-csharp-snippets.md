---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 935fd344851b9ccdc0f8854402433155f7103029301cf448f859455c88b64ec6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recentPlans = await graphClient.Me.Planner.RecentPlans
    .Request()
    .GetAsync();

```