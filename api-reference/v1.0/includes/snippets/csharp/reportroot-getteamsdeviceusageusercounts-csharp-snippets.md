---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4452e14ae02393ed7e6d52d8e5ac7803f27aad10
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```