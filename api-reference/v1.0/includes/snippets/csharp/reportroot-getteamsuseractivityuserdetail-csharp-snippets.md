---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62c97697177b491d29fcc588bc8352e98342c539
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886625"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityUserDetail('D7')
    .Request()
    .GetAsync();

```