---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cddcbe5e6b922d9a51beb82f016905ff13682928baa2c97b9f28d886dd50b346
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Members
    .Request()
    .Filter("roles/any(r:r eq 'owner')")
    .GetAsync();

```