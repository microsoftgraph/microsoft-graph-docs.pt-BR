---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfcdf0f03ada674e169315da651e80e5ca10a938
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .Request()
    .GetAsync();

```