---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 428edfd9ac6ee33305cea3a39833e9a9cd1da61e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageVersionsUserCounts("D7")
    .Request()
    .GetAsync();

```