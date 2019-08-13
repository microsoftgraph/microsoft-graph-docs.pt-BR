---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12677c65d969777b28419429111f530f8152eb0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```