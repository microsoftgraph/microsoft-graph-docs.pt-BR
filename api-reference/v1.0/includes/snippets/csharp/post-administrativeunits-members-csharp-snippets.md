---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9495fcfca8c7a735d15a198d1f3944a14e6e1aba01417219f10c308a5c9fd3b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899563"
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