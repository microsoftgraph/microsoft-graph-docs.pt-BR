---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8b6dfdc39a4eeb5fa1c728bdc6ac0dceb647150
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageVersionsUserCounts = await graphClient.Reports
    .GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```