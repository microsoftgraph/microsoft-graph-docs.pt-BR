---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 882b12801c8620502112fe6bf6842743475a24316ee27625ab700c04205b7a4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getActivitiesByInterval = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .GetActivitiesByInterval("2017-01-01","2017-01-3","day")
    .Request()
    .GetAsync();

```