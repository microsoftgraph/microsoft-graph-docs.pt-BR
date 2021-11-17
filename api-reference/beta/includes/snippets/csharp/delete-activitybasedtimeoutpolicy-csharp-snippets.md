---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14c024f30d05b1bdb1afd3df5ebea992678c22153f58cd3b399b63021deb4053
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ActivityBasedTimeoutPolicies["{activityBasedTimeoutPolicy-id}"]
    .Request()
    .DeleteAsync();

```