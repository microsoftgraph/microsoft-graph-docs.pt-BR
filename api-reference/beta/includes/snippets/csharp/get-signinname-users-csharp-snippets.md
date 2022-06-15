---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7959d5b304f07ea5b6929a45f88d24005c48d5a9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'My B2C tenant')")
    .Select("displayName,id")
    .GetAsync();

```