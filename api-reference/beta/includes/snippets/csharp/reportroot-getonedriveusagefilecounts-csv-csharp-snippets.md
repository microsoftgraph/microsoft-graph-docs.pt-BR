---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f279d578571493d06427bfcec24ac92355b2e376
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageFileCounts = await graphClient.Reports
    .GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```