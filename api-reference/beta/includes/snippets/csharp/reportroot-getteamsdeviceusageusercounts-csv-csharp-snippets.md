---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30c36e5ff6d0f2f60ce799de0cf6584ea51a2abc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserCounts = await graphClient.Reports
    .GetTeamsDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```