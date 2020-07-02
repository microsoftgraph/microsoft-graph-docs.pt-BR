---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 023577eee33e9fa8e8702a49c156723efec01aab
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var followedSites = await graphClient.Me.FollowedSites
    .Request()
    .GetAsync();

```