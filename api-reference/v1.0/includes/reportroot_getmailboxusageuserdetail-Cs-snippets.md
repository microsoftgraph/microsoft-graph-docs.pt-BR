---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 940d4ba5eaf3384db2bb175f64512ada74338bd7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463393"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```