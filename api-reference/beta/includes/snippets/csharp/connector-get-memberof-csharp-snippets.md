---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afe67f3eb04fca47edb4e7e2200577a9783578ebd86faf4213d587ac335e37ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"].MemberOf
    .Request()
    .GetAsync();

```