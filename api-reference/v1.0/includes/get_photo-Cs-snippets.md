---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eac7b203c4b6194a37202b1f709aa94416b60777
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profilePhoto = await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .GetAsync();

```