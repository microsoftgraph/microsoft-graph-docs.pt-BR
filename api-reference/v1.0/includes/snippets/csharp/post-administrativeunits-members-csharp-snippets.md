---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e73d864a3b0601bc971126382e565ce1d922e3bd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```