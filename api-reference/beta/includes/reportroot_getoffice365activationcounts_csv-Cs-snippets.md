---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d97a7e041480ae2737043cddf2c6b559f3b69572
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationCounts = await graphClient.Reports.GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```