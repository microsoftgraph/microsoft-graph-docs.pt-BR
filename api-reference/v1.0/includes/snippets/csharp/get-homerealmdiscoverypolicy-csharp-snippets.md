---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5446c858aa65b44a5c8191ba0a7e0c34942e1ad2e37bb5b7e20eb13515c7c7f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = await graphClient.Policies.HomeRealmDiscoveryPolicies["{homeRealmDiscoveryPolicy-id}"]
    .Request()
    .GetAsync();

```