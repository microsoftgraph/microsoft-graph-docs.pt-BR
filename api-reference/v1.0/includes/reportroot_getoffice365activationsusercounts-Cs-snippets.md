---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b851ba91848442bf8c866b9d1a9720d86467848c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationsUserCounts()
    .Request()
    .GetAsync();

```