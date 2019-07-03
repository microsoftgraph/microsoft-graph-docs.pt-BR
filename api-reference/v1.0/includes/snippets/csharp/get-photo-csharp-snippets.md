---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eac7b203c4b6194a37202b1f709aa94416b60777
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profilePhoto = await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .GetAsync();

```