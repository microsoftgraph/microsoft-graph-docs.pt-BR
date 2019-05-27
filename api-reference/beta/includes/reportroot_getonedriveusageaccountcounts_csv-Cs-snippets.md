---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64cdbe5dd19d706c570639e4bcfbe96d67a6633b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountCounts = await graphClient.Reports.GetOneDriveUsageAccountCounts('D7')
    .Request()
    .GetAsync();

```