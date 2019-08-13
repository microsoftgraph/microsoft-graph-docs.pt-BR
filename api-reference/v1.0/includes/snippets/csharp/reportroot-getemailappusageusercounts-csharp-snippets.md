---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 823b4bc2f2251ced705e5ab674da3637ec95c17a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageUserCounts("D7")
    .Request()
    .GetAsync();

```