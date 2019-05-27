---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 351f13b9ecfb7412fbbbb6473edb1ac324b8142c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454310"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```