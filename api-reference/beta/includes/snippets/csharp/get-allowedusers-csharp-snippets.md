---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2febd0d93350c4e8ce888b0ec278299304ec0e72
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedUsers = await graphClient.Print.Shares["{id}"].AllowedUsers
    .Request()
    .GetAsync();

```