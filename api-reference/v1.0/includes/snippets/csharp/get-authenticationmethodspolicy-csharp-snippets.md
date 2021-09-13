---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9a9dbc1c12e3193dfdb47686d36aef70d4044b87867af49ee23313467105395
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodsPolicy = await graphClient.Policies.AuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```