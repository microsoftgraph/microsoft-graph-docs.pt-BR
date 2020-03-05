---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d09f279f79bac5c6adaae7da89bb12d8cf05ba7c
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {id} = await graphClient.Policies["homeRealmDiscoveryPolicies"].{id}
    .Request()
    .GetAsync();

```