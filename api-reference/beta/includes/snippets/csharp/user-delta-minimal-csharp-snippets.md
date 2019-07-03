---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3235e68f041adbf09c3b3c2b082b60138a2bf384
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users.Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.MobilePhone 
             })
    .GetAsync();

```