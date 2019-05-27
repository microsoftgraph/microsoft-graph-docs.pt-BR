---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a918586b0cb62135430dabd89766a665f154723d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "84b80893-8749-40a3-97b7-68513b600544",
    "5d6059b6-368d-45f8-91e1-8e07d485f1d0"
};

var types = new List<String>()
{
    "user"
};

await graphClient.DirectoryObjects
    .GetByIds(ids,types)
    .Request()
    .PostAsync();

```