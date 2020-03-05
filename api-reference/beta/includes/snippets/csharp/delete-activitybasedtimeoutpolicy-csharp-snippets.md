---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4e5625b97bddf075903780e98fe34d76d187c07
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies["activityBasedTimeoutPolicies"].{id}
    .Request()
    .DeleteAsync();

```