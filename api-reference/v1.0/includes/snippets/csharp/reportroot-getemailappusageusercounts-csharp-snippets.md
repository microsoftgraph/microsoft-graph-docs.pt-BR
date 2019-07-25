---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8b8ca994940a3841fafd068f6f0c0cd00ca05bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886372"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```