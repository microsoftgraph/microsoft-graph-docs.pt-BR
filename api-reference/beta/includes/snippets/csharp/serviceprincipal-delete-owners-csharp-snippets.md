---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 11c14dbaaaa281485c73c516047ee922dfd2fd41
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```