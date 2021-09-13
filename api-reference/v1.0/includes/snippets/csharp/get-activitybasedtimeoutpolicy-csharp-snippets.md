---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c726b42bc93bcb16ca46f95d08b217c91f2d5974b8b9538628a9ef354ca1bcc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = await graphClient.Policies.ActivityBasedTimeoutPolicies["{activityBasedTimeoutPolicy-id}"]
    .Request()
    .GetAsync();

```