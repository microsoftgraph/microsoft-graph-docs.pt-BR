---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 415eebc06fdcade6596b07a8a636d99ae4a326e3
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .GetAsync();

```