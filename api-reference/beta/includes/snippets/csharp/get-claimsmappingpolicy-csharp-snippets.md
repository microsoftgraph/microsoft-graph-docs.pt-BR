---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0882349acf1dd0dc0edc366f7a362286b4441e9b
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {id} = await graphClient.Policies["claimsMappingPolicies"].{id}
    .Request()
    .GetAsync();

```