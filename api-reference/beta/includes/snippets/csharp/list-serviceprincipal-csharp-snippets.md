---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: ef8b711a2f7bee18c4d2c1c4a0eda0cd94c77477
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .GetAsync();

```