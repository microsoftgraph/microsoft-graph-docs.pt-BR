---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77c76b300817676a4ca86bca45f1c4fb6d7291033305ed6e32e28f82c062de77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationFeatureSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByFeature(IncludedUserTypes.All,IncludedUserRoles.All)
    .Request()
    .GetAsync();

```