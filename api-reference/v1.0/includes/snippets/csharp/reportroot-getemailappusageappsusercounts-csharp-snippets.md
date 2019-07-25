---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0909aba727aade187f3623bfabdfc82e917525bb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageAppsUserCounts('D7')
    .Request()
    .GetAsync();

```