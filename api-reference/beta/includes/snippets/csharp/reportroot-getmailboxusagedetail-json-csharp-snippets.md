---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f551142a6f8293d893fda0940d1424634edf0e36
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageDetail = await graphClient.Reports
    .GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```