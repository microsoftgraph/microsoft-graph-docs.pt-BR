---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c42167aca00ad80b5ae7cb2dc56e9b6389cc351bbd236a53b63c5e2377384b1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Rosters["{plannerRoster-id}"].Members["{plannerRosterMember-id}"]
    .Request()
    .DeleteAsync();

```