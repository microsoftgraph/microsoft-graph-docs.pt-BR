---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60d7898b91836f808f5cfb5dc57d77393b8b60a36401b6abb186ed5c5aa16837
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.HomeRealmDiscoveryPolicies["{homeRealmDiscoveryPolicy-id}"].AppliesTo
    .Request()
    .GetAsync();

```