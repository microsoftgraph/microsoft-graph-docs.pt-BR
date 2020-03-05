---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 991d265068774da19de0b6590262e56413c9d6ca
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.ServicePrincipals["{id}"].HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```